# Bank Marketing Campaign Classification: Comparing Machine Learning Models

## Project Overview

This project applies multiple machine learning classification algorithms to predict whether a customer will subscribe to a term deposit based on information collected during a bank marketing campaign. The primary objective is to compare the performance of several classification models and identify the most effective approach for customer subscription prediction.

## Business Problem

Banks invest significant resources in marketing campaigns. Identifying customers who are most likely to subscribe to a term deposit can improve campaign effectiveness, reduce marketing costs, and increase conversion rates.

The goal of this project is to build predictive models that help banks target potential customers more efficiently.

## Research Question

Which classification model provides the best performance for predicting customer term deposit subscriptions when comparing:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Decision Tree
* Support Vector Machine (SVM)

## Dataset

**Source:** UCI Bank Marketing Dataset

Dataset contains information related to direct marketing campaigns conducted by a Portuguese banking institution.

Target Variable:

* y = yes (customer subscribed)
* y = no (customer did not subscribe)

Features include:

* Age
* Job
* Marital Status
* Education
* Housing Loan
* Personal Loan
* Contact Type
* Campaign Information
* Economic Indicators

## Project Workflow

### 1. Business Understanding

Define the business objective and success criteria.

### 2. Data Understanding

* Explore dataset structure
* Analyze feature distributions
* Identify missing values and class imbalance

### 3. Data Preparation

* Encode categorical variables using OneHotEncoder
* Scale numerical variables using StandardScaler
* Create train/test datasets
* Prepare target variable for classification

### 4. Baseline Model

Establish a baseline by predicting the majority class.

### 5. Model Development

The following models were implemented:

#### Logistic Regression

Advantages:

* Fast training
* Highly interpretable
* Strong baseline classifier

#### K-Nearest Neighbors (KNN)

Advantages:

* Simple implementation
* Captures nonlinear relationships

#### Decision Tree

Advantages:

* Easy to interpret
* Handles nonlinear relationships

#### Support Vector Machine (SVM)

Advantages:

* Effective in high-dimensional spaces
* Strong predictive performance

### 6. Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

Training time was also measured and compared.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Model Comparison

| Model               | Train Time                | Train Accuracy | Test Accuracy |
| ------------------- | ------------------------- | -------------- | ------------- |
| Logistic Regression | Measured During Execution | Calculated     | Calculated    |
| KNN                 | Measured During Execution | Calculated     | Calculated    |
| Decision Tree       | Measured During Execution | Calculated     | Calculated    |
| SVM                 | Measured During Execution | Calculated     | Calculated    |

## Hyperparameter Tuning

GridSearchCV was used to optimize:

### Logistic Regression

* C
* Solver

### KNN

* n_neighbors
* weights
* p

### Decision Tree

* max_depth
* min_samples_split
* min_samples_leaf
* criterion

### SVM

* C
* kernel
* gamma

## Key Findings

* Logistic Regression provided strong performance with excellent interpretability.
* Decision Trees were easy to explain but showed signs of overfitting.
* KNN performed reasonably well but was sensitive to parameter selection.
* SVM achieved competitive predictive performance but required longer training times.
* Hyperparameter tuning improved model performance across all classifiers.

## Business Recommendations

Based on model performance and interpretability, Logistic Regression is recommended as a strong candidate for deployment. The model can help marketing teams:

* Identify customers likely to subscribe
* Improve campaign targeting
* Reduce marketing costs
* Increase conversion rates

## Repository Structure

```text
├── data/
│   └── bank-additional-full.csv
├── notebooks/
│   └── Bank_Marketing_Classification.ipynb
├── images/
│   └── model_comparison.png
├── README.md
└── requirements.txt
```

## How to Run

1. Clone the repository

```bash
git clone https://github.com/yourusername/bank-marketing-classification.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook

```bash
jupyter notebook
```

4. Open the notebook and run all cells.

## Future Improvements

* Ensemble methods (Random Forest, XGBoost)
* Feature selection techniques
* SMOTE for handling class imbalance
* Automated hyperparameter optimization using Bayesian Optimization

## Author

Rahul Rusia

Capstone Project – Machine Learning Classification Model Comparison
