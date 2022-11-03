# Surprise Housing
> This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.
Answer the below question:
Which variables are significant in predicting the price of a house, and
How well those variables describe the price of a house.


## Table of Contents
* Business Objective
* Understanding and Cleaning the data
* EDA
* Outliers detction and handling
* Derived columns
* Model Build using Ridge and Lasso

<!-- You can include any other section that is pertinent to your problem -->

## General Information
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The company is looking at prospective properties to buy to enter the market. And want to build a model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Top 5 significant features as per Lasso Regression:
* ('OverallQual_Excellent', 0.1428)
* ('Functional_Typical Functionality', 0.0958)
* ('Exterior1st_BrkFace', 0.0946)
* ('1stFlrSF', 0.0935)
* ('2ndFlrSF', 0.0921)

## Metrices for Training data for Lasso Regression:
* Lasso testing R2 score: 0.889
* The RSS value of Test data: 6.037
* The mse value of Test data: 0.021
* The RMSE value of Test data: 0.144
* Adjusted R square: 0.831

## Metrices for Testing data for Lasso Regression:
* Lasso training R2 score : 0.911
* The RSS value of Taining data: 15.806
* The MSE value of Taining data: 0.014
* The RMSE value of Taining data: 0.116
* Adjusted R Square: 0.903

## Top 5 significant features as per Ridge Regression:
* ('BsmtUnfSF', 0.123) 
* ('MSZoning_Residential Low Density', 0.1184) 
* ('BsmtFinSF2', 0.1072)
* ('MSSubClass_2-1/2 STORY ALL AGES', 0.0932)
* ('LandSlope_Moderate', 0.0922)

## Metrices for Training data for Ridge Regression:
* Ridge training R2 score : 0.916
* The RSS value of Taining data: 14.937
* The MSE value of Taining data: 0.0128
* The RMSE value of Taining data: 0.113
*  Adjusted R square: 0.908

## Metrices for Testing data for Ridge Regression:
* Ridge testing R2 score: 0.891
* The RSS value of Test data: 5.945
* The mse value of Test data: 0.020
* The RMSE value of Test data: 0.143
* Adjusted R square: 0.872

## Both Lasso and Ridge regression worked well for this model but I will choose Ridge Regression as it works well with multicollinearity of data and use RFE to select the features. 


## Contact
Created by [@githubusername] - feel free to contact me!
