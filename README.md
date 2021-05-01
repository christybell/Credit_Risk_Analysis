# Supervised Machine Learning and Credit Risk

<img src="images/machine-learning-brain.jpg" width="1000" height="450">

## Project Overview
In this project, I used Python to build and evaluate several machine learning models to predict credit risk.
I employed the following different techniques:

- Oversample the data using the `RandomOverSampler` and `SMOTE` algorithms.
- Undersample the data using the `ClusterCentroids` algorithm.
- Use a combinatorial approach of over- and undersampling using the `SMOTEENN` algorithm.
- Compare two machine learning models that reduce bias, `BalancedRandomForestClassifier` and `EasyEnsembleClassifier`.

I will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Resources
- **Data Source**: LoanStats_2019Q1.csv
- **Software and Tools**: Python, Anaconda, Jupyter Notebook & Git Bash

## Deliverables & Results

### Deliverable 1: Use Resampling Models to Predict Credit Risk

### RandomOverSampler Model

- **Accuracy Score is 65.4%**
- **Precision High Risk Score is 1%**
- **Precision Low Risk Score is 100%**
- **Recall High Risk Score is 73%**
- **Recall Low Risk Score is 58**
<img src="images/Random Oversampler Results.PNG">

### SMOTE Model

- **Accuracy Score is 66.3%**
- **Precision High Risk Score is 1%**
- **Precision Low Risk Score is 100%**
- **Recall High Risk Score is 63%**
- **Recall Low Risk Score is 69%**
<img src="images/SMOTE Oversampling Results.PNG">

### ClusterCentroids Model

- **Accuracy Score is 66.3%**
- **Precision High Risk Score is 1%**
- **Precision Low Risk Score is 100%**
- **Recall High Risk Score is 69%**
- **Recall Low Risk Score is 40%**
<img src="images/Cluster Centroids Undersampling Results.PNG">

### Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk

### SMOTEENN Model

- **Accuracy Score is 54.5%**
- **Precision High Risk Score is 1%**
- **Precision Low Risk Score is 100%**
- **Recall High Risk Score is 79%**
- **Recall Low Risk Score is 56%**
<img src="images/SMOTEENN Results.PNG">

### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

### BalancedRandomForestClassifier Model

- **Accuracy Score is 78.9%**
- **Precision High Risk Score is 3%**
- **Precision Low Risk Score is 100%**
- **Recall High Risk Score is 70%**
- **Recall Low Risk Score is 87%**
<img src="images/Balanced Random Forest Classifier Results.PNG">

### EasyEnsembleClassifier Model

- **Accuracy Score is 93.2%**
- **Precision High Risk Score is 9%**
- **Precision Low Risk Score is 100%**
- **Recall High Risk Score is 92%**
- **Recall Low Risk Score is 94%**
<img src="images/Easy Ensemble Classifier Results.PNG">

## Summary
In summary, the results of these machine learning models show that the two Ensemble Classifiers perform best. When we compare the accuracy scores of all the models, the Balanced Random Forest Classifier model and the Easy Ensemble Classifier model had the highest scores, at 78.9% and 93.2% respectively. Since the goal of our analysis is to find a model that can best detect when a loan is high risk, we should take a close look at how all the models performed for the recall high risk score. When we compare these statistics, we find that the Easy Ensemble Classifier had the highest score at 92%. Therefore, the model I would recommend to use for predicting high risk loans is the Easy Ensemble Classifier model due to its recall high risk score and its good performance overall.
