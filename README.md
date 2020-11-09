# Credit Risk Analysis
## Overview of the analysis: 
The purpose of the analysis is to determine the best supervised machine learning model to assess credit risk. The data that is used is unbalanced; there are far more good loans than risky loans making classifaction trickey.

### Resources
LoanStats_2019.csv
Jupyter Notebook
Python
Scikit-learn
Python 3.7

## Results: 
1. Oversampling: Naive Random Oversampling
* Accuracy Score: 64.03%
* Precision
  * High Risk: 0.01
  * Low Risk: 1.00
* Recall
  * High Risk: 0.66
  * Low Risk: 0.62

2. Oversampling: SMOTE Oversampling
* Accuracy Score: 65.14%
* Precision
  * High Risk: 0.01
  * Low Risk: 1.00
* Recall
  * High Risk: 0.61
  * Low Risk: 0.69


3. Undersampling: Cluster Centroids
* Accuracy Score: 54.74%
* Precision
  * High Risk: 0.01
  * Low Risk: 1.00
* Recall
  * High Risk: 0.68
  * Low Risk: 0.41


4. Combination of Over and Under Sampling
* Accuracy Score: 65.5%
* Precision
  * High Risk: 0.01
  * Low Risk: 1.00
* Recall
  * High Risk: 0.75
  * Low Risk: 0.56


5. Balanced Random Forest Classifier
* Accuracy Score: 78.85%
* Precision
  * High Risk: 0.03
  * Low Risk: 1.00
* Recall
  * High Risk: 0.70
  * Low Risk: 0.87


6. Easy Ensemble AdaBoost Classifier
* Accuracy Score: 93.16%
* Precision
  * High Risk: 0.09
  * Low Risk: 1.00
* Recall
  * High Risk: 0.92
  * Low Risk: 0.94

## Summary: 
From the results listed above we can see the accuracy ranges from the 50% range to the 90% range. Likewise the precision of the high risk 

