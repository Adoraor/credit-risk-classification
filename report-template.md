# Report

## Overview of the Analysis

This analysis focused on building a predictive machine learning model to assess borrower creditworthiness based on historical data from a peer-to-peer lending service.The dataset encompassed vital financial attributes like loan size, interest rate, borrower income, and more. 

The objective of the analysis was to predict loan status, distinguishing between healthy (0) and high-risk loans (1). An initial exploration revealed the distribution of these labels. The analysis proceeded through stages:

    - Data Preprocessing: Data was loaded, explored, and cleaned to prepare it for modeling.

    - Data Splitting: The dataset was divided into training and testing sets for model evaluation.

    - Logistic Regression Models: Two logistic regression models were employed. One utilized the original data, while the other used oversampled data created with Random Over Sampler.

    - Model Evaulation : The performance of the logistic regression models was assessed to determine their effectiveness in predicting loan status.

This analysis was done with the LogisticRegression method which estimates the probability of a given sample belonging to a particular class. It was selected for this analysis due to its interpretability and suitability for binary classification tasks.


## Results

* Machine Learning Model 1:
        - Balanced Accuracy: 0.952
        - Precision for Label 0 (Healthy Loan): 1.00
        - Recall for Label 0 (Healthy Loan): 0.99
        - Precision for Label 1 (High-Risk Loan): 0.85
        - Recall for Label 1 (High-Risk Loan): 0.91

* Machine Learning Model 2:
        - Balanced Accuracy: 0.994
        - Precision for Label 0 (Healthy Loan): 1.00
        - Recall for Label 0 (Healthy Loan): 0.99
        - Precision for Label 1 (High-Risk Loan): 0.84
        - Recall for Label 1 (High-Risk Loan): 0.99


## Summary

Based on the evaluation results, both models perform exceptionally well. Model 2 demonstrates higher balanced accuracy and recall for Label 1, indicating its strong capability to correctly classify high-risk loans. However, Model 1 achieves a slightly higher precision for Label 1, suggesting it may be more conservative in predicting high-risk loans. The choice between Model 1 and Model 2 should be made based on the specific priorities and objectives of the company. If minimizing false positives for high-risk loans is a critical consideration, Model 1 may be favored. Otherwise, I would recommend Model 2 as it offers strong all-around performance.
