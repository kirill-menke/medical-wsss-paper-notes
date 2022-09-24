## Paper Information
#### Paper Title: [CAMEL: A Weakly Supervised Learning Framework for Histopathology Image Segmentation](https://arxiv.org/pdf/1908.10555.pdf)

#### Conference: ICCV 2019

#### Network Structure

<div  align="center">    
<img src="https://raw.githubusercontent.com/zhixuanli/segmentation-paper-reading-notes/master/images-folder/*.png" width="80%" />
</div>

## Short Summary
CAMEL achieves comparable performance with fully-supervised approaches in both tasks: instance-level classification and pixel-level segmentation.
It first performs a weakly-supervised patch classification using their proposed method cMIL. 
These patch labels are then used in a self-supervised manner to train a pixel-wise segmentation under full supervision with [DeepLabv2](https://github.com/google-research/deeplab2).

## Five questions about this paper:

### 1. [Problem Definition / Motivation] What problem is this paper trying to solve? 



### 2. [Contribution / Method] What's new in this paper? / How does this paper solve the above problems?



### 3. Details about the experiment

#### 3.1 Which Datasets are used?



#### 3.2 How is the experiment set up?



#### 3.3 What's the evaluation metric?



#### 3.4 Ablation Study



#### 3.5 What is the ranking of the experiment results?



### 4. Advantages (self-summary rather than the author's)



### 5. Disadvantages (self-summary rather than the author's)