# Module 12 Report Template

## Overview of the Analysis

This project aims to build supervised machine learning models to predict loan credit risk. The data (lending_data.csv) provides data on loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, and loan status. "Loan status" is designated by ‘0’ (low risk) and ‘1’ (high risk); this is what is being predicted. LogosticRegression and RandomOverSampler were used to create these models.

## Results

* Machine Learning Model 1: LogisticRegression method
    * Classification report indicates 0.99 accuracy, precision 1.0, and 0.99 recall. Balanced accuracy was 0.95.
 
* Machine Learning Model 2: LogosticRegression model applied after using RandomOverSampler to balance the data.
    * Classification report indicates 0.99 accuracy, precision 1.0, and 0.99 recall. Balanced accuracy was 0.95.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
   * Classification reports were identical, both indicated values from 0.99 to 1.0. Both are excellent performers but this data alone cannot be used to determine which one is best. 
  
* Does performance depend on the problem we are trying to solve? Yes. The models did show differences when looking at the matrices of confusion, which could be used to determine which model works "best." Model 1 was less prone to return false negative than Model 2 which was prone to returning false positive results. To determine what is best would depend on the end user's risk tolerance of denying qualified loans or extending risky loans.
