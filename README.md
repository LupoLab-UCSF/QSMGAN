# QSMGAN
Efficient and accurate QSM dipole invsersion based on 3D U-Net and GAN


**Overview:** This deep learning tool takes preprocessed phase and magnitude data and produces processed QSM images. To read about the network architecture and training process please refer to our article: https://www.sciencedirect.com/science/article/pii/S1053811919309802?via%3Dihub

**Requirements:**

PyTorch >= 0.4
Matlab 2015b

IMPORTANT: To fully utilize this project, create anaconda or virtualenv on machines with GPUs and install packages used in pytorch code.


**Usage:**

To apply trained models to new data, 

1. Run SEPIA https://sepia-documentation.readthedocs.io/en/latest/
2. Run DL script with local field from step 1 (post background field removal), for example: 

python make_swan_qsm_DL.py /path/to/phase/data/subID_tissue_phase.nii

