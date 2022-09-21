# Weakly-supervised Semantic Segmentation for Histopathology Images

In this repository a collection of short literature reviews on the topic of WSSS for histopathological image data is created.
Occasionally, WSSS papers will be summarized whose methods have been evaluated with natural images only (e.g. from PASCAL VOC 2012 or ADE20K).
In addition, a short summary of the publicly available histopathological data sets for semantic segmentation will be compiled.

## Progress on Literature Review

### WSSS for Histopathology Images
| Index  |  Conference | Title | Annotation | LOD | My Review | Official Code | Datasets |
| :----: | :-------: | :--------: | :----------: | :--------: | :--: | :-------: | :-------: |
| 01     | ICCV 2019 | [CAMEL: A Weakly Supervised Learning Framework for Histopathology Image Segmentation](https://arxiv.org/pdf/1908.10555.pdf) | Image label (Binary) | Patch-level | *Coming soon* | No | [CAMELYON16](https://camelyon16.grand-challenge.org/Home/), [Colorectal Adenoma](https://github.com/ThoroughImages/CAMEL) |

### WSSS for Natural Images
| Index  |  Conference | Title | Annotation | LOD | My Review | Offical Code | Datasets |
| :----: | :-------: | :--------: | :----------: | :--------: | :--: | :-------: | :-------: |
| 01     | ICCV 2017 | [Simple Does It: Weakly Supervised Instance and Semantic Segmentation](https://arxiv.org/pdf/1603.07485.pdf) | Bounding Box (Multi-class) | Pixel-level | *Coming soon* | No | [PASCAL VOC2012](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/), VOC12+COCO |

## Summary of Semantic Segmentation Datasets for Histopathology
| Name      | Type          | #Labels/Img     | #Classes      | #Img       | #GT   | Image Size    | Resolution        | Paper    |
| :----:    | :-------:     | :--------:        | :----------:  | :--------:    | :--:              | :-------:     |:-------:          | :-------:|
| CoCaHis   | Colon Cancer  | 1 + BG            | 1 + BG        | 82            | 82                | 1388 × 1037   | 0.45 microns/px   | [Yes](https://www.sciencedirect.com/science/article/abs/pii/S1746809420305085)|



### TODO
- Add DL approach used within each paper
- 
