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
