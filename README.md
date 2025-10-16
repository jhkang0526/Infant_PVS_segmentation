# INFANT PVS SEGMENTATION

## Data
Both *training* and *inference* datasets should be organized as the following structure:
```
dataset
│
└───subject 1
|   |    epc.nii.gz
|   |    mask.nii.gz(optional)
|   |    target.nii.gz(not required for the inference dataset)
└───subject 2
|   |    epc.nii.gz
|   |    mask.nii.gz
|   |    target.nii.gz
└───subject 3
|   |    epc.nii.gz
|   |    mask.nii.gz
|   |    target.nii.gz
│   ...
```
[developing Human Connectome Project (dHCP)](https://www.developingconnectome.org/) dataset was used for the training and evaluation. 
