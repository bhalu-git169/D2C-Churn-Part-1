# Data Quality Report

## 1. Overview
This report summarizes the data quality issues discovered during the initial audit of the raw D2C datasets. Understanding these issues early ensures we prevent errors and data leakage during the modeling phase.

## 2. Missing Values & Duplicates
Based on the automated scan of the raw data, here are the findings:

* **Customers Dataset:** 2,400 rows. 0 duplicates. High volume of missing values in `loyalty_tier` (1,386 missing, 57.75%) and `skin_type` (401 missing, 16.71%).
* **Orders Dataset:** 10,009 rows. 0 duplicates. Minor missing values in `rating` (80 missing, 0.8%).
* **Support Tickets Dataset:** 1,921 rows. 0 duplicates. 0 missing values.
* **Web/App Events Dataset:** 2,400 rows. 0 duplicates. 0 missing values.

## 3. Invalid Values, Outliers & Date Consistency
* *Note: Continuous monitoring for outliers (e.g., unusually high order values or negative ages) will be conducted during feature engineering.*

## 4. Join / Key Issues
* *Note: All primary tables will be joined via `customer_id`. Any orphaned records will be flagged during the merging process.*

## 5. Potential Leakage Risks
* **Warning:** To prevent data leakage, no data generated after the customer snapshot date will be used. Any columns revealing post-snapshot interventions or the actual churn event will be strictly excluded from model input features.