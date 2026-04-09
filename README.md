# Housing Price Prediction 🏠

Predict house prices using **Multiple Linear Regression** in Python.

## Dataset
- Source: [Kaggle Housing Prices Dataset](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset)  
- Features: area, bedrooms, bathrooms, stories, mainroad, guestroom, basement, hotwaterheating, airconditioning, parking, prefarea, furnishingstatus  

## How it works
1. Preprocess data: encode yes/no as 1/0, ordinal encoding for furnishing status.  
2. Train a Linear Regression model.  
3. Evaluate model using **R² Score** (~0.65).  
4. Save model with `joblib` for future predictions.

## Multiple Linear Regression Equation

The general multiple linear regression equation:

$$
\hat{y} = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \dots + \beta_n x_n
$$

For our housing dataset, the equation becomes:

$$
\text{Price} = \beta_0 + \beta_1 (\text{Area}) + \beta_2 (\text{Bedrooms}) + \beta_3 (\text{Bathrooms}) + \beta_4 (\text{Stories}) + \beta_5 (\text{MainRoad}) + \beta_6 (\text{GuestRoom}) + \beta_7 (\text{Basement}) + \beta_8 (\text{HotWaterHeating}) + \beta_9 (\text{AirConditioning}) + \beta_{10} (\text{Parking}) + \beta_{11} (\text{PrefArea}) + \beta_{12} (\text{FurnishingStatus})
$$


# Requirements
- Python 3.10+
- pandas, numpy, scikit-learn, joblib
