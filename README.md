# Credit_Risk_Analysis
Module 17

# Project Overview
Fast Lending wants to use machine learning to determine credit risk of customers applying for loans. To accomplish this, we'll use various machine learning models and techniques to determine what practices would be best for Fast Lending. 

# Results

The dataset we are given contains 115,675 loan applications from Q1 of 2019. Using loan_status as our target, we were able to determine the risk of an account as low or high. All accounts that were current with their loan status was considered low risk, while all others were considered high risk. 
<img src="<link>" width="300">



### Naive Random Oversampling
<img src="<link>" width="600">
 - Balanced accuracy score: 0.6484905987244723
 - Precision is low for high-risk and high for low-risk
 - Recall Scores
    - High: 0.63
    - Low: 0.66

### SMOTE Oversampling
<img src="<link>" width="600">
 - Balanced accuracy score: 0.623523937295285
 - Precision is low for high-risk loans and high for low-risk loans
 - Recall Scores
    - High: 62
    - Low: 63

### Undersampling
<img src="<link>" width="600">
 - Balanced accuracy score: 0.5207293391509643
 - Precision is low for high-risk loans and high for low-risk loans
 - Recall Scores
    - High: 0.59
    - Low: 0.46

### Combination Under-Over Sampling
<img src="<link>" width="600">
 - Balanced accuracy score: 0.6398024261616125
 - Precision is low for high-risk loans and high for low-risk loans
 - Recall Scores
    - High: 0.70
    - Low: 0.58

### Balanced Random Forest Classifier
<img src="<link>" width="600">
 - Balanced accuracy score: 0.7959971556458013
 - Precision is low for high-risk loans and high for low-risk loans
 - Recall Scores
    - High: 0.68
    - Low: 0.91

### Easy Ensemble AdaBoost Classifier
<img src="<link>" width="600">
 - Balanced accuracy score: 0.9252521040566293
 - Precision is low for high-risk loans and high for low-risk loans
 - Recall Scores
    - High: 0.91
    - Low: 0.94

# Summary
All models showed low precision for high-risk loans and high precision for low-risk loans. This could be attributed to how narrow our scope for low-risk loans are (if the loan is current) versus how we determine high risk (Late (31-120 days), Late (16-30 days), Default, In Grace Period). With the results generated thus far I would recommend proceeding with the Easy Ensemble AdaBoost Classifier as it provides a high balanced accuracy score and high recall scores. 
