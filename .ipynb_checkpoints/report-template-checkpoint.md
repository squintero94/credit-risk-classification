# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
      The purpose of this analysis is to identify the creditworthiness of borrowers.
* Explain what financial information the data was on, and what you needed to predict.
      The data contained the following financial information: loan_size	interest_rate	borrower_income	debt_to_income	num_of_accounts	derogatory_marks	total_debt. With this info, I needed to predict loan_status. 
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
      I was predicting whether the loan_status was a healthy-risk loan `0` or a high-risk loan `1`.
* Describe the stages of the machine learning process you went through as part of this analysis.
      First, separating loan_status from the other features by assinging them to variables `y` and `X`. Then I could split the data using train_test_split. Using these newly created, I built the `LogisticRegression` model to create predictions. Lastly, these predictions were evaluated using a confusion matrix and a classification report.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
      With the `LogisticRegression` model, I had to train, fit, predict.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
      Accuracy: 19226 / 19384 = 0.9918
      Precision: 18663 / 18765 = 0.9946
      Recall: 18663 / 18719 = 0.9970

* Machine Learning Model 2:
    * Description of Model 2 Accuracy, Precision, and Recall scores.
      Accuracy: 0.99
      Precision: weighted avg = 0.99
      Recall: weighted avg = 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
      Both perform very well. As both have 99% across the board for accuracy, precision, and recall, I can't say that one performs better than the other. 
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
      Since the purpose of this analysis is to identify the creditworthiness of borrowers, it would be more important to predict the `1`'s (high-risk). This model has a an f1-score of 0.88 for the `1`'s and an f1-score of 1.00 for the `0`'s. While 0.88 is a rather high mark, I would imagine that the financial instution using this would want a bit more certainty in predicting a high-risk loan.
  

