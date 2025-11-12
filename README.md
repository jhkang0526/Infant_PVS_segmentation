# INFANT PVS SEGMENTATION

## [Paper Under Revision]

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

- Python 3.12.4
- MONAI 1.3.2
- Numpy 1.26.4
- Pytorch 2.4.1

## How to run the code
### Pseudo labeling
- Input: 3D T2-weigthed MR image & Tissue segmentation from [infant freesurfer](https://surfer.nmr.mgh.harvard.edu/fswiki/infantFS) or [dHCP pipeline](https://github.com/BioMedIA/dhcp-structural-pipeline)
- Output: refinement BG and BGPVS Mask
- [Pseudo labeling (jupyter notebook)](pseudo_labeling.ipynb)

  
### Training:
- Input: 3D T2-weigthed MR image
- Output: refinement BG and BGPVS Mask
- [Training (jupyter notebook)](training.ipynb)


### Inference:
- Input: 3D T2-weigthed MR image
- Output: refinement BG and BGPVS Mask
- [Inference (jupyter notebook)](inference.ipynb)

## Attribution

- MONAI: An open-source framework for deep learning in healthcare. [arXiv:2211.02701]. 

**This repository uses a loss function re-implemented from:**
- Gros C et al. (2021). SoftSeg: Advantages of soft versus binary training for image segmentation. Medical Image Analysis, 102038.  
  DOI: https://doi.org/10.1016/j.media.2021.102038

