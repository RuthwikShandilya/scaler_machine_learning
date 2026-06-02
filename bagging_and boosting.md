# Ensemble Methods

## Why Ensemble Methods?

A single ML model may not generalize well because every algorithm has its own weaknesses.

Ensemble Learning combines predictions from multiple models to produce a more robust and accurate final prediction.

Instead of trusting one model, what if we combine many models?

Multiple Models
      ↓
Combine Predictions
      ↓
Better Final Prediction


## Bias-Variance Tradeoff

Most machine learning problems can be viewed through the lens of Bias and Variance.

High Variance (Overfitting)

A high variance model is extremely sensitive to fluctuations in the training data.

Characteristics:
- Learns noise along with actual patterns
- Performs well on training data
- Generalizes poorly to unseen data
- Small changes in training data can significantly alter the model

Example

Decision Trees

Interview Statement:

Decision Trees are considered high variance models because small changes in the training dataset can result in 
a completely different tree structure.

##High Bias (Underfitting)

A high bias model is too simple to capture the underlying complexity of the data.

Characteristics
- Misses important patterns
- Strong assumptions about the data
- Poor performance on both training and test datasets

Example

Very shallow trees or simple linear models on complex problems.

Interview Statement:

High bias occurs when the model lacks sufficient complexity to learn the true relationship between input features and the target variable.


## Ensemble Methods

Two major ensemble techniques:

1. Bagging (Bootstrap Aggregating)

Primary Objective: Reduce Variance

Bagging (Bootstrap Aggregating)
Definition

Bagging trains multiple models independently on different bootstrap samples of the dataset and combines their predictions.

Why Does Bagging Work?

Different models make different errors.

By averaging predictions, random fluctuations tend to cancel out.

Interview Statement:

Bagging reduces variance by averaging multiple independently trained models, resulting in more stable and robust predictions.

### Random Forest
Definition

Random Forest is an ensemble of Decision Trees built using Bagging and Random Feature Selection.

At each split, Random Forest considers only a random subset of features rather than evaluating all features.

This ensures that trees become less correlated with each other.

2. Boosting

Primary Objective: Reduce Bias

### Boosting
Definition

Boosting is an ensemble technique where models are trained sequentially, and each new model focuses on correcting errors made by previous models.

Primary Goal: Reduce Bias

Why Does Boosting Work?

Each model learns from the residual errors of previous models.

Over multiple iterations, the ensemble progressively improves its predictive capability.

Interview Statement:

Boosting reduces bias by sequentially fitting models to the errors of previous models, thereby creating a strong learner from multiple weak learners.



Popular Boosting Algorithms
AdaBoost
First successful boosting algorithm
Assigns higher weights to misclassified observations
Gradient Boosting
Learns residual errors using gradient descent principles
More powerful than AdaBoost
XGBoost
Optimized implementation of Gradient Boosting
Regularization support
High predictive accuracy
LightGBM
Faster training
Lower memory usage
Suitable for large datasets
CatBoost
Handles categorical variables effectively
Requires minimal preprocessing
Bagging vs Boosting
Aspect	Bagging	Boosting
Objective	Reduce Variance	Reduce Bias
Training Style	Parallel	Sequential
Model Dependency	Independent	Dependent
Main Strength	Stability	Accuracy
Overfitting Risk	Lower	Higher
Typical Base Model	Decision Tree	Decision Tree
Example	Random Forest	XGBoost, LightGBM, CatBoost
Most Important Interview Answers
What is Ensemble Learning?

Ensemble Learning is a technique that combines multiple models to achieve better predictive performance and generalization than any individual model.

Why are Decision Trees considered high variance models?

Small changes in the training dataset can result in significantly different tree structures, making Decision Trees highly sensitive to data variations.

What problem does Bagging solve?

Bagging primarily reduces variance by training multiple models on bootstrap samples and aggregating their predictions.

What problem does Boosting solve?

Boosting primarily reduces bias by sequentially learning from previous prediction errors.

What is the difference between Random Forest and Bagging?

Random Forest extends Bagging by introducing random feature selection at each split, which reduces correlation among trees and further decreases variance.

Why is Random Forest usually preferred over a single Decision Tree?

Random Forest maintains the low bias of Decision Trees while significantly reducing variance, leading to better generalization performance.

One-Line Revision
Ensemble Learning = Combining Multiple Models

Bagging → Reduces Variance
Random Forest → Bagging + Feature Randomness

Boosting → Reduces Bias
XGBoost, LightGBM, CatBoost → Popular Boosting Algorithms

Decision Tree:
Low Bias + High Variance

Random Forest:
Low Bias + Lower Variance

Interview Memory Trick:

Bagging = Train Independently + Average Predictions
Boosting = Learn Sequentially + Correct Errors

These notes use terminology such as generalization, bootstrap sampling, weak learner, residual errors, model correlation, variance reduction, and sequential learning, which is the vocabulary interviewers expect from Data Scientist, ML Engineer, and Applied Scientist candidates.















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


# One Line Revision 

Ensemble Learning = Combining Multiple Models

Bagging → Reduces Variance
Random Forest → Bagging + Feature Randomness

Boosting → Reduces Bias
XGBoost, LightGBM, CatBoost → Popular Boosting Algorithms

Decision Tree:
Low Bias + High Variance

Random Forest:
Low Bias + Lower Variance

Interview Memory Trick:

Bagging = Train Independently + Average Predictions
Boosting = Learn Sequentially + Correct Errors
