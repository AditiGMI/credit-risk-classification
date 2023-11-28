# Module 20 Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Purpose of the analysis: use various techniques to train and evaluate a model based on loan risk. I’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* The financial information the data was on "loan_status", a value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting and we need to see how well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels.
* I am using various variables to predict : like Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns, Split the data into training and testing datasets by using train_test_split, Split the data into training and testing datasets by using train_test_split,  & `value_counts`.
* Describe the stages of the machine learning process you went through as part of this analysis: model’s performance by doing the following:
generate a confusion matrix, print the classification report, how well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels
* I am using `LogisticRegression` & resampling method.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores:
  Predicted 0	Predicted 1
Actual 0	18663	102
Actual 1	56	563
Accuracy Score : 0.9918489475856377
Classification Report
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores: Predicted 0	Predicted 1
Actual 0	18649	116
Actual 1	4	615
Accuracy Score : 0.9918489475856377
Classification Report
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384


## Summary

Summary of the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* The acuracy of this model is very high at 99%, compared to other models in calculating both good & high risk loans. 

* It more important to predict the `1`'s, or predict the `0`'s
After observing the results, the accuracy seems to be good enought to start exploring this kind of algorithms in a bank, however, I would prefer to start running a pilot with new data to assess model's reliability.

