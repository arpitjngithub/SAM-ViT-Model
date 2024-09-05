# Masking Approach using SAM-ViT Model

### This repository contains code for a masking approach using the SAM-ViT (Self-Attention Mechanism for Vision Transformers) model, tailored for segmentation tasks.

## Overview

The code provided in this repository includes:

## 1. Data Loading and Preprocessing:

Functions to load and pad images and masks from specified folders.
Patching large images into smaller patches for efficient processing.
Creation of a custom dataset (SAMDataset) using the MONAI library for medical imaging.

## 2. Model Setup:

Initialization and configuration of the SAM-ViT model (SamModel) using the Huggingface Transformers library.
Optimization of the model setup to freeze parameters of the vision and prompt encoders.

## 3. Training Setup:

Configuration of training parameters such as epochs, learning rate, and optimizer (Adam).
Implementation of a training loop that iterates through epochs, computes losses, and updates model parameters.
Saving of model weights after each epoch to specified directories.

## 4. Loss Functions:

Utilization of MONAI library's loss functions (DiceCELoss, etc.) for calculating segmentation losses during training.


# USAGE

## Environment Setup

1. Install required packages:

pip install torch torchvision numpy matplotlib monai transformers

## Training the Model

To train the model for different class change the image_folder and mask-folder path
