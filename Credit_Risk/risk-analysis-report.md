# Module 12 Report Template

## Overview of the Analysis

I have created a logistic regression model to predict whether a home loan will be healthy or high-risk based on data about the loan and loanee:

* The variables taken into account are loan size, interest rate, borrower income, debt to income ratio, total debt, number of accounts, derogatory marks
* I used SciKit-Learn's train/test split module to separate the data, and its logistic regression function to create my model
* I then used the confusion matrix and classification report modules to evaluate my results

## Results

* The model proved incredibly accurate at predicting healthy loans without false positives or negatives, with a precision score of 100% and a recall score of 99%
* Because healthy loans make up nearly 97% of the dataset, the overall accuracy, precision, and recall scores of the model came in at 99%.
* The model is less adept at predicting high-risk loans, while still largely being successful. When looking only at the high-risk classification, precision is 85%, recall is 91%, accuracy is 88%.

## Summary

* This logistic regression model will be a powerful tool that allows us to save many work-hours in evaluating the risk levels of loans.
* With that said, we will get best results if we have humans to vet all loans flagged as high-risk, to ensure that those misclassified by the model are correctly identified.
* We may want to set up an appeal/review process within that department as well, as a further redundancy to ensure all borrowers are treated fairly.
* We should make sure this review department has all the resources they may need, as they will only be reviewing roughly 3% of our total loans. No matter how costly this department may seem, the savings vs evaluating all of these loans manually as we have in the past will be enormous.