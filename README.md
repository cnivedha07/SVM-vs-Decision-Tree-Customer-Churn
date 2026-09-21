# SVM vs Decision Tree — Customer Churn Prediction

A machine learning classification project that compares **Support Vector Machine (SVM)** and **Decision Tree** models for predicting customer churn.

The project focuses on understanding how two different classification algorithms perform on the same customer churn dataset using multiple evaluation metrics.

---

## Project Overview

Customer churn prediction is a common machine learning problem where the objective is to identify customers who are likely to leave a service.

In this project, two classification algorithms are implemented and compared:

- **Support Vector Machine (SVM)**
- **Decision Tree Classifier**

Both models are trained on the same dataset and evaluated using:

- Accuracy
- Precision
- Recall
- ROC-AUC

The project also demonstrates how to make a churn prediction for a new customer.

---

## Objectives

The main objectives of this project are to:

1. Understand the customer churn dataset.
2. Perform basic data preprocessing.
3. Encode categorical variables.
4. Split the data into training and testing sets.
5. Train an SVM classifier.
6. Train a Decision Tree classifier.
7. Compare both models using multiple evaluation metrics.
8. Understand the difference between the two classification approaches.
9. Use the trained models to predict churn for a new customer.

---

## Dataset

The project uses a customer churn dataset containing information about customers and their service usage.

### Features Used

| Feature | Description |
|---|---|
| `monthly_charges` | Monthly amount charged to the customer |
| `tenure_months` | Number of months the customer has been with the service |
| `contract_type` | Type of contract held by the customer |
| `support_calls` | Number of support calls made by the customer |

### Target

The target variable represents whether the customer churned:

| Value | Meaning |
|---|---|
| `Yes` | Customer churned |
| `No` | Customer did not churn |

---

## Machine Learning Models

### 1. Support Vector Machine

SVM is a supervised classification algorithm that attempts to find an optimal decision boundary separating different classes.

The model is particularly useful for understanding:

- Decision boundaries
- Margin maximization
- Classification in feature space
- Kernel-based classification

---

### 2. Decision Tree

Decision Tree is a tree-based classification algorithm that recursively splits the data based on feature conditions.

It provides an interpretable structure where predictions can be followed through a sequence of decisions.

The project uses the Decision Tree as a contrasting model to SVM because the two algorithms approach classification differently.

---

## Project Workflow

```text
Customer Churn Dataset
        ↓
Data Loading
        ↓
Data Inspection
        ↓
Data Preprocessing
        ↓
Categorical Feature Encoding
        ↓
Feature / Target Separation
        ↓
Train-Test Split
        ↓
   ┌───────────────┐
   ↓               ↓
  SVM       Decision Tree
   ↓               ↓
   └───────┬───────┘
           ↓
     Model Evaluation
           ↓
 Accuracy / Precision
 Recall / ROC-AUC
           ↓
   Model Comparison
           ↓
 New Customer Prediction
