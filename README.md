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

### Naive Random Oversampling: 
  * The balanced accuracy score is about 64%. 
  * The high_risk precision is only 1% with a sensitivity of 62%, which makes an F1 of 2%.
  * Due to the high number of low_risk populations, its precision is 100% with a sensitivity of 67%.


### SMOTE Oversampling
  * Our results for this method are similar to the Naive Random Oversampling method.
  * The balanced accuracy score is about 65%
  * The high_risk precision is about 1% only with 66% sensitivity which makes a F1 of 2% only.
  * Due to the high number of low_risk populations, its precision is almost 100% with a sensitivity of 64%.

### Cluster Centroid Undersampling
  * The balanced accuracy score is down to about 51%.
  * The high_risk precision is still 1% only with 59% sensitivity which makes a F1 of 1%.
  * Due to the high number of false positives, the low_risk sensitivity is only 43%.

### SMOTEENN Sampling
  * The balanced accuracy score is about 63%.
  * The high_risk precision is still 1% only with 71% sensitivity which makes a F1 of only 2%.
  * Due to the high number of false positives, the low_risk sensitivity is 55%.
