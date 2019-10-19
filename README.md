# CTR-Prediction-Using-Text-and-Numerical-Data
Predicting Clicks and Click Through Rate of ads using their text and other features.

Using the advertisement data which contains text and other numerical features like keywords and their average position, Cost, target market and etc. Using this data to predict the Clicks and Click through rate which is useful for the advertising companies as it will guide them towards making better ads.

I used NLP techniques like tf idf and word vectors and then other pre processing for this task. For tfidf training people's wiki dataset was used for better training and Used Scikit learn for feature extraction and feature generation and model building and prediction. 
The metric of evaluation I used was RMSE but due to limitations and its problems I used R2 score but then due to its problem of increasing score when adding new features, and so I used Adjusted R2 score.

XGBoost worked the best in both cases of predicting clicks and Click thorogh ratio (CTR).
Linear model wasnt good for CTR predicting but gave a acceptable answer for Clicks
SVM was the worst among all the algorithms

Here are the results for test data:

Linear Regression for prediction of clicks
  RMSE: 1460.213436
  R2 score =  0.6679342949614837
  Adjusted R2 score =  0.6679013050248968

XGBOOST for prediction of clicks
  RMSE: 162.238753
  R2 score =  0.9959007864524558
  Adjusted R2 score =  0.995900379205357
  
Linear Regression for prediction of CTR
  RMSE: 1.691520
  R2 score =  0.38103071163636404
  Adjusted R2 score =  0.3809692185123752

XGBOOST for prediction of CTR
  RMSE: 0.149034
  R2 score =  0.9951951072489301
  Adjusted R2 score =  0.9951946298942839
  
  
So seeing the result, we can easily say that xgboost worked the best for this problem as it gave 99% accuracy on test data for both clicks and CTR prediction. 
