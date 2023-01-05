# Credit_Risk_Analysis

# Overview:
The purpose of this analysis is that we use supervised Machine Learning models to predict the status of a loans. To do so, we first gathered the data from a csv file into a dataframe. We then divide the features and the target columns, where features are independant variables which machine learning models will use to predict the target column which was "loan_status" for our problem. And loan status had two values, namely, low_risk and high_risk. We used several machine learning models to predict whether a loan was risky or not. Then amongst, all the machine learning model, we will determine which model provides us the best accuracy score. 

# Results:
For our analysisAfter splitting the X_train, X_test, y_train, and y_test, we used six Machine Learning models to train and test on our data. The higher the balanced accuracy score, the better the model. Higher precision score implies that the model is predicting more true positive with respect to false positive and higher sensitivity score implies that the model is predicting more true positive with respect to false negative. For our case of predicting risky loans, we value precision more than sensitivity and we also value balanced accuracy score. They are listed below: 
- RandomOverSampling: This model gave us a balanced accuracy score of 0.646. The high_risk class has precision score of 0.01, and sensitivity score of 0.71, and the low_risk class has precision score of 1.0, and sensitivity score of 0.58.  
- SMOTE: This model gave us a balanced accuracy score of 0.658. The high_risk class has precision score of 0.01, and sensitivity score of 0.63, and the low_risk class has precision score of 1.0, and sensitivity score of 0.68.
- ClusterCentroids: This model gave us a balanced accuracy score of 0.544. The high_risk class has precision score of 0.01, and sensitivity score of 0.69, and the low_risk class has precision score of 1.0, and sensitivity score of 0.40.
- SMOTEENN: This model gave us a balanced accuracy score of 0.628. The high_risk class has precision score of 0.01, and sensitivity score of 0.65, and the low_risk class has precision score of 1.0, and sensitivity score of 0.60.
- BalancedRandomForestClassifier: This model gave us a balanced accuracy score of 0.788. The high_risk class has precision score of 0.03, and sensitivity score of 0.70, and the low_risk class has precision score of 1.0, and sensitivity score of 0.87.
- EasyEnsembleClassifier: This model gave us a balanced accuracy score of 0.932. The high_risk class has precision score of 0.09, and sensitivity score of 0.92, and the low_risk class has precision score of 1.0, and sensitivity score of 0.94.

# Summary:
After running all the above models, I have come to the conclusion that EasyEnsembleClassifier is the best model to use as it had the highest accuracy score being 0.932, and it had the highest precision score for detecting high_risk loans compared to the rest of the models. It also had a very high sensitivity score, being 0.92 which is great to have. However, the precision score is still very low, being 0.09, thus I recommend trying out more ML models to see if we can reach a higher precision score along with balanced accuracy score. 






