# Customer Churn & Risk Analytics
## Overview
This project analyzes customer churn behavior using a real-world telecom dataset and develops a machine learning–based risk segmentation framework to support data-driven retention strategies.
## Business Problem
Customer churn directly impacts recurring revenue. Identifying customers at risk of churn and understanding the drivers behind churn enables targeted interventions rather than uniform retention efforts.
## Dataset
- Source: IBM Telco Customer Churn dataset
- Rows: 7,043 customers
- Features include customer tenure, service subscriptions, billing information, contract details, and demographics
## Approach
1. **Exploratory Data Analysis (EDA)**
   - Churn distribution and class imbalance
   - Churn vs tenure, contract type, pricing, and support services
2. **Feature Selection**
   - Removed identifiers, high-cardinality geographic variables, and leakage features
3. **Preprocessing Pipeline**
   - Missing value imputation
   - Scaling for numerical features
   - One-hot encoding for categorical features
4. **Modeling**
   - Logistic Regression (baseline)
   - Random Forest (final model)
   - Recall prioritized due to class imbalance
5. **Risk Segmentation**
   - Probability-based segmentation into Low, Medium, and High churn risk groups
   - Validation of segments against actual churn behavior
## Key Results
- Random Forest achieved ~80% recall for churned customers
- Month-to-month contracts, high monthly charges, low tenure, and lack of technical support were key churn drivers
- Risk segmentation enabled targeted retention strategies instead of blanket outreach
## Tools & Technologies
- Python (pandas, numpy, matplotlib, seaborn)
- scikit-learn (pipelines, preprocessing, models)
- Jupyter Notebook
- VS Code
## Business Impact
This framework enables organizations to proactively identify high-risk customers and design targeted retention actions, improving customer lifetime value and operational efficiency.
