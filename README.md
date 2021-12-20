# Credit_Risk_Analysis
 
## Overview of the analysis:
Explain the purpose of this analysis.

## Results: 
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

- Naive Random Oversampling 
    - Accuracy score: 0.629
    - high_risk: precision is about 1% only with 57% sensitivity which makes a F1 of 2%
    - low_risk: precision is almost 100% with a sensitivity of 68%
![nro](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/nro.png)
- SMOTE
    - Accuracy score: 0.627
    - high_risk: precision is about 1% only with 62% sensitivity which makes a F1 of 2%
    - low_risk: precision is almost 100% with a sensitivity of 63%.
![smote](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/smote.png)
- ClusterCentroid (Undersampling)
    - Accuracy score: 0.51
    - high_risk: precision is about 1% only with 59% sensitivity which makes a F1 of 1%
    - low_risk: precision is almost 100% with a sensitivity of 43%.
![cc](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/cc.png)
- SMOTEENN (combination)
    - Accuracy score: 0.51
    - high_risk: precision is about 1% only with 70% sensitivity which makes a F1 of 2%
    - low_risk: precision is almost 100% with a sensitivity of 61%.
![smoteenn](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/smoteenn.png)
- Balanced Random Forest Classifier
    - Accuracy score: 0.79
    - high_risk: precision is about 4% only with 67% sensitivity which makes a F1 of 7%
    - low_risk: precision is almost 100% with a sensitivity of 91%.
![BRF](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/BRF.png)
- Easy Ensemble AdaBoost
    - Accuracy score: 0.93
    - high_risk: precision is about 7% only with 91% sensitivity which makes a F1 of 14%
    - low_risk: precision is almost 100% with a sensitivity of 94%.
![EEC](https://github.com/HappyM0f0/Credit_Risk_Analysis/blob/main/Resources/eec.png)

## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.