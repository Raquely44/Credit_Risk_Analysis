# Credit Risk Analysis
## Overview of the analysis: 
The purpose of the analysis is to determine the best supervised machine learning model to assess credit risk. The data that is used is unbalanced; there are far more good loans than risky loans making classifaction trickey.

### Resources
LoanStats_2019.csv</br>
Jupyter Notebook</br>
Python</br>
Scikit-learn</br>
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
From the results listed above we can see the accuracy ranges from the 50% range to the 90% range amoung the four methods. Likewise the precision and recall scores vary as well. The first four methods can be analyisised together as having decent accuracy scores in the 50-68% however the percision scores for high risk for all four was 0.01 which signal large amounts of false positives (low risk loans were marked as high risk). On the other hand the percision of low risk loans were 1.00, a good score. When we look at the recall values for both high and low risk we see the mid values, which indicate our model is not perfectly predicting loan classifications.</br>
When we look at our last two models we can see an accuracy score of 78% and 93% for Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier which means we are getting more accurate labeling. Our percision scores are also around the same from the first four models with the High Risk loans being more precise. Also Our recall scores are higher meaning we are actually getting a model that is better at predicting the right classification.

### Recommendation
I would recommend the Easy Ensemble AdaBoost Classifier because it gives the most balances results in accuracy, precision, and recall. I would suggest continual fine tuning since the precision for High risk Loand is quite low, meaning there are alot of false positives or low risk loans that were classified as high risk.

