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
|   |    target.nii.gzhttps://github.com/jhkang0526/Infant_PVS_segmentation/blob/main/README.md
│   ...
```
[developing Human Connectome Project (dHCP)](https://www.developingconnectome.org/) dataset was used for the training and evaluation. 

## Requirements

python 3 is required and `python 3.6.4` was used in the study.  

Please use ```pip install requirements.txt``` to install the requirements.  

## How to run the code
### Pseudo labeling
- Input: 3D T2-weigthed MR image & Tissue segmentation from [infant freesurfer](https://surfer.nmr.mgh.harvard.edu/fswiki/infantFS) or [dHCP pipeline](https://github.com/BioMedIA/dhcp-structural-pipeline)
- Output: refinement BG and BGPVS Mask
- [Pseudo labeling (jupyter notebook)](pseudo_labeling.ipynb)

  
### Training:
- Input: 3D T2-weigthed MR image
- Output: refinement BG and BGPVS Mask
- [Pseudo labeling (jupyter notebook)](training.ipynb)


### Inference:
- Input: 3D T2-weigthed MR image
- Output: refinement BG and BGPVS Mask
- [Pseudo labeling (jupyter notebook)](inference.ipynb)

