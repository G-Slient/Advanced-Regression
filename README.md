# House Price Prediction
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

## Table of Contents
* [Problem Statement](#problem-statement)
* [Business Goal](#business-goal)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)

## Problem Statement

The company wants to know:
   - Which variables are significant in predicting the price of a house, and
   - How well those variables describe the price of a house.
Also, determine the optimal value of lambda for ridge and lasso regression.

## Conclusions

### Final Model:
    Lasso [alpha : 0.001]
    Number of Features : 45
    Train R2 Score : 0.897
    Test R2 Score : 0.883

- Our model has been able to explain 89.7% variance in train and 88.3% variance in test
- Just 1% of gap between Train and Test R2 Score proves the final model is robust

### Top 5 Features : (based on coef)
    - Neighborhood_Crawfor : (Crawford)
    - Neighborhood_Edwards : (Edwards)
    - OverallQual_7 : (Good)
    - OverallQual_simple : (OverallQual Feature squashed into smaller groups)
    - Total_SF : (TotalBsmtSF + GrLivArea)

- Best Parameter for Ridge Model : 'alpha': 5.0
- Best Parameter for Lasso Model : 'alpha': 0.001

## Technologies Used
- numpy - version 1.21.5
- pandas - version 1.4.2
- matplotlib - version 3.5.1
- seaborn - version 0.11.2
- statsmodels - version 0.13.2
- sklearn - version 1.0.2

## Contact
Created by [@G-Slient] - feel free to contact me!
