# Super-Resolution-Image-Generation-for-APTOS-2019-Dataset-Based-on-SRGAN

## Overview
This project utilizes a Super-Resolution Generative Adversarial Network (SRGAN) to generate high-quality and high-resolution images from the APTOS 2019 dataset. SRGAN is particularly effective for upscaling low-resolution images to high-resolution outputs, making it well-suited for enhancing medical image datasets, including those used for diabetic retinopathy detection.

## Key Steps

### 1. Environment Setup
Prepare the necessary software and hardware environment:
- Ensure compatibility with GPU acceleration for optimal performance.
- NVIDIA RTX 4090 GPU is recommended and used in this setup.

### 2. Dataset Preparation
- Process the APTOS 2019 dataset:
  - Normalize images for consistent input.
  - Resize images to desired dimensions.
  - Split the dataset into training and validation subsets.

### 3. Configuration Setup
- In **`APTOS_SR.ipynb`** file: 
  - Hyperparameters such as learning rate, batch size, and epochs.
  - File paths for dataset storage and output results.
  - Training settings for efficient execution.

### 4. Defining the SRGAN Model Structure
- Implement the SRGAN architecture:
  - Design the generator network for image upscaling.
  - Define the discriminator network to distinguish between real and generated high-resolution images.
  - Utilize perceptual loss, combining content loss and adversarial loss, to achieve high-quality image reconstruction.

### 5. Defining the Training Process
- Import the preprocessed dataset for training.
- Implement the training loop:
  - Compute losses (e.g., adversarial and perceptual losses).
  - Perform backpropagation and model updates.
  - Periodically evaluate the generated images to monitor training progress.

### 6. Initialize Training
- Begin training the SRGAN model.
- For demonstration purposes, results are provided for **60 epochs**. Users can scale up the training process to **600 or 1000 epochs** based on project requirements.

### 7. Model Evaluation
- Evaluate the performance of the trained SRGAN model using the following metrics:
  - **PSNR (Peak Signal-to-Noise Ratio):** Measures image quality.
  - **SSIM (Structural Similarity Index):** Assesses structural similarity between images.

## File Details
- All required code is contained in the file **`APTOS_SR.ipynb`**.
- The notebook provides:
  - Implementation of the SRGAN model.
  - Training process scripts.
  - Sample outputs from the model.


