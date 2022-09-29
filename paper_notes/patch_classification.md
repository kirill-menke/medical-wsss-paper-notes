## Paper Information
#### Paper Title: [Weakly supervised multiple instance learning histopathological tumor segmentation](https://arxiv.org/abs/2004.05024)

#### Conference: MICCAI 2020

#### Official Codes
#### Network Structure

![Image](images/patch_classification.png)

## Short Summary
Within this paper a WSSS algorithm is proposed based on binary image-level labels of WSIs.
MIL is applied to train an instance classifier model. Therefore, an WSI is divided into equally-sized patches (224 x 224) which are interpreted as instances.


## Five questions about this paper:

### 1. [Problem Definition] What problem is this paper trying to solve? 
It tackles the problem of WSI segmentation using only binary image-level labels of WSIs


### 2. [Method] How does this paper solve the above problems?
It trains a binary patch classifier which is then used to perform a segmentation of the gigapixel WSI.
To train this model, a new method is proposed which enables to use patches with uncertain labels.


### 3. Details about the experiment

#### 3.1 Which Datasets are used?



#### 3.2 How is the experiment set up?



#### 3.3 What's the evaluation metric?
- Precision
- Recall
- F1-Score
- AUC


#### 3.4 What is the ranking of the experiment results?
No comparision with other methods was performed. 


### 4. Advantages (self-summary rather than the author's)



### 5. Disadvantages (self-summary rather than the author's)