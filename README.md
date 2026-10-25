# Banking Customer Churn Analysis

## Project Overview

This project analyzes customer churn patterns using exploratory data analysis (EDA), statistical hypothesis testing, and machine learning.

The objective is to identify customer segments associated with higher churn rates and evaluate a baseline classification model that could support data-driven customer retention strategies.

## Business Questions

1. Which customer characteristics are associated with higher churn rates?
2. Are there statistically significant associations between selected customer attributes and churn?
3. How well can Logistic Regression identify customers who are likely to churn?
4. How does changing the classification threshold affect churn detection?

## Dataset

The dataset contains 10,000 customer records and 18 columns, including demographic information, account characteristics, banking product usage, and churn status.

The target variable is `Exited`:

- `0`: Customer stayed.
- `1`: Customer exited.

**Dataset source:** To be added after verifying the original source and applicable usage terms.

## Tools and Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- SciPy
- Scikit-learn
- Jupyter Notebook

## Methodology

1. Data loading and quality checks
2. Exploratory data analysis
3. Churn rate analysis across customer segments
4. Chi-Square tests of independence
5. Logistic Regression classification
6. Model evaluation using accuracy, precision, recall, F1-score, and ROC-AUC
7. Classification threshold comparison

## Key Findings

- Inactive customers had a churn rate of **26.87%**, compared with **14.27%** among active customers.
- Germany had the highest churn rate at **32.44%**, compared with **16.17%** in France and **16.67%** in Spain.
- Customers aged 46–55 had the highest churn rate at **50.57%**.
- The baseline Logistic Regression model achieved **81.30% accuracy** and a **0.7783 ROC-AUC**.
- At a classification threshold of 0.3, churn recall increased to **52.70%**, with an F1-score of **0.5065**.

## Business Recommendations

- Investigate engagement patterns among inactive customers.
- Explore potential reasons for the higher churn rate in Germany.
- Investigate the needs and experiences of customers aged 46–55.
- Evaluate classification thresholds based on the trade-off between missed churn cases and unnecessary retention outreach.

These recommendations are exploratory and should be validated with additional business context.

## Limitations

- Findings describe associations and do not establish causation.
- The model is a baseline and has not been comprehensively compared with alternative models.
- Threshold selection requires validation on separate validation data before final test evaluation.
- Predictor variables should be checked for potential data leakage.
- The dataset's original source and usage terms must be verified before public redistribution.

## Future Work

- Compare Logistic Regression with alternative classification models.
- Investigate feature importance and model interpretability.
- Validate threshold selection using separate validation data.
- Estimate the potential business impact of retention strategies.
