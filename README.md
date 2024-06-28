# FLIGHT-FARE-PREDITION-AND-ANALYTICS


## Project Overview
This project aims to predict flight fares using various machine learning models. By leveraging a dataset from Kaggle, the project focuses on exploring and preprocessing the data, feature engineering, model building, and evaluation. The main objective is to build an accurate flight fare prediction model to assist airlines and customers in understanding fare patterns and making informed decisions.


## Dataset
The dataset used in this project is taken from Kaggle and contains various features representing flight details such as airline, date of journey, source, destination, duration, and total stops. The dataset can be found [here](https://www.kaggle.com/nikhilmittal/flight-fare-prediction-mh).

## Data Preprocessing
- **Handling Missing Values**: Dropped rows with missing values.
- **Feature Engineering**: Extracted day and month from the date of journey, extracted hours and minutes from departure and arrival times, and transformed the duration column into hours and minutes.
- **Encoding Categorical Variables**: Applied one-hot encoding to nominal categorical features (Airline, Source, Destination) and label encoding to ordinal categorical features (Total_Stops).
- **Feature Scaling**: Used RobustScaler for feature scaling.

## Exploratory Data Analysis (EDA)
- Analyzed the distribution of flight prices.
- Identified top 10 aviation companies based on the number of flight tickets sold.
- Explored the relationship between different features and flight prices.

## Model Building
Various machine learning models were used to predict flight fares:
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **XGBoost Regressor**
- **Linear Regression**

## Model Evaluation
The models were evaluated using the following metrics:
- **R2 Score**
- **Adjusted R2 Score**
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**

The XGBoost Regressor with hyperparameter tuning provided the best results.

## Hyperparameter Tuning
Hyperparameter tuning was performed for the XGBoost Regressor using RandomizedSearchCV to optimize the model's performance.

## Results
The final XGBoost Regressor model demonstrated the following performance on the test set:
- **R2 Score**: 0.8605
- **Adjusted R2 Score**: 0.8602
- **MAE**: 1184.96
- **MSE**: 2975705.18
- **RMSE**: 1725.76



