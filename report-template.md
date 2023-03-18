# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Logistic Regression Model(Training): 
* OVERALL ACCURACY : .952
  * (Healthy)
  * Precision : 1
  * recall : .99
  * (At-Risk)
  * Precision : .85
  * Recall : .91


* Logistic Regression Model(Resampled):
* OVERALL ACCURACY : .994
  * (Healthy)
  * Precision : 1
  * Recall : .99
  * (At-Risk)
  * Precision : .84
  * Recall : .99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Two logistic regression models were used in this challenge. Although both models performed very well, the Resampled LRM seems to perform best. with an overall accuracy of 99.4%. the Training LRM has an overall accuracy of 95.2%. Between both models, it's clear that they should be used to predict `0`'s and not `1`'s. Until either model's precision for at-risk loans increases, the bank will always be more confident in predicting healthy loans. As stated above, I recommend that the bank use the Logistic Regression Model with resampled training data rather tham the Logistic Training Model with original data due to the difference in overall accuracy (99.4% as opposed to 95.2%).