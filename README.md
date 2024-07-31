# Customer Purchase Prediction

## Project Overview

This project aims to predict whether a customer will make a purchase in the following month based on their transaction history. We explored various machine learning models, including Logistic Regression and Gaussian Naive Bayes, to determine the best approach for this prediction task.

## Dataset

The dataset used for this project includes customer transaction records, with features such as:
- InvoiceDate
- Country
- CustomerID
- InvoiceNo
- TotalPrice
- Revenue

## Data Preparation and Feature Engineering

### Steps:
1. **Data Loading and Cleaning**: The dataset was cleaned to handle missing values and ensure consistency.
2. **Date Conversion**: The 'InvoiceDate' column was converted to datetime format.
3. **Target Variable Creation**: A binary target variable, `NextMonthPurchase`, was created to indicate whether a purchase occurred in the following month.
4. **Encoding Categorical Features**: Categorical features like 'Country' were encoded using `LabelEncoder`.
5. **Feature Engineering**: New features were created to capture customer behavior:
   - Recency: Days since the last purchase.
   - Frequency: Number of unique purchases.
   - Monetary: Total spending.
   - Average Order Value: Average amount spent per order.
   - Revenue: Total revenue generated.

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
   git clone https://github.com/your-repository-link
   cd your-repository-link
