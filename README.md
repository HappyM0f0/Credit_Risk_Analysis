# Credit_Risk_Analysis
 
## Overview of the analysis:
Use Python to build and evaluate several machine learning models to predict credit risk.

The following was completed using a credit card credit dataset from LendingClub
- oversample the data using the RandomOverSampler and SMOTE algorithms
- undersample the data using the ClusterCentroids algorithm
- combinatorial approach of over- and undersampling using the SMOTEENN algorithm
- compare two new machine learning models that reduce bias
    - BalancedRandomForestClassifier and EasyEnsembleClassifier

## Results: 
<br/>

**Naive Random Oversampling** 
- Accuracy score: 0.629
- high_risk: precision is about 1% only with 57% sensitivity which makes a F1 of 2%
- low_risk: precision is almost 100% with a sensitivity of 68%
![nro](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/nro.png)
<br/>

**SMOTE**
- Accuracy score: 0.627
- high_risk: precision is about 1% only with 62% sensitivity which makes a F1 of 2%
- low_risk: precision is almost 100% with a sensitivity of 63%.
![smote](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/smote.png)
<br/>

**ClusterCentroid (Undersampling)**
- Accuracy score: 0.51
- high_risk: precision is about 1% only with 59% sensitivity which makes a F1 of 1%
- low_risk: precision is almost 100% with a sensitivity of 43%.
![cc](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/cc.png)
<br/>

**SMOTEENN (combination)**
- Accuracy score: 0.51
- high_risk: precision is about 1% only with 70% sensitivity which makes a F1 of 2%
- low_risk: precision is almost 100% with a sensitivity of 61%.
![smoteenn](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/smoteenn.png)
<br/>

**Balanced Random Forest Classifier**
- Accuracy score: 0.79
- high_risk: precision is about 4% only with 67% sensitivity which makes a F1 of 7%
- low_risk: precision is almost 100% with a sensitivity of 91%.
![BRF](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/BRF.png)
<br/>

**Easy Ensemble AdaBoost**
- Accuracy score: 0.93
- high_risk: precision is about 7% only with 91% sensitivity which makes a F1 of 14%
- low_risk: precision is almost 100% with a sensitivity of 94%.
![EEC](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/eec.png)

## Summary: 
All models used to perform credit risk analysis show weak precision with high risk. The EasyEnsembleClassifier model shows a recall of 91% and detects the highest amount of high-risk individuals at 7%. However, the low precision would categorize some low-risk credits as high-risk, negatively impacting the bank's credit strategy and affecting revenue by missing credit opportunities. I cannot recommend any models for use as the precision and F1 scores are to low for a positive impact.