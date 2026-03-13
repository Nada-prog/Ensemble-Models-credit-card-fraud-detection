# Credit Card Fraud Detection using Ensemble Learning

## Overview

This project focuses on detecting fraudulent credit card transactions using machine learning techniques on a highly imbalanced dataset. The goal is to compare different sampling strategies and ensemble models to improve the detection of rare fraud cases.

The dataset contains transactions made by credit cards in September 2013 and is highly imbalanced, with fraud cases representing only a small fraction of all transactions.

Dataset used: Credit Card Fraud Detection Dataset from Kaggle.

---

## Project Workflow

### 1. Data Preparation

* Loaded the dataset and explored class distribution.
* Split the data into training and testing sets.
* Applied feature scaling using StandardScaler.

### 2. Baseline Model

A Logistic Regression model was trained without handling class imbalance to establish a baseline performance.

Evaluation metrics used:

* Precision
* Recall
* F1-score
* ROC-AUC

This step demonstrates why accuracy alone is misleading in imbalanced datasets.

---

### 3. Sampling Techniques

Several sampling techniques were applied to handle class imbalance:

* Random Oversampling
* Random Undersampling
* SMOTE (Synthetic Minority Over-sampling Technique)
* Tomek Links

Each technique was evaluated using:

| Technique | Precision | Recall | F1-score | Training Time |
| --------- | --------- | ------ | -------- | ------------- |

---

### 4. Ensemble Models

Different ensemble learning algorithms were trained and compared:

* Random Forest
* Gradient Boosting
* XGBoost
* Stacking Classifier

These models were evaluated using Precision, Recall, F1-score, and Training Time.

---

### 5. Model Visualization

Two important visualizations were used to analyze model performance:

Confusion Matrix
Shows how well the model distinguishes between normal and fraudulent transactions.

Feature Importance
Displays the most influential features contributing to fraud detection.

---

## Key Findings

* Handling class imbalance significantly improved fraud detection performance.
* Sampling techniques such as SMOTE improved recall for the minority class.
* Ensemble models outperformed the baseline Logistic Regression model.
* XGBoost achieved the best balance between precision, recall, and training time.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Imbalanced-learn
* Matplotlib
* Seaborn

---

## How to Run the Project

1. Download the dataset from Kaggle.
2. Place the dataset file `creditcard.csv` in the project directory.
3. Open the notebook in Google Colab or Jupyter Notebook.
4. Run the cells sequentially.

---

## Author

Nada Ragab
Faculty of Computers and Artificial Intelligence
AI Department
