Multi Collinearity is basically a corelation between multiple features in your dataset you ideally want your data set with no multi collinearity. So if one feature could be explained by other feature. The model everytime it trains it gets confused which 
feature to use and everyt time you get different coeefiiects in your Logisttic regression.


With Multi collinearity the feature importance doesnt work properly and it will give unstable results everytime you train the model
we cant interpret the model like which feature is imporant or which is not

Best thing to figure out this is VIF(Variance Inflation Factor)

This is basically telling us if a feature can be measured using other features. If it can be measured we remove that column to tain in the model

R² always increases or remains constant when additional predictors are added, even if those predictors are irrelevant.

Adjusted R² penalizes unnecessary complexity and increases only when a new feature provides sufficient explanatory value.
