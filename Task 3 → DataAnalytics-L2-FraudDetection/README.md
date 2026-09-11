# Fraud Detection

## Oasis Infobyte Internship - Task 3

### Objective

Build a machine learning model to detect fraudulent credit card transactions using a highly imbalanced dataset.

### Dataset

Credit Card Fraud Detection Dataset from Kaggle.

Dataset Link:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

The dataset contains 284,807 transactions, including 492 fraudulent transactions.

### Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- Jupyter Notebook

### Project Steps

1. Load and understand the dataset
2. Check missing and duplicate values
3. Analyze fraudulent and legitimate transactions
4. Perform exploratory data analysis
5. Analyze transaction amounts
6. Analyze fraud by time of day
7. Split the data into training and testing sets
8. Scale the features
9. Handle class imbalance using SMOTE
10. Train Logistic Regression model
11. Train Random Forest model
12. Evaluate the models
13. Compare Precision, Recall, F1-Score, and ROC-AUC
14. Create confusion matrices
15. Analyze feature importance
16. Discuss model scalability

### Models Used

#### Logistic Regression

Used as a baseline classification model with SMOTE to handle the class imbalance.

#### Random Forest

Used as an ensemble classification model with `class_weight="balanced"` to give more importance to fraudulent transactions.

### Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

Recall and Precision are given particular importance because the dataset is highly imbalanced and accuracy alone can be misleading.

### Class Imbalance

Fraudulent transactions represent only about 0.17% of all transactions. A model predicting almost every transaction as legitimate could achieve very high accuracy while failing to detect fraud.

Therefore, SMOTE and class weighting are used to improve fraud detection performance.

### Feature Analysis

Random Forest feature importance is used to identify the features that contribute most to fraud prediction.

The `V1` to `V28` features are anonymized PCA-transformed features, so their individual business meanings cannot be directly interpreted.

### Scalability

The project also discusses how the fraud detection system could handle approximately 1 million transactions per hour, which is around 278 transactions per second.

A production system could use real-time streaming, scalable model-serving APIs, load balancing, monitoring, and periodic model retraining.

### Conclusion

This project demonstrates a complete machine learning workflow for credit card fraud detection, including exploratory data analysis, class imbalance handling, model development, evaluation, feature analysis, and scalability considerations.

The project highlights the importance of using Precision, Recall, F1-Score, and ROC-AUC instead of relying only on accuracy when working with highly imbalanced fraud detection data.
