# **Module 12: Credit Risk Classification**

## Overview of the Analysis


Credit risk poses a classification problem that’s inherently imbalanced. This is because healthy loans easily outnumber risky loans. 

This analysis allows us to understand if our model can efficiently identify the loans whether it is a healthy one or risky one. 

Our labeled original data included the loan size, interest rate, borrower's income, debt-to-income, number of their accounts, any derogatory marks and total debt they have, which ultimately is used to predict whether their loan status -- whether a healthy loan or a high risk loan.

One of the variables that our analysis is predicting is our `value_counts` which describes our data that are healthy loans are 75036, while 2500 are high risk loans. We also use a `confusion_matrix` to determine the performance of the classification model used in the analysis for both the original data and the oversampled data.

The stages of the machine learning process starts at picking which type of model to be used. In this analysis, we rely on Logistic Regression and RandomOverSampler. Then, we would then fit the model with our original X data, and predict the model. These steps are repeated for after a RandomOverSampler is created and Logistic Regression is called and fitted again with the resampled data.

------

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1: Logistic Regression with the original labeled data

  * Balance Accuracy Score: 95%
  * Precision (minority): 85%
  * Recall scores (minority): 91%


* Machine Learning Model 2: Logistic Regression with the use of a Random Oversampled Data

  * Balance Accuracy Score: 99.4%
  * Precision (minority): 84%
  * Recall scores (for both majority and minority data): 99%

## Summary

After creating an oversampled data, our model performed better. We know that it performs better because just basing it off the balance accuracy score we have 95% (orginal data) vs 99% (resampled data), and even our classification matrix shows that it has improved the loan analysis model. 

The performance of the analysis does depend on the problem, predicting which are healthy loans or risky loans should be correctly predicted since the model result itself will be use as basis for the machine to learn how to classify these loans properly. Overall, the Logistic regression model is recommended to create a machine learning that'll classify the loans in the data.
