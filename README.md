# Alzheimers-diagnosis-model

This repository presents an initial implementation for detecting Alzheimer's disease stages from MRI brain scans using Convolutional Neural Networks (CNNs) and pre-trained EfficientNet models. The aim is to develop an AI-powered tool that can assist in the early and accurate detection of Alzheimer's by analyzing brain imaging data.

---

Dataset

The dataset used is from [Kaggle - Alzheimer MRI Dataset](https://www.kaggle.com/datasets/sachinkumar413/alzheimer-mri-dataset) and is structured into four categories:

- **NonDemented**
- **VeryMildDemented**
- **MildDemented**
- **ModerateDemented**

  Models Implemented

### 1. EfficientNetB0 (Transfer Learning)
- Used pre-trained weights from ImageNet.
- Applied additional dense layers with dropout and L2 regularization.
- Achieved training accuracy up to ~83% in initial runs.

### 2. CNN – Basic
- Three convolutional + max-pooling blocks.
- Flattened to dense layers ending in softmax activation.
- No augmentation or normalization initially.

### 3. CNN – With Data Augmentation
- Same structure as above.
- Included `ImageDataGenerator` for real-time augmentation (rotation, flip, zoom, etc.).
