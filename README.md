Forest Fire Prediction - README
Project Overview
This project develops machine learning models to predict the burned area of forest fires using meteorological and other environmental data. The dataset includes features like temperature, humidity, wind, and rain, along with spatial and temporal information.
Data Description
The dataset contains the following features:

X, Y: Spatial coordinates
FFMC, DMC, DC, ISI: Fire Weather Index (FWI) System components
temp: Temperature (°C)
RH: Relative Humidity (%)
wind: Wind speed (km/h)
rain: Rain amount (mm)
month: Month of the year
day: Day of the week
area: Burned area (hectares) - Target variable

Data Preprocessing

Log-transformation of the target variable ('area') to handle right-skew
One-hot encoding of categorical variables (month, day)
Feature selection to handle multicollinearity (identified using VIF analysis)

Models Evaluated

Linear Regression: Baseline model
Ridge Regression: To handle multicollinearity
Lasso Regression: For feature selection
Random Forest: To capture non-linear relationships
Gradient Boosting: Best-performing model
