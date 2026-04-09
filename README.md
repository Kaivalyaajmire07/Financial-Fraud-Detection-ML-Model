# Financial-Fraud-Detection-ML-Model
Kaivalyaajmire07/Financial-Fraud-Detection-ML-Model
# Financial Fraud Detection using Machine Learning

## Project Overview

This project focuses on building an **end-to-end machine learning model** to detect fraudulent financial transactions. The model analyzes transaction data, identifies patterns, and predicts whether a transaction is fraudulent or legitimate.

The project includes **data cleaning, feature engineering, model building, evaluation, and visualization**.

---

## Dataset Information

- **Total Records:** 6,362,620 transactions  
- **Total Features:** 11 columns  
- **Target Variable:** isFraud  

### Features

- step  
- type  
- amount  
- nameOrig  
- oldbalanceOrg  
- newbalanceOrig  
- nameDest  
- oldbalanceDest  
- newbalanceDest  
- isFraud  
- isFlaggedFraud  

---

## Project Workflow

### 1. Data Cleaning

- Checked missing values  
- Handled null values  
- Removed unnecessary columns  
- Data formatting  

---

### 2. Outlier Detection

- Used Boxplot visualization  
- Removed extreme transaction values using 99th percentile  

---

### 3. Multi-collinearity Handling

- Correlation matrix visualization  
- Removed highly correlated features:

- newbalanceOrig  
- newbalanceDest  

---

### 4. Feature Engineering

- Converted categorical variables using One-Hot Encoding  
- Selected relevant features for model training  

---

## Model Used

### Random Forest Classifier

### Why Random Forest?

- Works well with large datasets  
- Handles imbalanced data  
- High accuracy  
- Robust against overfitting  

---

## Model Training

- **Train-Test Split:** 80% Training / 20% Testing  
- Stratified sampling used for balanced training  

### Training Data Shape

- **5,039,194 rows**

### Testing Data Shape

- **1,259,799 rows**

---

## Model Performance

### Accuracy

- **Accuracy:** 96.69%  
- **ROC-AUC Score:** 99.67%  

---

## Confusion Matrix

| Actual | Predicted 0 | Predicted 1 |
|--------|-------------|-------------|
| 0 | 1,216,892 | 41,658 |
| 1 | 17 | 1,232 |

---

## Classification Report

- Precision  
- Recall  
- F1 Score  
- Support  

The model successfully identifies fraudulent transactions with **high recall**.

---

## Feature Importance

### Top Fraud Predicting Features

- oldbalanceOrg  
- amount  
- type_CASH_OUT  
- type_TRANSFER  
- type_PAYMENT  
- oldbalanceDest  
- step  

---

## Visualizations

The project includes:

- Boxplot for Outlier Detection  
- Correlation Heatmap  
- Confusion Matrix  
- Feature Importance Graph  

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Jupyter Notebook  

----------------------------------------


## Dataset

The original dataset is large (>400MB), so a sample dataset is provided.

File included:
- Fraud_Sample.csv (Sample dataset for testing)

-------------------------------------


## Author

**Kaivalya Mohan Ajmire**  
Machine Learning | Data Science | AI Enthusiast  

GitHub: https://github.com/Kaivalyaajmire07

## Conclusion

This project successfully builds a machine learning model for detecting fraudulent financial transactions with high accuracy and strong predictive performance. The model can be extended for real-time fraud detection in financial systems.
