# Ames Iowa Pricing Project

In Ames, Iowa exploring the Ames Housing dataset

## Project Overview

This project aims to analyze and predict housing prices in Ames, Iowa using the Ames Housing dataset. The dataset contains information about various features of houses, such as their size, location, and condition, as well as their sale prices.

The data was provided in a csv file, you can find [here](/data/DataDocumentation.txt)

## Project Goals

The primary goal of this project is to build a predictiv model that can accurately estimate the sale price of a house in Ames, Iowa based on its features. The model will be trained on the Ames Housing dataset and evaluated using appropriate metrics such as mean squared error (MSE) and root mean squared error (RMSE).

Create a baseline model using only 8 columns as features using other than linear regression model.

## Project Structure

The project is organized into several key components:

1. **Data Preprocessing**: This step involves cleaning and transforming the raw data to prepare it for modeling.This includes removing and filling NaNa values, convertering numeric columns to float
and remove the top outliers from Ground Living Area columns. Besides removing the top outliers, they were left in not interfere with the rest of columns.

&nbsp;

2. **Feature Engineering**: This step involves creating new features from existing ones to improve the model's predictive power. This incluede create subsets of the data to break down for visulization, to create a base model and looking at these and create 1 column 'Time to Sell'.

&nbsp;

3. **Model Selection**: This step involves selecting an appropriate machine learning algorithm ensemble of algorithms to use for prediction.This may include linear regression, Ridge Regression Hist Gradient Boosting Regression and random forests. The main model used Linear Regression and the other 3 algorithm were used for a baseline.  

&nbsp;

4. **Model Training**: This step involves training the selected model on the preprocessed


&nbsp;

5. **Model Performace**: This step involved using a Linear Regression as the main model. I also created baseline models to evaluate my Linear Regression model performance. For the base models I used Ridge Regression, Hist Gradient Boosting Regression and Random Forest Regression.

| Model |  RMSE   | R^2 
|---    |----     |----
Linear Regression   | 28,367 | 0.87 
Ridge  Regression	| 44,202 | 0.62
Boosting Regression | 39,570 | 0.70 
Random Forest Regression | 34,974 | 0.76


![Actual vs Predicted Sale](/images/predicted.png)


5. **Model Evaluation**: This step involves evaluating the trained model's performance on a holdout dataset using appropriate metrics such as MSE and RMSE. This may also involve visualizing the model's predictions and comparing them to the actual sale prices.



## Recommendation 
- Tear down old homes that have been off the market for more than 8 year
- Expanding homes and remodeling old house in Neighborhood such as BrkSide, Old Town, IDOTRR, SWISU, and Edwards.
	- Starting with houses that were built between late 1800's to 1910's.
	- include modern appliance like  A/C and Utilities attract buyers. 




