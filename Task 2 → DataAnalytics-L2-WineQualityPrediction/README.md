# Wine Quality Prediction – Level 2 Task 2

## Project Overview

This project focuses on predicting wine quality using machine learning classification techniques based on the physicochemical properties of wine.

The original wine quality scores are converted into two categories:

- **Bad Wine:** Quality < 7
- **Good Wine:** Quality >= 7

Three classification models are trained and compared to identify the most suitable model for wine quality prediction.

## Objective

The main objectives of this project are:

- Analyze the Wine Quality dataset
- Perform data cleaning and exploratory data analysis
- Understand the distribution of wine quality scores
- Identify and analyze class imbalance
- Engineer a binary wine-quality classification target
- Train multiple classification models
- Evaluate and compare model performance
- Identify important features influencing predictions
- Select the best-performing model

## Dataset

**Dataset:** Wine Quality Dataset – Red & White Wine

**Source:** Kaggle

The dataset contains physicochemical properties of red and white wines along with their quality scores.

### Features

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol
- Wine Type

### Target

The original `quality` score is transformed into:

| Quality Score | Category |
|---|---|
| `< 7` | Bad |
| `>= 7` | Good |

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Machine Learning Models

The following classification algorithms are implemented:

### 1. Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees to improve prediction performance and reduce overfitting.

### 2. SGD Classifier

A linear classification algorithm trained using Stochastic Gradient Descent.

### 3. Support Vector Classifier (SVC)

A classification algorithm that finds an optimal decision boundary between different classes.

## Project Workflow

```text
Data Collection
      ↓
Data Loading
      ↓
Data Inspection
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Quality Distribution Analysis
      ↓
Class Imbalance Analysis
      ↓
Feature Engineering
      ↓
Train-Test Split with Stratification
      ↓
Feature Scaling
      ↓
Model Training
      ↓
Random Forest
SGD Classifier
SVC
      ↓
Model Evaluation
      ↓
Confusion Matrix
      ↓
Feature Importance
      ↓
Model Comparison
      ↓
Best Model Selection
