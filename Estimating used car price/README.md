# Used Car Price Estimation Project
## Introduction
A used car sales service is developing an application to attract new customers. The application will enable users to quickly determine the market value of their used car. This project involves building a model to predict the market value of used cars based on historical data that includes various features such as technical specifications, configurations, and prices of cars.

## Goals
The main goals of this project are as follows:

- Build a predictive model for determining the market value of used cars.
- Emphasize prediction quality, prediction speed, and training time.
- Perform exploratory data analysis to understand the dataset and identify patterns.
- Handle missing values, outliers, and uninformative features in the dataset.
- Encode categorical features to prepare the data for model training.
- Evaluate and compare the performance of different machine learning models.

## Data Overview

The dataset contains information about used cars, including the following columns:

- DateCrawled: Date the listing was downloaded from the database.
- Price: Car's price (target variable).
- VehicleType: Body type of the car.
- RegistrationYear: Year of car registration.
- Gearbox: Transmission type.
- Power: Engine power.
- Kilometer: Mileage (in km).
- RegistrationMonth: Month of car registration.
- FuelType: Fuel type.
- Brand: Car brand.
- Repaired: Whether the car was previously repaired.
- DateCreated: Date the listing was created.
- NumberOfPictures: Number of photos of the car.
- PostalCode: Postal code of the owner.
- LastSeen: Date of the last user activity.
## Project Steps
1. Exploratory Data Analysis (EDA)
Import necessary libraries (Pandas, Numpy, Matplotlib, Seaborn).
Load the dataset and examine its structure using data.info() and data.head().
Identify missing values in the dataset using data.isna().mean().
Visualize distributions and statistics of numerical features (e.g., Kilometer, Price) using histograms and box plots.
Explore categorical features (e.g., VehicleType, FuelType) using bar plots.
2. Data Preprocessing
Reset the index of the dataset using data.reset_index(drop=True, inplace=True).
Fill missing values in categorical columns with the value "unknown" using data=data.fillna('unknown').
Remove outliers in columns like "Kilometer" and "Price" based on appropriate cutoffs.
Filter and remove anomalies in the "RegistrationYear" column based on the last seen date.
Remove uninformative features like "NumberOfPictures," "DateCrawled," "DateCreated," and "LastSeen."
3. Feature Encoding
Use One Hot Encoding (OHE) for linear regression by encoding categorical features like "VehicleType," "Gearbox," "FuelType," "Brand," and "Repaired."
Prepare the training and testing datasets for linear regression using the transformed features.
4. Model Training and Evaluation
Train a Linear Regression model using the prepared dataset and evaluate its performance using cross-validation.
Train a Random Forest model using the original ordinal encoded dataset and optimize hyperparameters using GridSearchCV.
Train a LightGBM model using the original ordinal encoded dataset and optimize hyperparameters using GridSearchCV.
Train a CatBoost model using the original dataset, and cross-validate it to find optimal iterations.
Train another CatBoost model using GridSearchCV to fine-tune hyperparameters.
5. Model Comparison
Create a DataFrame to analyze and compare the performance of different models in terms of fit time, score time, and RMSE.
Visualize the performance of different models using bar plots.
6. Conclusion
Summarize the findings of the project, including the best-performing model and insights gained from data analysis and model evaluation.
Discuss the model's suitability for the application's requirements and the trade-offs between prediction quality, prediction speed, and training time.
## Conclusion
This README provides an overview of the Used Car Price Estimation project. The project involves performing exploratory data analysis, data preprocessing, feature encoding, model training, and evaluation to build a predictive model for determining the market value of used cars. The project emphasizes prediction quality, prediction speed, and training time. The best-performing model will be selected based on its RMSE score and other performance metrics, making it suitable for the used car sales service application's requirements.



