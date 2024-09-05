# SAM-ViT Masking Approach for Segmentation
This repository provides a streamlined implementation of the SAM-ViT model, designed for efficient image segmentation tasks.

# Key Features
  ## Data Loading & Preprocessing:

Load and pad images and masks from designated folders.
Break down large images into smaller patches for easier processing.
Utilize the MONAI library to create a custom dataset (SAMDataset) for medical imaging.
## Model Configuration:

Set up the SAM-ViT model (SamModel) using Huggingface Transformers.
Optimize by freezing parameters of the vision and prompt encoders.
## Training Setup:

Configure training parameters such as epochs, learning rate, and optimizer (Adam).
Implement a training loop to compute losses, update parameters, and save model weights after each epoch.
## Loss Calculation:

Apply MONAI’s loss functions (e.g., DiceCELoss) for segmentation during training.
