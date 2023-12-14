# House Rent Prediction Project

## Overview

This project focuses on predicting house rents based on various features such as size, locality, and furnishing status. The goal is to develop an accurate predictive model that aids in estimating rental values for residential properties.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Graphs](#graphs)
- [Model Development](#model-development)
- [Model Evaluation](#model-evaluation)
- [Conclusion](#conclusion)

## Introduction

In the pursuit of accurate house rent predictions, we explored different regression models, including linear regression, XGBoost regression, and Random Forest regression. The project also involved creating a stacked ensemble model, combining multiple algorithms to enhance predictive accuracy.

## Dataset

The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/datasets/iamsouravbanerjee/house-rent-prediction-dataset). Special thanks to the dataset contributor [iamsouravbanerjee](https://www.kaggle.com/iamsouravbanerjee) for making this data available.

The dataset used in this project contains information about various rental properties, including size, area type, city, and furnishing status. Additionally, the dataset includes the target variable, rent, measured in INR, which was converted to EUR for better understanding.

## Data Preprocessing

Data preprocessing steps were crucial in refining the dataset for modeling. This included handling outliers, converting currencies, and transforming categorical variables. Noteworthy preprocessing steps:

- Extracting floor information
- Reducing dimensionality of area type and city
- Converting categorical features to ordered categories

## Graphs

Visualizations were created to explore relationships between key features and rental values. Examples include:

- Size vs. Rent by Area Type
- Size vs. Rent by City
- Size vs. Rent by Furnishing Status
- Size vs. Rent by Bathroom Count
- Size vs. Rent by Point of Contact

These visualizations provide insights into the relationships between different features and rental values, aiding in understanding the impact of each variable on the rent


## Model Development

We experimented with various regression models to identify the most suitable one for our prediction task. Models included:

- Linear Regression
- Random Forest Regression
- XGBoost Regression
- Stacking Ensemble Model (Linear, XGBoost, and Random Forest)

## Model Evaluation

Model evaluation was conducted to assess predictive performance. Key metrics considered:

- Root Mean Squared Error (RMSE)
- R-squared Score (R2)

The best-performing model, XGBoost Regression, exhibited a slight trade-off between RMSE and R2 compared to Random Forest but provided a substantial speed advantage.

## Conclusion

Despite the efforts to construct a stacked ensemble model, the marginal gain in predictive accuracy did not justify the increased complexity. The XGBoost Regression model, with a slightly worse RMSE and R2, proved considerably faster, making it a practical choice for certain applications.

It's essential to note that model performance may be influenced by specific dataset characteristics. Further refinement and experimentation could unveil optimization opportunities. The mean rent was found to be 207.53 EUR.


