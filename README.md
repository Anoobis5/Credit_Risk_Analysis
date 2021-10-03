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
  * The balanced accuracy score is about 65%. 
  * The high_risk precision is only 1% with a sensitivity of 73%
  * The low_risk precision is 100% with a sensitivity of 57%

![Oversampling](https://user-images.githubusercontent.com/84881187/135723187-cbf32adc-99be-42fc-9bf6-65bd285e1cb7.PNG)


#### SMOTE Oversampling
  * The balanced accuracy score is about 66%
  * The high_risk precision is about 1% only with a sensitivity of 78%.
  * The low_risk precision is almost 100%, but with a sensitivity of 54%
![SMOTE Method](https://user-images.githubusercontent.com/84881187/135723194-88769a36-7337-4d5b-8053-c54d322bf7ae.PNG)


#### Cluster Centroid Undersampling
  * The balanced accuracy score is down to about 54%.
  * The high_risk precision is still 1% only with 69% sensitivity which makes a F1 of 1%.
  * The low_risk precision is 100% with a sensitivity of 40%

![Undersampling Method](https://user-images.githubusercontent.com/84881187/135723248-155d9612-67d4-4d02-8d47-33408f9dcf49.PNG)


#### SMOTEENN Sampling
  * The balanced accuracy score is about 66%.
  * The high_risk precision is still 1% only with 78% sensitivity which makes a F1 of only 2%.
  * The low risk score is still 100% with a 54$ sensitivity score.
![SMOTEENN](https://user-images.githubusercontent.com/84881187/135723255-ee5e909d-b8e3-4b92-aaa1-472ce4f48778.PNG)


#### Balanced Random Forest Classifier
  * The balanced accuracy score improved to about 68%.
  * The high_risk precision is now high at 88%, but with only a 37% sensitivity score.
  * Due to the incredibly high True Negative score, the low_risk precision is 100% and the sensitivity score is also 100$ **

![Balanced_Random_Forest_Classifier](https://user-images.githubusercontent.com/84881187/135723263-a8986340-c835-4478-8256-e7c30f03beab.PNG)

#### Easy Ensemble Classifying
  * The balanced accuracy score is high to about 93%. 
  * The high_risk precision is still low at 9%, but with 92% sensitivity which makes a F1 of only 14%.
  * Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

![Easy_Ensemble_ADABoost_Classifier](https://user-images.githubusercontent.com/84881187/135723270-a570ce12-0471-42cc-98f6-de0d35b200ac.PNG)


## Project Summary

Our analysis aims to find the best model that can detect if a loan is high risk or not. BIn order to do that, we need to find a model that lets the least amount of high risk loans pass through undetected. Our first four models oversamples, undersampled, and a combination of both to determin which is best at predicting which loans are the highest risks. The final two models we used ensemble classifiers to resample the data to try and determine wether loans are either high or low risk. 

Ideally we want our models to display a good balance of recall and precision. That is why it is within our best interest to recommend using the ensemble classifiers over the other models. The Easy Ensemble Classifier model shows a high recall accuracy score of 93%. However, with a low precision of 9% with 92% sesnitivity, a lot of low risk credits are still falsely detected as high risk which would be detrimental to the bank's credit strategy. On the other-hand, using a Random Forest Classifier would give us an 88$ score when detecting high risk cases, but the sensitivity would drop to 37%. Based on our analyses, we would not be comfortable recomending any of these models to accurately predict credit risk.
