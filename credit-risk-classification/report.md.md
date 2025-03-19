# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of this analysis was to determine the accuracy of a logistic regression model when using original data with a class imbalance compared with a logistic regression model using resampled (oversampled minority class) data.
* Loan lending data including: loan size, interest rate, debt-to-income ratio, etc. was used to predict if a potential borrower would default on their loan.
* These models were used to predict loan status (high-risk vs healthy).
* For this analysis we created logistic regression models using separated training and test data. The models were fit to the training data and predictions were created. These predictions were evaluated against the test data to determine their accuracy, recall/sensitivity, precision, F1 score, and other metrics useful in evaluating the model's relevance.
* Logistic regression was used to model the target (loan status). This model was used with original lending data and then again with resampled data (oversampled minority class) to acheive a more appropriately trained model. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Accuracy= 0.95
  * Precision_healthy= 1.00 ; precision_high-risk= 0.84
  * Recall_healthy= 0.99 ; recall_high-risk= 0.94


* Machine Learning Model 2:
  * Accuracy= 0.99
  * Precision_healthy= 1.00 ; precision_high-risk= 0.84
  * Recall_healthy= 0.99 ; recall_high-risk= 0.99

## Summary


* Machine learning model 2, which used the resampled data, performed better. This improved performance is evidenced by a higher balanced accuracy score (higher rate of correct true positive and true negative predictions) and improved recall/sensitivity (fewer false negatives- ie high risk categorized as healthy). 
* Though the second model (resampled data) was unable to improve the precision for the high-risk (1) loan predictions, it performed better in the more relevant categories of accuracy and recall. The 0.84 precision for high-risk loans seen in model 2 indicates that there was a 16% false positive rate. In this situation that would mean that 16% of healthy individuals were categorized as high risk. Thus, this model would deny some individuals who should be approved for a loan. However, this is a small casualty to pay for approving fewer individuals who are high-risk/likely to default on their loans. Assuming the company administering the loans is willing to accept that some healthy individuals will be denied loans due to being categorized as false positives for being high-risk the second model with the resampled data would be adequate and recommended.

