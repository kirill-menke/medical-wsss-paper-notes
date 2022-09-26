# Weakly-supervised Semantic Segmentation for Histopathology Images

This repository contains an overview and short papers reviews of WSSS methods for histopathological image data.
Occasionally, WSSS papers dealing exclusively with semantic segmentation on natural images (e.g. from PASCAL-VOC 2012 or ADE20K) will be included.
I will update this list continuously during my current master thesis.

## Progress on Literature Review
The ground-truth annotation type used for training is mentioned in the *Annotation* column for each paper. 
For WSSS, it generally falls into one of the following categories (in order of decreasing informativeness): 
- Bounding box
- Scribble
- Point
- Image label

The *LOD* column roughly indicates the level of detail of the segmentation for each paper, e.g. whether a class is assigned to each pixel or only to each patch.
This is a very vague information, since the pathology images have a different resolution for the different methods and the chosen patch size differs too. Therefore the *LOD* should only serve as a rough estimation for the time being.
### WSSS for Histopathology Images

| Conference | Title | Annotation | LOD | Notes | Official Code | Datasets |
| :-------: | :-------- | :----------: | :--------: | :--: | :-------: | :------- |
| ICCV 2019 | [CAMEL: A Weakly Supervised Learning Framework for Histopathology Image Segmentation](https://arxiv.org/pdf/1908.10555.pdf) | image label (1280 x 1280) | pixel-level | [camel.md](paper_notes/CAMEL.md) | - | [CAMELYON16](https://camelyon16.grand-challenge.org/Home/), [Colorectal Adenoma](https://github.com/ThoroughImages/CAMEL) |
| MICCAI 2020 | [Weakly supervised multiple instance learning histopathological tumor segmentation](https://arxiv.org/abs/2004.05024) | image label (100k x 100k) | patch-level (224 x 224) | *coming soon* | [pytorch](https://github.com/marvinler/tcga_segmentation) | [TCGA](https://portal.gdc.cancer.gov/), [PatchCamelyon](https://patchcamelyon.grand-challenge.org/) |
| 2021 | [Data-efficient and weakly supervised computational pathology on whole-slide images](https://arxiv.org/pdf/2004.09666.pdf) | image label (100k x 100k) | patch-level | *coming soon* | [pytorch](https://github.com/mahmoodlab/CLAM) | [CAMELYON16](https://camelyon16.grand-challenge.org/), [CAMELYON17](https://camelyon17.grand-challenge.org/), [TCGA](https://portal.gdc.cancer.gov/), [CPTAC](https://proteomics.cancer.gov/data-portal) |
| MICCAI 2021 | [Learning Whole-Slide Segmentation from Inexact and Incomplete Labels using Tissue Graphs](https://arxiv.org/pdf/2103.03129.pdf) | image labels and scribbles (11k x 11k and 3k x 3k) | superpixel-level | *coming soon* | [pytorch](https://github.com/histocartography/seg-gini) | [SICAPv2](https://data.mendeley.com/datasets/9xxm58dvs3/1), UZH |
| MICCAI 2022 | [Transformer based multiple instance learning for weakly supervised histopathology image segmentation](https://arxiv.org/abs/2205.08878) | image label (3000 x 3000) | pixel-level | *coming soon* | [pytorch](https://github.com/Nexuslkl/Swin_MIL) | Colon cancer |
| ICIGP 2022 | [HistoSegResT: A Weakly Supervised Learning Method for Histopathology Image Segmentation](https://dl.acm.org/doi/pdf/10.1145/3512388.3512416) | image label (775 x 522) | pixel-level | *coming soon* | - | [GlaS](https://warwick.ac.uk/fac/cross_fac/tia/data/glascontest/)




### WSSS for Natural Images
| Conference | Title | Annotation | LOD | Notes | Offical Code | Datasets |
| :-------: | :-------- | :----------: | :--------: | :--: | :-------: | :------- |
| ICCV 2017 | [Simple Does It: Weakly Supervised Instance and Semantic Segmentation](https://arxiv.org/pdf/1603.07485.pdf) | bounding box (multi-class) | pixel-level | *coming soon* | no | [PASCAL VOC2012](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/), VOC12+COCO |

## Histopathology Datasets for Semantic Segmentation
| Name      | Type          | #Labels/Img     | #Classes      | #Img       | #GT   | Image Size    | Resolution        | Paper    |
| :----:    | :-------:     | :--------:        | :----------:  | :--------:    | :--:              | :-------:     |:-------:          | :-------:|
| [CAMELYON16](https://camelyon16.grand-challenge.org) | Lymph node metastasis | 1 | 1 | 400 | 400 | 100k x 100k | 0.25 microns/px | [yes](https://jamanetwork.com/journals/jama/article-abstract/2665774) |
| [CAMELYON17](https://camelyon17.grand-challenge.org/) | Lymph node metastasis | 1 | 1 | 1000 | 500 | 100k x 100k | 0.25 microns/px | [yes](https://ieeexplore.ieee.org/document/8447230)
| [CoCaHis](https://cocahis.irb.hr/) | Colon cancer  | 1 + BG            | 1 + BG        | 82            | 82                | 1037 x 1388   | 0.45 microns/px   | [yes](https://www.sciencedirect.com/science/article/abs/pii/S1746809420305085) |



## TODO
- Level-of-detail for segmentation resolution is too vague/ inaccurate
- Add image sizes of datasets used in papers since in some papers image label refers to small images (e.g. 3000 x 3000) while in others it refers to a WSI (e.g. 100k x 100k)
