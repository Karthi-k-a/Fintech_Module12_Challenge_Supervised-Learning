# Fintech Module 12 Challenge - Supervised Learning
## Credit Risk Classification
![](https://github.com/Karthi-k-a/Karthi-k-a-Fintech_Module12_Challenge_Supervised-Learning/blob/main/Images/12-homework-image.png)
### Overview of the Analysis
It is very important for lending companies to thoroughly check the creditworthiness of customers before extending credit to protect their businesses from late payment or nonpayment. This project aims at analysing a dataset of historical lending activity from a peer-to-peer lending services company to build a machine learning model that can predict the creditworthiness of borrowers. The following steps were performed in [credit_risk_resampling](https://github.com/Karthi-k-a/Karthi-k-a-Fintech_Module12_Challenge_Supervised-Learning/blob/main/credit_risk_resampling.ipynb) file to build a LogisticRegression model with various sampling methods- 
- Split the Data into Training and Testing Sets
- Create a Logistic Regression Model with the Original Data
- Predict a Logistic Regression Model with Resampled Training Data
- Write a Credit Risk Analysis Report

### Results
- Machine Learning Model 1: Logistic Regression Model with the Original Data

- Machine Learning Model 2: Logistic Regression Model with Resampled Training Data

Description of Model 1 and 2 Accuracy, Precision, and Recall scores.

### Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

- Which one seems to perform best? How do you know it performs best?
- Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the 1's, or predict the 0's? )

If you do not recommend any of the models, please justify your reasoning.

A lending company might want a model that requires a higher recall because:

healthy loans being identified as a non-healthy loan might be more costly for a lending company since it might cause the loss of customers but it would not be as big of a deal since they have not provided any funds to the customer indicating no loss in terms of money

non-healthy loans being identified as a healthy loan might surely be more costly for a lending company due to the loss of funds being provided by the lender
