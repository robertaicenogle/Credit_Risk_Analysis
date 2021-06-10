# Credit_Risk_Analysis
Module 17: Supervised Machine Learning and Credit Risk


### Project Overview
In this project, we use Python and jupyter notebook to evaluate different machine learning models which predict credit risk. Then we'll make an evaluation based on their performance. See the deliverables below:

- Deliverable 1: Use Resampling Models to Predict Credit Risk
- Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
- Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

### Resources
- Data Source:
- Software: Python, Jupyter Notebook


## Deliverable 1: Use Resampling Models to Predict Credit Risk
- Oversampling RandomOverSampler and SMOTE algorithms
- Undersampling ClusterCentroids algorithm

### RandomOverSampler Model
![](RandomOverSamplerModel1.PNG)
![](RandomOverSamplerModel2.PNG)
![](RandomOverSamplerModel3.PNG)

- The balanced accuracy score is 65%.
- The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
- Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### SMOTE Model
![](SmoteModel1.PNG)
![](SmoteModel2.PNG)
![](SmoteModel3.PNG)

- The results are pretty similar to the previous model.
- The balanced accuracy score is 64%.
- The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
- Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.

### ClusterCentroids Model
![](ClusterCentroidsModel1.PNG)
![](ClusterCentroidsModel2.PNG)
![](ClusterCentroidsModel3.PNG)

- Here the balanced accuracy score is down to about 52%.
- The high_risk precision is still 1% only with 63% sensitivity which makes a F1 of 1%.
- Due to the high number of false positives, the low_risk sensitivity is only 40%.

## Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
![](SmoteennModel1.PNG)
![](SmoteennModel2.PNG)
![](SmoteennModel3.PNG)

-The balanced accuracy score is about 62%.
- The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
- Due to the high number of false positives, the low_risk sensitivity is 57%.

## Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

### BalancedRandomForestClassifier Model
![](BalancedRandomForestClassifierModel.PNG)
![](BalancedRandomForestClassifierModel2.PNG)
![](BalancedRandomForestClassifierModel3.PNG)

- The balanced accuracy score improved to about 79%.
- The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
- Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

### EasyEnsembleClassifier Model
![](EasyEnsembleClassifierModel1.PNG)
![](EasyEnsembleClassifierModel2.PNG)
![](EasyEnsembleClassifierModel3.PNG)

- Now, the balanced accuracy score is high to about 93%.
- The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
- Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

## Summary
The credit risk analysis models have weak precision to determine if credit risk is high. Though, the Ensemble models have higher sensitivity of the high risk credits.
On the other hand, the EasyEnsembleClassifier model detects high credit risk, but - with a low precision - a considerable number of low risk credits are erroneously detected as high risk, resulting in missed opportunity.
As a consequence, I cannot recommend of the models to predict credit risk.
