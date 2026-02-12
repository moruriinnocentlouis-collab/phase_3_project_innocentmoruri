# SyriaTel Customer Churn Prediction

## Overview
This project aims to reduce revenue loss for SyriaTel by predicting which customers are likely to cancel their service (churn). By identifying at-risk customers, the retention team can proactively offer incentives to keep them.

## Business Problem
It is significantly more expensive to acquire a new customer than to retain an existing one. SyriaTel is facing a churn problem that impacts long-term profitability. This project provides a predictive classification model to identify churn drivers and at-risk individuals.

## Data
The dataset contains customer information including usage patterns (day, evening, night), account details, and service interactions.
- **Source:** SyriaTel Dataset (provided for Phase 3 Project).
- **Target Variable:** `churn` (True/False).

## Methods
- **Preprocessing:** Used `ColumnTransformer` for Scaling and One-Hot Encoding.
- **Models:** Compared a **Logistic Regression** baseline against a **Decision Tree Classifier**.
- **Metrics:** Prioritized **Recall** and **F1-Score** to ensure we catch as many churners as possible while maintaining model reliability.

## Key Insights
- **Top Predictor:** `Total Day Charge` (High-value customers are most sensitive to pricing).
- **Service Threshold:** Customers with 3+ service calls show a significantly higher probability of leaving.

## Final Model Performance
The **Decision Tree** achieved a **Recall of 74.3%**, allowing SyriaTel to identify the majority of potential churners before they leave.

## Repository Structure
- `phase_3_project.ipynb`: The complete technical analysis.
- `presentation.pdf`: Non-technical stakeholder slides.
- `data/`: Folder containing the SyriaTel dataset.
