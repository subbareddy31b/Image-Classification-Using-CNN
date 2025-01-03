# Image Classification Using VGG13 and ResNet18

## Overview
This project involves image classification using deep learning models, specifically **VGG13** and **ResNet18**, to classify images from a dataset containing three categories: vehicles, food, and dogs. The dataset consists of 10k images from each category, totaling 30,000 images. 

Both models were trained, and optimizations were applied, including regularization, early stopping, and dropout to enhance model performance.

## Key Features
- 🧑‍💻 **VGG13 Model**: A deep convolutional neural network with 13 layers for image classification.
- 🔄 **ResNet18 Model**: A deep residual network with 18 layers for better generalization.
- 🧹 **Data Preprocessing**: Normalization of pixel values to improve convergence during training.
- 🔧 **Regularization Techniques**: Dropout, L2 regularization, and early stopping to prevent overfitting.
- 📊 **Performance Metrics**: Achieved high precision, recall, and F1 scores for both models.

## Dataset
The dataset contains 30,000 images (10k images for each of the following categories):
- 🚗 **Vehicles**
- 🍔 **Food**
- 🐶 **Dogs**

The images were preprocessed by normalizing pixel values using standard mean and standard deviation values.

## Model Architecture
### VGG13 Model
VGG13 is a deep convolutional neural network architecture that consists of 13 layers. Here's an overview of its structure:
- 🌀 **Multiple convolutional layers** with ReLU activation.
- 🔽 **Max-pooling layers** for dimensionality reduction.
- 🔒 **Fully connected layers** at the end.

We applied regularization techniques like dropout and early stopping to prevent overfitting and improve generalization.

### Confusion Matrix
![output](https://github.com/user-attachments/assets/1d45f8f6-d8d8-4250-b80b-17508f11f68d)


#### Training Results (VGG13)
- **Test Accuracy**: 89%
- **Precision**: 0.8930  
- **Recall**: 0.8917

### Classification Report
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| **0** | 0.87      | 0.88   | 0.87     | 2002    |
| **1** | 0.86      | 0.89   | 0.88     | 1996    |
| **2** | 0.95      | 0.90   | 0.93     | 2002    |

| **Overall Metrics** | **Value** |
|----------------------|-----------|
| **Accuracy**         | 0.89      |
| **Total Support**    | 6000      |

![output](https://github.com/user-attachments/assets/02f782e9-bcbe-4602-bf64-1a4b1db4dccc)

### ResNet18 Model
ResNet18 is a residual network architecture with 18 layers. It uses skip connections, which helps in training deeper networks by mitigating the vanishing gradient problem.

### Confusion Matrix
![output](https://github.com/user-attachments/assets/8ef75b03-1109-43a6-884a-2fa3c0120930)

#### Training Results (ResNet18)
- **Test Accuracy**: 87.2%
- **Precision**: 0.873
- **Recall**: 0.87

### Classification Report
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| **0** | 0.90      | 0.78   | 0.84     | 2002    |
| **1** | 0.89      | 0.87   | 0.88     | 1996    |
| **2** | 0.87      | 0.96   | 0.89     | 2002    |

| **Overall Metrics** | **Value** |
|----------------------|-----------|
| **Accuracy**         | 0.87      |
| **Total Support**    | 6000      |

![output](https://github.com/user-attachments/assets/d1f28df0-b424-4f75-be96-d3355a0fa591)
