# Sales Data Analysis

## Overview

In this report My aims to predict whether a customer will make a purchase in the following month based on their transaction history. We explored various machine learning models, including Logistic Regression and Gaussian Naive Bayes, to determine the best approach for this prediction task.

## Dataset

The dataset used for this project includes customer transaction records, with features such as:
- InvoiceDate
- Country
- CustomerID
- InvoiceNo
- Description
- Quantity
- Unit Price


## Data Preparation and Feature Engineering

### Steps:
1. Data Collection.
2. Data Exploration and Cleaning.
3. Descriptive Analysis.
4. Sales Trend.
5. Customer Analysis.
6. Geographical Analysis.
7. Recommendations.
8. Machine Learning Model

## Model Training and Evaluation

### Logistic Regression
- **Accuracy**: 0.46
- **Precision**: 0.22
- **Recall**: 0.85
- **F1 Score**: 0.35
- **ROC-AUC Score**: 0.67

### Gaussian Naive Bayes
- **Accuracy**: 0.63
- **Precision**: 0.58
- **Recall**: 0.91
- **F1 Score**: 0.71
- **ROC-AUC Score**: 0.62

### Summary
Based on the evaluation metrics, the Naive Bayes classifier demonstrated superior performance in predicting the likelihood of a customer making a purchase in the next month compared to the logistic regression model. Therefore, in my opinion, the Naive Bayes classifier is the most suitable model for predicting future customer purchases.

## Usage

### Requirements
- pandas
- scikit-learn
- imbalanced-learn

### Installation
1. Clone the repository:
   ```bash
   https://github.com/Vineetg2003/Sales-Data-Analysis

