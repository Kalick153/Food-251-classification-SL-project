# Food Image Classification Project

## Introduction

This project explores image classification using both traditional and deep learning approaches. Our goal is to classify food images into 251 fine-grained categories using the FoodX-251 dataset. We preprocess the images, perform feature extraction using ORB (Oriented FAST and Rotated BRIEF), and classify the images with Random Forests on the Bag of Words (BoW) representations. Additionally, we train a custom Convolutional Neural Network (CNN) for comparison. Model performance is evaluated.

## Dataset Description

Food classification is a challenging problem due to the large number of categories and high visual similarity between different foods. The FoodX-251 dataset contains 251 fine-grained food categories with 118,475 training images collected from the web. Human-verified labels are provided for the validation set of 11,994 images, which is used as a test set in this report. The initial set of 118,475 images was split into training and validation sets.

## Repository Contents

- **data**: Contains the best model and also loss values.
- **Custom_CNN_part (2).ipynb**: Notebook for training the custom CNN model.
- **Dataset_and_features_BoW.ipynb**: Notebook for the traditional machine learning approach using BoW.
- **SupervisedReport.pdf**: Detailed project [report](./SupervisedReport.pdf).
- **best_model_training.ipynb**: Notebook for training the CNN model that performed the best.

## Best Model's Performance

(Some classes were not predicted at all. Marble cake class is the least represented in the dataset.)
Here we provide the onformation on the best model's performance and what classes were not predicted by the model at all.

#### Training Set
- **Class 162 - Marble Cake**
  - Accuracy: 0.3718
  - Precision: 0.4067
  - Recall: 0.3718
  - F1-score: 0.3602
  - Top-5 Accuracy: 0.6600

#### Validation Set
- **Class 162 - Marble Cake**
  - Accuracy: 0.3014
  - Precision: 0.3302
  - Recall: 0.3014
  - F1-score: 0.2890
  - Top-5 Accuracy: 0.5770

#### Test Set
- **Class 162 - Marble Cake**
- **Class 238 - Rugulah**
  - Accuracy: 0.3515
  - Precision: 0.3914
  - Recall: 0.3515
  - F1-score: 0.3411
  - Top-5 Accuracy: 0.6422
