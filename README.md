# Fraud_detection_analysis

## Overview

This project implements machine learning models to detect fraudulent transactions.  
Two supervised algorithms are used:

- **Logistic Regression**
- **Random Forest Classifier**

The goal is to accurately classify transactions as:

- **0** → Legitimate  
- **1** → Fraudulent  

Special attention is given to handling **class imbalance** and evaluating models using meaningful metrics beyond simple accuracy.

---

## Dataset

The dataset contains transaction-level features with a binary fraud label.

Key characteristics:

- Highly imbalanced (fraud cases are rare)
- Mostly numerical features
- Some missing values handled carefully
- Target column: `Class` / `Fraud` / `Label`

---

## Methodology

1. Data loading and exploration  
2. Handling missing values  
3. Feature scaling (for Logistic Regression)  
4. Train-test split  
5. Model training  
6. Performance evaluation  
7. Feature importance analysis  

---

## Models Used

### Logistic Regression  
A linear model used as a baseline for fraud classification.  
It is fast, interpretable, and works well with scaled features.

### Random Forest  
An ensemble model that captures complex patterns and non-linear relationships.  
It also provides feature importance for better interpretability.

---

## Evaluation Metrics

Due to class imbalance, the following metrics were used:

- Precision  
- Recall  
- F1-score  
- ROC-AUC  

Accuracy alone is not sufficient for fraud detection tasks.

---

## Results

| Model | Precision | Recall | F1-score | ROC-AUC |
|------|-----------|--------|----------|---------|
| Logistic Regression | Good | Moderate | Balanced | Strong |
| Random Forest | Higher | Higher | Stronger | Very Strong |

Random Forest performed better in identifying fraudulent transactions.

---

## Visualizations

The notebook includes:

- Class distribution plots  
- Confusion matrices  
- ROC curves  
- Feature importance charts  

These visuals help explain both technical performance and business impact.

---

## Business Insights

- Fraudulent transactions show distinct behavioral patterns  
- Certain features strongly influence fraud probability  
- Random Forest is suitable for production-level detection  
- Logistic Regression supports explainability and compliance needs 
