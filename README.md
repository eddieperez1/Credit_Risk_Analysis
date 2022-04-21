# Credit_Risk_Analysis

## Overview of the analysis: 
### Outline

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we'll need to employ different techniques to train and evaluate models with unbalanced classes. A client asks us to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling and ensemble. Logistic Regression is used across multiple different sampling techniques. The results are compared to see which method has the highest accuracy score and highest sensitivity. In other words, to find the best model that can predict a high percentage of high-risk loans accurately even if it predicts low-risk loans incorrectly. The data is cleaned so that all values are numeric and prepared for machine learning analysis.

## Results: 

### Random Over Sampler:
- Accuracy Score: 0.66143
- Precision: 0.01
- Recall: 0.72

![ROS image](/screenshots/RandomOversampler.PNG)

### SMOTE:
- Accuracy Score: 0.65811
- Precision: 0.01
- Recall: 0.62

![SMOTE image](/screenshots/SMOTE.PNG)

### ClusterCentroids
- Accuracy Score: 0.54778
- Precision: 0.01
- Recall: 0.66

![CC image](/screenshots/ClusterCentroids.PNG)

### SMOTEENN
- Accuracy Score: 0.67107
- Precision: 0.01
- Recall: 0.77

![SMOTEENN image](/screenshots/SMOTEENN.PNG)

### Balanced Random Forest Classifier
- Accuracy Score: 0.72844
- Precision: 0.06
- Recall: 0.50

![BRFC image](/screenshots/BalancedRandomForest.PNG)

### Easy Ensemble Classifier
- Accuracy Score: 0.93167
- Precision: 0.09
- Recall: 0.92

![EEC image](/screenshots/EasyEnsemble.PNG)    

## Summary:
### Conclusions and Recommendations
The best model was Easy Ensemble Classifier with an accuracy score of 0.93167 and a recall of 0.92. The worst model was Cluster Centroids with an accuracy score of 0.54778 and a recall of 0.66. The model recommended to use is the Easy Ensemble Classifier because it has the highest accuracy score and recall.