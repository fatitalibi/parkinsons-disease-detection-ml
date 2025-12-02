# Parkinson's Disease Detection ML Project

## Overview
This project predicts whether a person has Parkinson's disease using a machine learning model trained on clinical voice measurements. It walks through data loading, preprocessing, model training, evaluation, and building a simple predictive system.

## Dataset
- **Name:** Parkinson's Disease Dataset (UCI Machine Learning Repository)
- **Type:** Tabular data with voice-based features
- **Features:** Multiple numeric voice measurements (frequency, amplitude, jitter, etc.)
- **Target:** `status`
  - `0` = Healthy
  - `1` = Parkinson's disease

## Methods

### 1. Data Preprocessing
- Loaded the dataset using **Pandas**
- Dropped non-numeric identifier columns
- Split the data into:
  - Features (`X`)
  - Target labels (`y`)
- Standardized the feature values using **StandardScaler**
- Split the data into training and test sets

### 2. Model Training
- Trained a **Support Vector Machine (SVM)** classifier
- Used the standardized training data
- Fit the model to learn the relationship between voice features and the `status` label

### 3. Evaluation
- Calculated accuracy on:
  - Training data
  - Test data
- Optionally examined metrics like confusion matrix or classification report to understand model performance

### 4. Predictive System
- Built a simple predictive system that:
  - Takes a new set of feature values as input
  - Applies the same preprocessing steps (scaling)
  - Uses the trained SVM model to predict whether the person has Parkinson's disease

## Results
- **Training Accuracy:** _88.5%_  
- **Test Accuracy:** _87.2%_
