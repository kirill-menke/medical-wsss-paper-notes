# Weakly-supervised Semantic Segmentation for Histopathology Images

In this repository a collection of short literature reviews on the topic of WSSS for histopathological image data is created.
Occasionally, WSSS papers will be summarized whose methods have been evaluated with natural images only (e.g. from PASCAL VOC 2012 or ADE20K).
In addition, a short summary of the publicly available histopathological data sets for semantic segmentation will be compiled.

## Progress on Literature Review

### WSSS for Histopathology Images

| Conference | Title | Annotation | LOD | My Review | Official Code | Datasets |
| :-------: | :-------- | :----------: | :--------: | :--: | :-------: | :------- |
| ICCV 2019 | [CAMEL: A Weakly Supervised Learning Framework for Histopathology Image Segmentation](https://arxiv.org/pdf/1908.10555.pdf) | image label (binary) | patch-level | *coming soon* | - | [CAMELYON16](https://camelyon16.grand-challenge.org/Home/), [Colorectal Adenoma](https://github.com/ThoroughImages/CAMEL) |
| MICCAI 2020 | [Weakly supervised multiple instance learning histopathological tumor segmentation](https://arxiv.org/abs/2004.05024) | image label (binary) | patch-level | *coming soon* | [pytorch](https://github.com/marvinler/tcga_segmentation) | [TCGA](https://portal.gdc.cancer.gov/), [PatchCamelyon](https://patchcamelyon.grand-challenge.org/) |
| 2021 | [Data-efficient and weakly supervised computational pathology on whole-slide images](https://arxiv.org/pdf/2004.09666.pdf) | image label (binary) | patch-level | *coming soon* | [pytorch](https://github.com/mahmoodlab/CLAM) | [CAMELYON16](https://camelyon16.grand-challenge.org/), [CAMELYON17](https://camelyon17.grand-challenge.org/), [TCGA](https://portal.gdc.cancer.gov/), [CPTAC](https://proteomics.cancer.gov/data-portal) |
| MICCAI 2021 | [Learning Whole-Slide Segmentation from Inexact and Incomplete Labels using Tissue Graphs](https://arxiv.org/pdf/2103.03129.pdf) | image labels and scribbles (multi-class) | superpixel-level | *coming soon* | - | [SICAPv2](https://data.mendeley.com/datasets/9xxm58dvs3/1), UZH |
| MICCAI 2022 | [Transformer based multiple instance learning for weakly supervised histopathology image segmentation](https://arxiv.org/abs/2205.08878) | patch label (binary) | pixel-level | *coming soon* | [pytorch](https://github.com/Nexuslkl/Swin_MIL) | Colon cancer |
| ICIGP 2022 | [HistoSegResT: A Weakly Supervised Learning Method for Histopathology Image Segmentation](https://dl.acm.org/doi/pdf/10.1145/3512388.3512416) | image label (binary) | pixel-level | *coming soon* | - | [GlaS](https://warwick.ac.uk/fac/cross_fac/tia/data/glascontest/)




### WSSS for Natural Images
| Conference | Title | Annotation | LOD | My Review | Offical Code | Datasets |
| :-------: | :-------- | :----------: | :--------: | :--: | :-------: | :------- |
| ICCV 2017 | [Simple Does It: Weakly Supervised Instance and Semantic Segmentation](https://arxiv.org/pdf/1603.07485.pdf) | bounding box (multi-class) | pixel-level | *coming soon* | no | [PASCAL VOC2012](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/), VOC12+COCO |

## Summary of Semantic Segmentation Datasets for Histopathology
| Name      | Type          | #Labels/Img     | #Classes      | #Img       | #GT   | Image Size    | Resolution        | Paper    |
| :----:    | :-------:     | :--------:        | :----------:  | :--------:    | :--:              | :-------:     |:-------:          | :-------:|
| CoCaHis   | Colon Cancer  | 1 + BG            | 1 + BG        | 82            | 82                | 1388 × 1037   | 0.45 microns/px   | [yes](https://www.sciencedirect.com/science/article/abs/pii/S1746809420305085)|



### TODO
- Level-of-detail for segmentation resolution is too vague/ inaccurate
- Add image sizes of datasets used in papers since in some papers image label refers to small images (e.g. 3000 x 3000) while in others it refers to a WSI (e.g. 100k x 100k)
