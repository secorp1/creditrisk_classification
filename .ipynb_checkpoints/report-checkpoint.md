# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
  The goal is to determine if logistic regression model can be accurate to predict healthy loans vs. high risk loans using original data resampled data to increase the size of the minority class.
  
* Explain what financial information the data was on, and what you needed to predict.
  
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
  original-
  0: 75036
  1: 2500
  oversample-
  0: 56271
  1: 56271
  
* Describe the stages of the machine learning process you went through as part of this analysis.
  1. Prepare data
  2. Separate data to feature such as columns which X and Y is the outcome or labels
  3. train_test_split
  4. Pick ML model for classification for logisticregression
  5. Fit the model with training data
  6. Use the model to make predictions with the test data for default test data can be evaluated
  7. Evaluate the predictions camparing metrics, confusion matrix and classification report
     
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
  SKLearn LogisticRegression
  train_test_split
  confusion_matrix
  classification_report

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
Accuracy: 0.99
Precision: Class 0: 1.00 Class 1: 0.85
Recall scores: Class 0: 0.00 Class 1 0.91
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
  Overall Logistic Regression model performed well due to prediction of the outcome 0 healthly loans for class 0, both precision and recall were very high.
  For class 1- high risk loans model precision is 0.84 and the recall of 0.91. The model is more often gives false positives than false negatives.
  
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
  The information appears that logistic regression models predicts both healthy and high risk loans provided in the training dataset.

If you do not recommend any of the models, please justify your reasoning.
The logistice regression model appears promising but would need to be evaluated against different datasets to confirm that it should be put into use for health status of loans.