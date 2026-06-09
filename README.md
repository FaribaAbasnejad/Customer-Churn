# Customer-Churn

### 1.Business Understanding

Objective: Predict customer churn for a telecom company to improve customer retention and revenue.
Goal: Identify at-risk customers using historical usage, complaints, subscription, and demographic data.
Impact: Reducing churn could improve revenue and customer loyalty.
Notes: Clear problem definition and business relevance. Good job linking churn to potential business outcomes.


### 2.Data Understanding

Dataset: Customer Churn.csv with 3,150 rows and 14 columns.

Target Variable: Churn (0 = no churn, 1 = churn)

Data Types: Mostly numeric; no missing values.


### 3.Data Preparation

Splitting: 70% train / 30% test, stratified by churn.

Features: 13 numeric features, no explicit categorical features in this case.

Preprocessing:

StandardScaler for numeric features.

OneHotEncoder for categorical features (none in dataset, so this is effectively skipped).


### 4.Modeling

Observations:

XGBoost outperforms others in all metrics, particularly ROC-AUC.

SVM shows high recall but low precision (likely overpredicts churn).

Random Forest is close to XGBoost but slightly lower in ROC-AUC.


### 5.Evaluation


### 6.Deployment
