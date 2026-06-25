# Bagner-s_portafolio

# [Project 1: Review of Fraud database table with SQL](https://github.com/bagnerrobleto-dot/SQL-Fraud-database-Queries/blob/main/Fraud%20Analysis%20Queries.sql)

## This repository contains SQL scripts designed to explore and prepare transactional data for fraud investigation. The analysis pipeline includes:

* Data Quality & Discovery: Performed initial sanity checks and explored distributions of fraud rates across different transaction channels and merchant categories.

* Risk Profiling: Categorized merchants and transactions using behavioral indicators (geo-anomalies and velocity scores) and aggregated metrics (chargeback volumes).

* Feature Engineering: Combined transactional, customer, and merchant data to create a high-fidelity dataset, including derived features like transaction timing, risk scores, and historical spending patterns.

* Dataset Preparation: Finalized an "export-ready" view, effectively joining relational tables to provide a comprehensive, flattened feature set suitable for input into a Python-based machine learning pipeline.

## Technical Highlights

* SQL Techniques: Utilized Common Table Expressions (CTEs), CASE statements for risk classification, window functions for aggregation, and complex JOIN logic.
