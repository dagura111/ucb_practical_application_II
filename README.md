# Car Price Analysis Notebook

## Overview
This Jupyter notebook is to explore a dataset from Kaggle containing information on used cars. The provided dataset contains information on 426,000 cars, selected for processing speed from an original dataset of 3 million entries. The goal is to identify factors that affect a car's price to help used car dealerships understand consumer values.

## CRISP-DM Framework
The analysis follows the CRISP-DM (Cross-Industry Standard Process for Data Mining) framework, providing a structured approach to data analysis projects.

## Final Models:
1. Linear Regression:
Training RMSE: 0.2219
Test RMSE: 0.2217
Easy to understand the impact of each feature on the target variable and it's a low Computation Time. Since the training and test errors are very close this model generalizes well

2. Random Forest (n_estimators=100):
Training RMSE: 0.0462
Test RMSE: 0.1232
Random Forest models are difficult to understand and kind of a black box. The computation time is high but since the model has a much lower RMSE on both training and test sets compared to linear regression the performance will be good.

3. Random Forest (n_estimators=10):
Training RMSE: 0.0559
Test RMSE: 0.1305
As said before Random Forest models are difficult to understand and this model computation time is better than 100 trees but higher than the linear regression. The performance should be better than linear regression but lower than the model with n_estimators=100.

To get the best model the Random forest with 100 trees is the best performing model but if the model will be used in a real-time system where prediction speed is important, the linear regression or smaller Random Forest may be preferable. If it will be used in where prediction speed is less critical, a more complex Random Forest could be used.