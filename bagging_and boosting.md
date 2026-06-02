# Ensemble Methods

Why Ensemble :
Decision Trees are high variance models. Small change in data changes the model 

Instead of trusting one model, what if we combine many models?

Multiple Models
      ↓
Combine Predictions
      ↓
Better Final Prediction


The main problems of machine learning is :
High varience -> which means model is too sensitive.small changes in data results in model change
High Bias     -> Which means model is too simple.Model cannot learn complexity.


## Bagging
The main purpose of  bagging is to reduce varience not primarily bias.
So imagine there are 5 decision trees and each decision tree with sample data will be trained and we will 
take majority/ average of the result so that the variance is solved. 
the error gets nullified basically 
there is with replcement and without replacement and 


Example : Random Forest = Bagging + Feature Randomness

What Problem Does Random Forest Solve?

Single Tree:

Low Bias
High Variance

Random Forest:

Low Bias
Lower Variance

## Boosting 
Boosting is majorly used to solve bias.

Boosting addresses bias by sequentially training models where each new model learns from the mistakes of previous models. 
XGBoost, LightGBM, and CatBoost are common boosting algorithms.
