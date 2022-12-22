
# Pro-Person Segmentation

This repository contains a powerful semantic segmentation model designed to separate people from the background. It's built on a subset of the COCO segmentation dataset (http://cocodataset.org/), using only person class. The architecture, based on U-Net and DeepLab v3 (ASPP), is crafted and improved by huappe.

## Jupyter Notebooks

1. `pro-person-segmentation.ipynb`
    * Comprehensive notebook: data loading, model creation, training execution, inference running.
2. `post-processing.ipynb`
    * A platform for playing around with post-segmentation processing.
    * Includes functions for DOF effect emulation and background switching.
2. `kaggle_submission.ipynb`
    * Streamlines test images through the model.
    * Forms a submission file for Kaggle (translates all segmentation maps to CSV using RLE).

## Python Scripts

The scripts approximately replicate the content of `pro-person-segmentation.ipynb`.

1. `data.py`
    * Data Preparation - Contains classes for assembling training & validation data pipelines.
2. `model.py`
    * Model Definition - Class that shapes the network architecture.
3. `train.py`
    * Training Execution - Run this script to set off the training procedure.
4. `inference.py`
    * Inference Running - Run this script to carry out inference on a trained model.