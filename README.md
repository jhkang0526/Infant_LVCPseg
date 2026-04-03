# Infant_LVCPseg

## [Paper Under Revision]

## Data
Both *training* and *inference* datasets should be organized as the following structure:
```
dataset
│
└───subject 1
|   |    T1.nii.gz
|   |    mask.nii.gz(optional)
|   |    target.nii.gz(not required for the inference dataset)
└───subject 2
|   |    T1.nii.gz
|   |    mask.nii.gz(optional)
|   |    target.nii.gz
└───subject 3
|   |    T1.nii.gz
|   |    mask.nii.gz
|   |    target.nii.gz
│   ...
```
[developing Human Connectome Project (dHCP)](https://www.developingconnectome.org/) dataset was used for the training and evaluation. 

## Requirements
  
- Python 3.12.4
- MONAI 1.3.2
- Numpy 1.26.4
- Pytorch 2.4.1

## How to run the code
### Training:
- Input: 3D T1-weigthed MR image
- Output: CP and LV Mask
- [Training (jupyter notebook)](training.ipynb)


### Inference:
- Input: 3D T1-weigthed MR image
- Output: CP and LV Mask
- [Inference (jupyter notebook)](inference.ipynb)

## Attribution

- MONAI: An open-source framework for deep learning in healthcare. [arXiv:2211.02701].

