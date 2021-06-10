# Credit_Risk_Analysis
Module 17: Supervised Machine Learning and Credit Risk


### Project Overview
In this project, we use Python and jupyter notebook to evaluate different machine learning models which predict credit risk.

- Deliverable 1: Use Resampling Models to Predict Credit Risk
- Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
- Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
- Deliverable 4: A Written Report on the Credit Risk Analysis

### Resources
- Data Source:
- Software: Python, Jupyter Notebook


## Deliverable 1: Use Resampling Models to Predict Credit Risk
- Oversampling RandomOverSampler and SMOTE algorithms
- Undersampling ClusterCentroids algorithm
- Using these algorithms, resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report

### RandomOverSampler Model
![](RandomOverSamplerModel1.PNG)
![](RandomOverSamplerModel2.PNG)
![](RandomOverSamplerModel3.PNG)

### SMOTE Model
![](SmoteModel1.PNG)
![](SmoteModel2.PNG)
![](SmoteModel3.PNG)

### ClusterCentroids Model
![](ClusterCentroidsModel1.PNG)
![](ClusterCentroidsModel2.PNG)
![](ClusterCentroidsModel3.PNG)

## Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
![](SmoteennModel1.PNG)
![](SmoteennModel2.PNG)
![](SmoteennModel3.PNG)

## Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

### BalancedRandomForestClassifier Model
![](BalancedRandomForestClassifierModel.PNG)
![](BalancedRandomForestClassifierModel2.PNG)
![](BalancedRandomForestClassifierModel3.PNG)

### EasyEnsembleClassifier Model
![](EasyEnsembleClassifierModel1.PNG)
![](EasyEnsembleClassifierModel2.PNG)
![](EasyEnsembleClassifierModel3.PNG)

## Summary
The credit risk analysis models have weak precision to determine if credit risk is high. Though, the Ensemble models have higher sensitivity of the high risk credits.
On the other hand, the EasyEnsembleClassifier model detects high credit risk, but - with a low precision - a considerable number of low risk credits are erroneously detected as high risk, resulting in missed opportunity.
As a consequence, I cannot recommend of the models to predict credit risk.
