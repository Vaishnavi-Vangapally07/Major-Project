# Bank Customer Churn Prediction using Machine Learning

## Project Overview
Customer churn is a major challenge in the banking industry. When customers leave a bank, it results in revenue loss and increased marketing costs to acquire new customers.

This project develops a Machine Learning model to predict whether a customer is likely to churn or stay with the bank. The system analyzes historical customer data and identifies patterns that indicate churn behavior.

The goal is to help banks take preventive actions to retain valuable customers.

---

## Dataset
The dataset used in this project is **bank_churn_data.csv**.

It contains information about bank customers such as:

- Credit Score
- Geography
- Gender
- Age
- Tenure
- Account Balance
- Number of Products
- Has Credit Card
- Is Active Member
- Estimated Salary

### Target Variable
Exited / Churn

- 0 → Customer stays with the bank
- 1 → Customer leaves the bank

Dataset Size:
- ~50,000 rows
- ~14 features

---

## Project Workflow

### 1. Data Loading
The dataset is loaded using Pandas and basic inspection is performed.

### 2. Data Preprocessing
Data preprocessing steps include:
- Cleaning column names
- Handling missing values
- Converting data types
- Separating categorical and numerical features

### 3. Exploratory Data Analysis (EDA)
Several visualizations are created to understand customer behavior:

- Churn distribution
- Churn by geography
- Churn by gender
- Balance vs churn
- Tenure vs churn
- Correlation heatmap

These analyses help identify important factors influencing customer churn.

### 4. Feature Engineering
Unnecessary columns such as customer IDs are removed and the dataset is divided into:

X → Input features  
y → Target variable

### 5. Data Scaling
StandardScaler is used to normalize numerical features before training machine learning models.

### 6. Handling Class Imbalance
Customer churn datasets are usually imbalanced. To address this issue, **SMOTE (Synthetic Minority Oversampling Technique)** is applied to balance the dataset.

---

## Machine Learning Models Used

The following models are trained and evaluated:

1. Logistic Regression  
2. K-Nearest Neighbors (KNN)  
3. Random Forest  
4. Support Vector Machine (SVM)

Each model is trained on the processed dataset and evaluated using performance metrics.

---

## Model Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score

These metrics help measure how well the model identifies churn customers.

---

## Technologies Used

Programming Language:
Python

Libraries:
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Imbalanced-learn (SMOTE)

Development Environment:
Jupyter Notebook

---

## Project Structure

Bank-Churn-Prediction  
│  
├── bank_churn.ipynb  
├── bank_churn_data.csv  
└── README.md  

---

## Applications

This project can help banks to:

- Identify customers who are likely to leave
- Improve customer retention strategies
- Reduce churn rates
- Perform targeted marketing campaigns
- Improve overall business decision making

---

## Future Improvements

Possible improvements include:

- Hyperparameter tuning
- Feature importance analysis
- Model explainability using SHAP
- Deploying the model using Flask or Streamlit
- Building a real-time churn prediction dashboard

---

## Author

Vaishnavi Vangapally  
Aspiring Data Scientist interested in Machine Learning, Data Analysis, and AI-based solutions.
