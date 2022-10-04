## Paper Information
#### Paper Title: Transformer based multiple instance learning for weakly supervised histopathology image segmentation

#### Conference: MICCAI 2022

#### Official Code: https://github.com/Nexuslkl/Swin_MIL

#### Network Structure

![swin_mil](images/swin_mil.png)

## Short Summary
The Swin transformer is incorporated into the MIL framework to encode long-range relationships between instances within a bag.
It employs so-called deep supervision, meaning additional "companion" objective functions at different hidden layers (here: after each transformer stage) are introduced. The final loss is then computed from the output loss plus the companion losses.
A decoder produces pixel-wise predictions using the feature maps after each stage of the transformer. A fusion layer is employed to combine these side-outputs of different scales to produce the final segmentation map.

## Five questions about this paper:

### 1. [Problem Definition] What problem is this paper trying to solve? 
It tackles the problem of WSI patch segmentation using only binary image-level labels of WSIs


### 2. [Method] What's new in this paper?
It's the first method performing a weakly-supervised segmentation using a combination of Transformer and MIL, which enables to produce features that encode long-distance relationships between instances. Usually instances of a bag are independent of eachother in MIL.


### 3. Details about the experiment

#### 3.1 Which Datasets are used?
A private colon cancer dataset is used with 330 cancer positive (CA) and 580 cancer negative (NC) H&E stained images.
They were obtained at a 40x magnification, i.e. 226nm/pixel. The original image resolution of 3000 x 3000 is downsampled to 256 x 256 during expiriments in order the images can fit into memory.
250 CA and 500 NC images were used for training. 80 CA and 80 NC images were used for testing.


#### 3.2 How is the experiment set up?



#### 3.3 What's the evaluation metric?



#### 3.4 Ablation Study



#### 3.5 What is the ranking of the experiment results?



### 4. Advantages (self-summary rather than the author's)



### 5. Disadvantages (self-summary rather than the author's)