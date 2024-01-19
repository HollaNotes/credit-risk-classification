# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
  * The purpose of this analysis is to evaluate the performance of 2 different machine learning models that have been trained to predict loan outcomes and predict the accuracy, precision, and recall of each model.
* Explain what financial information the data was on, and what you needed to predict.
  * The data shows the size of historic loans, the interest rate, borrower rate, debt to income, number of derogatory marks, total debt, and loan status. The status of the loan is the variable we are predicting based on other factors from similar loans. We are trying to predict Healthy Loans(0) vs High Risk Loans(1).
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
  * Value Counts for Healthy Loans(0): 75036
  * Value Counts for High Risk Loans(1): 2500
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
  * The stages I went though as part of the machine learning process were:
    * Importing dependencies
    * Loading in the data
    * Separating out y (the "loan_status" column) from the rest of the data
    * Splitting the data into training and testing datasets
    * Fitting and modeling a logistic regression model by using the training dataset
    * Saving predictions based on the testing data
    * Generating a confusion matrix
    * Creating a classification report to see the accuracy, precision, and recall of the model (Model 1)
    * Resampling the data using RandomOverSampler
    * Fitting and predicting with the resampled data
    * Generating a confusion matrix on resampled data
    * Creating a classification report on the resampled data to see the accuracy, precision, and recall of the model (Model 2)


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    * Accuracy: 99%
    * Precision (Healthy Loans (0)): 100%
    * Precision (High Risk Loans (1)): 85%
    * Recall (Healthy Loans (0)): 99%
    * Recall (High Risk Loans (1)): 91%


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    * Accuracy: 99%
    * Precision (Healthy Loans (0)): 99%
    * Precision (High Risk Loans (1)): 99%
    * Recall (Healthy Loans (0)): 99%
    * Recall (High Risk Loans (1)): 99%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best? 
  * The second model seems to perform best due to the consistency of results against all metrics.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? ) 
  * I think this would be dependent on what the business is looking for. I would imagine that a business would like to predict if a loan is high risk as well as predict if a loan would be a healthy loan. I imagine that having the ability to predict a high risk loan would be more important for a business however, because high risk loans are not as good for business. Either way, I would say the second model would be the best model to use. 

If you do not recommend any of the models, please justify your reasoning.
