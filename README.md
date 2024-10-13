![](https://global.toyota/pages/news/images/2015/10/01/1330/crwa1510_28_s.jpg)
# Regression of Used Car Prices
## Overview:
- This project is part of a Kaggle competition focused on predicting the prices of used cars using machine learning models. The dataset for this competition was generated from a deep learning model trained on the "Used Car Price Prediction Dataset." The objective was to accurately predict car prices based on several features, while applying different data science techniques, including Exploratory Data Analysis (EDA), Feature Engineering, Data Transformation, and Model Training.

- I implemented two regression models: Linear Regression and Random Forest to predict the prices, and the performance was evaluated using various metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²) scores.

## Dataset Description:
The dataset contains features such as car brand, model year, engine power, mileage, transmission type, fuel type, and other variables relevant to car pricing.you can reach to dataset from [here](https://www.kaggle.com/competitions/playground-series-s4e9/data).
# Steps Followed:
## 1. Exploratory Data Analysis (EDA):
The first step involved understanding the dataset through various visualization and analysis techniques:

- Distribution Analysis: Plotted histograms and boxplots to understand the distributions of numerical features like mileage, engine power, and car prices. We observed skewness in features such as price and mileage, which was addressed during Feature Engineering.
- Correlation Analysis: Used heatmaps and scatter plots to study the correlation between features. Highly correlated features like engine size and horsepower showed a strong positive correlation with the target variable, price.
- Confusion Matrix: Though not applicable to regression models, we conducted advanced regression diagnostics, like residual plots, to check the model's prediction accuracy and detect possible anomalies in the predictions.
## 2. Data Preprocessing and Feature Engineering:
Preprocessing and transforming the dataset was crucial in improving model performance:

- Dealing with Missing Data: Checked for missing values and handled them appropriately by using imputation techniques for numerical features (mean/mode imputation) and frequent category replacement for categorical data. There were no missing values in the dataset.
- Outlier Detection and Treatment: Applied boxplots and z-scores to identify outliers in features such as mileage and engine power. Some outliers were capped to prevent distortion of model performance.
- Feature Encoding: Categorical variables like transmission, fuel_type, and brand were encoded using One-Hot Encoding to convert them into numerical form, while maintaining meaningful relationships between categories.
Data Transformation: Some skewed features were log-transformed to normalize their distributions, especially features like price and engine power.
## 3. Model Training:
Two models were trained on the dataset to predict the car prices:

- Linear Regression: A basic but effective regression technique was used as a baseline model. The linear regression model performed reasonably well.
- Random Forest: A more advanced ensemble learning technique, Random Forest, was used to improve the predictive performance.
## Results and Analysis:
Linear Regression: Despite being a simple model, linear regression provided valuable insights with a respectable R-squared score of 0.5994. However, the model showed some underfitting, likely due to the complex relationships in the data.

Random Forest: This model outperformed linear regression with an R-squared of 0.6353, indicating a better fit for the data. The reduction in MAE and RMSE values showed that Random Forest made more accurate predictions with fewer errors.
