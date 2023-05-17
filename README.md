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
- **Machine Learning Model 1: Logistic Regression Model with the Original Data**<br>
This model predicts the creditworthiness of borrowers using the original data and has the following characteristics-<br>

![](https://github.com/Karthi-k-a/Karthi-k-a-Fintech_Module12_Challenge_Supervised-Learning/blob/main/Images/1.png)<br>

![](https://github.com/Karthi-k-a/Karthi-k-a-Fintech_Module12_Challenge_Supervised-Learning/blob/main/Images/2.png)

- **Machine Learning Model 2: Logistic Regression Model with Resampled Training Data**<br>
This model predicts the creditworthiness of borrowers using resampled training data and has the following characteristics-<br>

![](https://github.com/Karthi-k-a/Karthi-k-a-Fintech_Module12_Challenge_Supervised-Learning/blob/main/Images/3.png)<br>

![](https://github.com/Karthi-k-a/Karthi-k-a-Fintech_Module12_Challenge_Supervised-Learning/blob/main/Images/4.png)

### Summary
The model with original data performs well as per the balanced accuracy score (95%). Also, the imbalanced classification report shows that the model predicted healthy loans (0) 100% of the time and non-healthy loans (1) 85% of the time. However, these results can be misleading bacause the dataset is imbalanced- the number of healthy loans (low-risk) highly outweigh the number of non-healthy loans (high-risk) indicating that the model would predict loan status as healthy better than predicting it as non-healthy. Therefore, it is important to predict the model with resampled data.

The oversampled model generated a balanced accuracy score of 99% which is higher than the model with original (imbalanced) data. With the recall score for non-healthy loans (1) increasing from 0.91 in imbalanced model to 0.99 in oversampled model, we can see that the oversampled model performs better in terms of measuring the count of true positives for non-healthy loans.

I recommend Machine Learning Model 2 (Logistic Regression with Resampled Training Data). A lending company will require a model that has a higher recall because non-healthy loans being identified as healthy loans might be more expensive for the company causing loss of money. 
