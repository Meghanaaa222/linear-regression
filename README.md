# Housing Price Prediction – Linear Regression

This project demonstrates Simple and Multiple Linear Regression using Python and Scikit-learn to predict housing prices based on various features.

Dataset

The dataset (`Housing.csv`) contains housing-related attributes such as:

- `area` (in sq. ft.)
- `bedrooms`, `bathrooms`, `stories`
- `mainroad`, `guestroom`, `basement`
- `hotwaterheating`, `airconditioning`
- `parking`, `prefarea`
- `furnishingstatus`

 Objectives

- Apply Simple Linear Regression using only the `area` feature.
- Apply Multiple Linear Regression using all available features (encoded where necessary).
- Compare model performance using regression metrics.
- Visualize regression results and feature importance.

 
Methodology

Simple Linear Regression
- Feature: `area`
- Equation:  
  \[
  price = 425.73 \times area + 2,512,254.26
  \]

Metrics:
- MAE: `1,474,748.13`
- MSE: `3.68 × 10¹²`
- RMSE: `1,917,103.70`
- R²: `0.2729`

Multiple Linear Regression
Features: All numerical and one-hot encoded categorical variables.
Scaling: Standardized using `StandardScaler`.

Metrics:
- MAE: `970,043.40`
- MSE: `1.75 × 10¹²`
- RMSE: `1,324,506.96`
- R²: `0.6529`

Feature Importance
Magnitude of coefficients shows influence on price:

- Positive: `bathrooms`, `area`, `airconditioning`, `stories`
- Negative:`furnishingstatus_unfurnished`, `furnishingstatus_semi-furnished`

