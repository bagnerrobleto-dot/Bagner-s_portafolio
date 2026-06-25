# Bagner-s_portafolio

# [Project 1: Review of Fraud database table with SQL](https://github.com/bagnerrobleto-dot/SQL-Fraud-database-Queries/blob/main/Fraud%20Analysis%20Queries.sql)

## This repository contains SQL scripts designed to explore and prepare transactional data for fraud investigation. The analysis pipeline includes:

* Data Quality & Discovery: Performed initial sanity checks and explored distributions of fraud rates across different transaction channels and merchant categories.

* Risk Profiling: Categorized merchants and transactions using behavioral indicators (geo-anomalies and velocity scores) and aggregated metrics (chargeback volumes).

* Feature Engineering: Combined transactional, customer, and merchant data to create a high-fidelity dataset, including derived features like transaction timing, risk scores, and historical spending patterns.

* Dataset Preparation: Finalized an "export-ready" view, effectively joining relational tables to provide a comprehensive, flattened feature set suitable for input into a Python-based machine learning pipeline.

## Technical Highlights

* SQL Techniques: Utilized Common Table Expressions (CTEs), CASE statements for risk classification, window functions for aggregation, and complex JOIN logic.

## Overview of the Database  	![](Images/Picture%2.png)
## Final query ready to work on Python  	![](Images/Picture%1.png)

# [Project 2: Fraud Detection Modeling (Python)](https://github.com/bagnerrobleto-dot/Python-Exploratory-Analysis/blob/main/Fraud_Trx%20Data%20Analysis.ipynb)

## This notebook processes the flattened dataset exported from your SQL pipeline. It focuses on understanding the data distribution and preparing the features for predictive modeling. The workflow includes:

* Exploratory Data Analysis (EDA): Performed high-level data profiling, including shape validation, missing value identification, and class imbalance assessment (fraud vs. non-fraud).

* Data Cleaning & Imputation: Addressed data sparsity by replacing missing values in risk scores (device and IP) with median values, ensuring a robust input set.

* Feature Engineering: Created informative "missingness flags" (e.g., cvv_missing) to capture potential patterns where incomplete transaction details correlate with fraudulent activity.

* Multicollinearity Mitigation: Used a correlation matrix heatmap to identify highly redundant features (e.g., overlapping amount formats and temporal frequency counts) and dropped them to ensure model interpretability and better performance.

## Technical Highlights

* Library Ecosystem: Leveraged pandas for manipulation, seaborn/matplotlib for visual correlation analysis, and scikit-learn for pre-processing.

* Feature Optimization: Streamlined the feature space by removing highly collinear variables, reducing noise
