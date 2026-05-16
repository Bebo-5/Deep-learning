# Deep Learning Course Project - CIFAR-10 Image Classification

## Project Overview
This project implements Deep Learning models for image classification using the CIFAR-10 dataset.  
Two different Convolutional Neural Network (CNN) architectures were developed and compared:

- Simple CNN Model
- ResNet-like CNN Model

The project includes:
- Data preprocessing
- Data augmentation
- Model training
- Model evaluation
- Performance comparison
- Visualization of training results

---

# Problem Description
The goal of this project is to classify images from the CIFAR-10 dataset into one of 10 categories using Deep Learning techniques.

The CIFAR-10 dataset contains 60,000 color images divided into the following classes:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

Each image has a size of 32x32 pixels.

---

# Dataset Information

## Dataset Used
CIFAR-10 Dataset

## Dataset Link
https://www.cs.toronto.edu/~kriz/cifar.html

The dataset is automatically downloaded using torchvision.

---

# Technologies Used

- Python
- PyTorch
- Torchvision
- Matplotlib
- Pandas

---

# Data Preprocessing

The following preprocessing techniques were applied:

- Resizing images to 64x64
- Normalization
- Data Augmentation:
  - Random Horizontal Flip
  - Random Rotation

The dataset was divided into:
- Training Set
- Validation Set
- Testing Set

---

# Models Implemented

## Model A - Simple CNN
Architecture includes:
- 3 Convolutional Blocks
- Batch Normalization
- ReLU Activation
- Max Pooling
- Dropout Layer
- Fully Connected Layers

Optimizer:
- Adam

---

## Model B - ResNet-like CNN
Architecture includes:
- Residual Blocks
- Batch Normalization
- ReLU Activation
- Adaptive Average Pooling
- Dropout Layer

Optimizer:
- SGD with Momentum

---

# Model Enhancement Techniques

The following enhancement techniques were used:

- Dropout
- Batch Normalization
- Data Augmentation

---

# Training Configuration

| Parameter | Value |
|---|---|
| Epochs | 20 |
| Batch Size | 64 |
| Loss Function | CrossEntropyLoss |
| Optimizers | Adam / SGD |
| Learning Rate | 0.001 / 0.01 |

---

# Results

## Final Results Comparison

| Model | Test Accuracy | Test Loss |
|---|---|---|
| Simple CNN + Adam | 78.15% | 0.6512 |
| ResNet-like + SGD | 65.39% | 0.9730 |

---

# Visualizations

The following plots were generated:
- Training vs Validation Accuracy
- Training vs Validation Loss

These visualizations help monitor model performance during training.

---

# Project Structure
How to Run the Project
1. Clone the Repository
[git clone https://github.com/your-username/your-repository-name.git](https://github.com/Bebo-5/Deep-learning)
2. Navigate to the Project Folder
cd your-repository-name
3. Install Required Libraries
pip install -r requirements.txt
4. Run the Project
python deep_learning_project.py
