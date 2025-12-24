# NazrinFlowersAI

This repository contains an individual deep learning project focused on classifying flowers using a Convolutional Neural Network (CNN) with data augmentation.

## Project Overview
The goal of this project is to train a CNN model on the **TensorFlow Flowers dataset**. The model learns to classify images of flowers into their respective categories, achieving robust performance through data augmentation and reproducible training.

## Dataset
- **Name:** TensorFlow Flowers  
- **Classes:** 5  
- **Images:** Varying size and resolution  
- **Splits:** 85% training, 15% testing  

## Model Architecture
- **Input:** 224x224x3 RGB images  
- **Layers:**
  - Data Augmentation (Random Flip, Rotation, Zoom)
  - Conv2D + ReLU + MaxPooling
  - Conv2D + ReLU + MaxPooling
  - Flatten
  - Dense (128 neurons, ReLU)
  - Dense (Softmax output for classification)
- **Optimizer:** Adam  
- **Loss:** Sparse Categorical Crossentropy  
- **Epochs:** 10  

## Data Augmentation
Applied to reduce overfitting and improve generalization:
- Horizontal flipping
- Random rotations
- Random zooms

## Results
- Training and validation accuracy plotted for analysis
- Test accuracy: ~80-90% (depending on training run)
- Model saved as `NazrinFlowersAI.h5`

## How to Run
1. Install dependencies:
```bash
pip install -r requirements.txt
