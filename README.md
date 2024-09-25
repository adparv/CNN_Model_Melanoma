# CNN-Based Skin Cancer Detection

## Overview
This project implements a custom Convolutional Neural Network (CNN) to classify images of skin diseases, including melanoma. Melanoma accounts for 75% of skin cancer deaths, and early detection through automated systems could help reduce mortality.

## Dataset
The dataset contains 2357 images of 9 types of skin diseases, sourced from the International Skin Imaging Collaboration (ISIC). These diseases include:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Approach
1. Data preprocessing and visualization
2. Model building and training using CNN
3. Data augmentation to tackle overfitting
4. Handling class imbalance
5. Final model performance evaluation

## Model Performance
| Metric          | Value   |
|-----------------|---------|
| Training Accuracy| XX%     |
| Validation Accuracy | XX% |
| Loss (Training) | XX      |
| Loss (Validation) | XX    |

## Improvements
- Data augmentation techniques such as rotation, zoom, and flipping were used to improve the model's generalization.
- Class imbalance was handled using resampling techniques.

## How to Run
- Clone the repository.
- Follow the steps in the notebook to preprocess the data, build and train the model.
