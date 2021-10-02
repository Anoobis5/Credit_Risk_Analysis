# Credit_Risk_Analysis

## Project Overview
We were tasked to create a Supervised Machine Learning Model that could accurately predict credit risk. We wanted to look at several factors using our loan_stats.csv file to help predict whether somebody might qualify as high or low risk status.  In order to determine credit risk factors amongst our data set, we used the following methods:

  1. Naive Random Oversampling
  2. SMOTE Oversampling
  3. Cluster Centroid Undersampling
  4. SMOTEENN Sampling
  5. Balanced Random Forest Classifying
  6. Easy Ensemble Classifying

## Results

When we examine the results of the balanced accuracy scores and the precision and the recall scores of each of the six machine learning methods, we were able to observe that: 

#### Naive Random Oversampling: 
  * The balanced accuracy score is about 64%. 
  * The high_risk precision is only 1% with a sensitivity of 62%, which makes an F1 of 2%.
  * Due to the high number of low_risk populations, its precision is 100% with a sensitivity of 67%.


#### SMOTE Oversampling
  * The balanced accuracy score is about 65%
  * The high_risk precision is about 1% only with 66% sensitivity which makes a F1 of 2% only.
  * Due to the high number of low_risk populations, its precision is almost 100% with a sensitivity of 64%.


#### Cluster Centroid Undersampling
  * The balanced accuracy score is down to about 51%.
  * The high_risk precision is still 1% only with 59% sensitivity which makes a F1 of 1%.
  * Due to the high number of false positives, the low_risk sensitivity is only 43%.


#### SMOTEENN Sampling
  * The balanced accuracy score is about 63%.
  * The high_risk precision is still 1% only with 71% sensitivity which makes a F1 of only 2%.
  * Due to the high number of false positives, the low_risk sensitivity is 55%.


#### Balanced Random Forest Classifier
  * The balanced accuracy score improved to about 67%.
  * The high_risk precision is now high at 60% only with a 34% sensitivity.
  * Due to a low  number of false positives, the low_risk sensitivity is now 100% with 100% presicion.


#### Easy Ensemble Classifying
  * The balanced accuracy score is high to about 92%. 
  * The high_risk precision is still low at 6% with 91% sensitivity which makes a F1 of only 14%.
  * Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.



## Project Summary

Our analysis aims to find the best model that can detect if a loan is high risk or not. BIn order to do that, we need to find a model that lets the least amount of high risk loans pass through undetected. Our first four models oversamples, undersampled, and a combination of both to determin which is best at predicting which loans are the highest risks. The final two models we used ensemble classifiers to resample the data to try and determine wether loans are either high or low risk. 

Ideally we want our models to display a good balance of recall and precision. That is why it is within our best interest to recommend using the ensemble classifiers over the other models. The Easy Ensemble Classifier model shows a high recall accuracy score of 92%. This would detect almost all high-risk cases. However, with a low precision of 6% with 91% sesnitivity, a lot of low risk credits are still falsely detected as high risk which would be detrimental to the bank's credit strategy. Based on our analyses, we would not be comfortable recomending any of these models to accurately predict credit risk.
