# Level 2 – Task 1: Predicting House Prices with Linear Regression

## Project Overview

This project is completed as part of the **Oasis Infobyte Data Analytics Internship – Level 2, Task 1**.

The objective of this project is to build a Machine Learning model that predicts house prices based on various property characteristics such as living area, overall quality, neighborhood, house age, number of rooms, bathrooms, garage capacity, and lot area.

The project uses the **House Prices: Advanced Regression Techniques** dataset from Kaggle.

---

## Objectives

- Perform Exploratory Data Analysis (EDA)
- Check and handle missing values
- Analyze the distribution of house prices
- Select relevant features for prediction
- Perform feature engineering
- Encode categorical variables using One-Hot Encoding
- Analyze feature correlations using a heatmap
- Split the data into 80% training and 20% testing sets
- Build a Linear Regression model
- Evaluate the model using MSE, RMSE, and R² Score
- Compare actual and predicted house prices
- Perform residual analysis
- Analyze regression coefficients
- Compare Linear Regression with Ridge and Lasso Regression
- Generate predictions for Kaggle submission

---

## Dataset

**Dataset:** House Prices – Advanced Regression Techniques

**Source:** Kaggle

##  Exploratory Data Analysis

The following analyses were performed:

- Dataset shape and structure
- Data types
- Descriptive statistics
- Duplicate-value checking
- Missing-value analysis
- Distribution of `SalePrice`
- Living area vs. house price
- Overall quality vs. house price
- Neighborhood vs. house price
- Correlation heatmap

---

##  Data Preprocessing

The following preprocessing techniques were applied:

- Numerical missing values were handled using median imputation.
- Categorical missing values were handled using the most frequent value.
- Categorical features were converted into numerical features using One-Hot Encoding.
- Numerical features were standardized using `StandardScaler`.
- The dataset was divided into 80% training and 20% testing data.

A preprocessing pipeline was created using Scikit-learn to ensure consistent data transformation.

---

## Machine Learning Models

### 1. Linear Regression

Linear Regression was used as the primary model to predict house prices based on the selected features.

### 2. Ridge Regression

Ridge Regression was implemented as a regularized alternative to Linear Regression to reduce the impact of large coefficients and improve model stability.

### 3. Lasso Regression

Lasso Regression was used as another regularization technique that can reduce less important feature coefficients toward zero.

---

## Model Evaluation

The models were evaluated using the following metrics:

### Mean Squared Error (MSE)

Measures the average squared difference between actual and predicted prices.

**Lower MSE indicates better performance.**

### Root Mean Squared Error (RMSE)

Measures the average prediction error in the same unit as the target variable.

**Lower RMSE indicates better performance.**

### R² Score

Measures how much of the variation in house prices is explained by the model.

**Higher R² indicates better performance.**

---

## Visualizations

The project includes the following visualizations:

- SalePrice Distribution
- Correlation Heatmap
- Living Area vs. House Price
- Overall Quality vs. House Price
- Neighborhood vs. House Price
- Actual vs. Predicted House Prices
- Residual Plot
- Regression Coefficient Analysis
- Model Comparison

---

## Actual vs. Predicted Prices

An Actual vs. Predicted scatter plot was created to evaluate the prediction performance.

Points closer to the diagonal reference line indicate predictions that are closer to the actual house prices.

---

## Residual Analysis

Residual analysis was performed to evaluate the errors made by the Linear Regression model.

Residuals were calculated as:

`Residual = Actual Price - Predicted Price`

The residual plot was used to check whether the errors were randomly distributed around zero without a strong systematic pattern.

---

## Coefficient Analysis

The Linear Regression coefficients were analyzed to identify features with relatively higher positive and negative effects within the fitted model.

This analysis helps understand how different property characteristics influence the model's predicted house prices.

---

## Kaggle Competition

The project uses the Kaggle **House Prices: Advanced Regression Techniques** competition.

The workflow includes:

1. Joining the Kaggle competition
2. Downloading `train.csv` and `test.csv`
3. Training the Machine Learning model
4. Generating predictions for `test.csv`
5. Creating the required `submission.csv`
6. Submitting the predictions to Kaggle
7. Evaluating the result on the Kaggle leaderboard
