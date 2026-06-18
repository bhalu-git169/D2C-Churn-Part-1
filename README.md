# Part 1: Data Audit, EDA & Business Understanding

## Project Overview
This repository contains Part 1 of the D2C Customer Churn Intelligence Capstone. The objective is to understand the business problem, audit raw data for quality/leakage risks, perform exploratory data analysis, and formulate data-backed churn hypotheses before modeling.

## Repository Contents
* `eda_audit.ipynb`: The primary Jupyter Notebook containing data loading, automated data quality checks, merges, and 6 exploratory visualizations.
* `data_quality_report.md`: A summary of missing values, duplicates, and strict leakage prevention rules.
* `business_memo.md`: A business-facing summary outlining 5 core churn-risk hypotheses and retention strategy recommendations.
* `requirements.txt`: Required Python dependencies.

## Instructions to Run
1. Ensure you have Python installed.
2. Clone this repository to your local machine.
3. Install dependencies by running: `pip install -r requirements.txt`
4. Place the raw dataset CSVs (`customers.csv`, `orders.csv`, `support_tickets.csv`, `web_events_snapshot.csv`, `churn_labels.csv`) in the same directory.
5. Open `eda_audit.ipynb` in Jupyter Notebook or Jupyter Lab.
6. Click **Kernel -> Restart & Run All** to execute the data audit and generate all charts sequentially.
