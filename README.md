# INFANT PVS SEGMENTATION

## Data
Both *training* and *inference* datasets should be organized as the following structure:
```
dataset
│
└───subject 1
|   |    T2.nii.gz
|   |    mask.nii.gz(optional)
|   |    target.nii.gz(not required for the inference dataset)
└───subject 2
|   |    T2.nii.gz
|   |    mask.nii.gz
|   |    target.nii.gz
└───subject 3
|   |    T2.nii.gz
|   |    mask.nii.gz
|   |    target.nii.gz
│   ...
```
[developing Human Connectome Project (dHCP)](https://www.developingconnectome.org/) dataset was used for the training and evaluation. 

## Requirements

python 3 is required and `python 3.6.4` was used in the study.  

Please use ```pip install requirements.txt``` to install the requirements.  

## How to run the code
### Training:
Training script is at  **./train**

Use the following command to run the training script:


## Inference:

Inference script is at  **./predict**. The corresponding BG and BGPVS segmentation results will be saved under the same directory as the inference dataset. 

Use the following command to run the inference script:

