# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis was to help the bank classify future borrowers as risky applicants or worthy of loan. Available data on loan amount, interest rate, income, debt to income ratio, number of accounts held with the bank, number of derogatory remarks, total amount of debt and whether on not they defaulted on the loan in question were leveraged from 77,537 bank customers. Of those customers, the majority (75,036) were were in good standing. This is to be expected, as those with low credit scores may be less likely to apply and therefore approved for a loan. However, this imbalance in information available to pedict default loan status poses a risk of bias in the analysis.  Therefore, in addition to logistic regression using the data set, an oversampling excercise was also completed. 

The first step was to preview the dataset (lending_data.csv) to determine what data is available. Next, two new dataframes (x and y) are created from the initial file.  One dataframe (y) included a single target variable that we'd like to predict, loan status.  The other dataframe (x) contained all variables except loan status. Next we checked the distribution of classifications (healthy versus default loan status) in the target dataframe. This step checks for balance in the categorical target we are trying to predict.  Next we split both dataframes into a test and a train dataframe. Generally speaking, the train set contains 75% of the data.  Next, since we are prediciting categorical data, we fit the training data to a logisitic model.  Then we try to make a prediction of loan status based on the X test data. The performance of the prediction was then evaluated using an accuracy score, confusion matrix, and a classification report was produced.  The same steps were repeated for resampled data.         

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

/content/saved_model.pb

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


