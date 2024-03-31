## Overview of the Analysis

This analysis aims to predict if an individual's level of loan risk is either healthy or high risk. This helps companies identify the level of risk when issuing loans to applicants to accept or deny an individual. In the data set, we looked at the loan_size, interest_rate   borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt and loan_status of a historical data set to train the modal on predicting the loan status of an individual. 

To train the modal, I first created the Y and X labels where Y was Loan Status, and X was the remaining columns in the data frame after dropping loan status. Next, I proceed by splitting the data set into a testing and training data set so we can train the model on the training data set and then test out how our modal works and its accuracy with the testing data set that the modal has not been trained with to replicate how it would perform in the real world. After the data set is split, a logistical regression modal is used to train and fit the data and make test predictions using the modal. Lastly, to evaluate the performance, I created a classification report to see the accuracy, precision and recall of the model. 
 

## Results

                precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

*Precision = is the ratio of correctly predicted positive observations to the total predicted positive observations. In the model, the precision for Healthy loans is 1, which is very good, and the precision for high-risk loans is 0.85, which is still okay and not bad.

*Accuracy = is how often the model is correct—the ratio of correctly predicted observations to the total number of observations. In the modal, the accuracy is 99, which is very good.

*Recall = is the ratio of correctly predicted positive observations to all predicted observations for that class. Recall numbers for both healthy and high-risk individuals are 0.99 and 0.91, which is relatively good.


## Summary

In summary, the modal is very good and has high accuracy scores, which suggests it can be used by the business to pre-qualify and determine if the individual is healthy or high risk. Since the precision of predicting healthy loan individuals is 1, it will help ensure that it ensures that the company is lending to only healthy financial individuals to reduce the risk of applicants defaulting on loans.