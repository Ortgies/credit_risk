# credit_risk
Home Credit Default Risk - Kaggle Competition

## Background
In the [Kaggle Home Credit Default Risk Competition](https://www.kaggle.com/c/home-credit-default-risk/overview), participants try to predict predicting future payment behavior of clients from application, demographic and historical credit behavior data.
Because of my academic background in Finance, I wanted to try my hand at a credit risk dataset and this one seemed like an interesting challenge. <br>
A ROC AUC of 0.8 would have been enough to place among the winners of this competition, so this is what I aim for. I want to try a few new methods on this dataset, for example feature reduction with an Autoencoder.

## Current state
The main dataset contains 120 features and one binary target variable. Using the supplementary datasets, I am able to increase the independent feature count to over 1400.
I do manual feature selection to reduce the dimensionality down to the 290 most important features. I am currently working on an Autoencoder as an alternative to manual feature selection. <br>
Using LightGBM I am able to get to a ROC AUC of over 0.78. Now I will have to do hyperparameter tuning to improve on this result.

## TODO
- [X] Feature Engineering
- [X] Manual Feature Selection
- [X] Baseline of LightGBM and NN
- [ ] Autoencoder for dimensionality reduction
- [ ] Hyperparameter tuning
