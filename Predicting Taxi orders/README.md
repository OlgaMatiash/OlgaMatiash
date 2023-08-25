# Taxi Booking Prediction Project

This repository contains the code and documentation for a project aimed at predicting the number of taxi bookings for the next hour using historical airport taxi booking data. The project includes data preprocessing, exploratory data analysis, feature engineering, model selection, tuning, and testing.

## Dataset

The dataset used for this project contains approximately 26.5 thousand records of taxi bookings at airports. The data includes the number of bookings recorded every 10 minutes from March 2018 to August 2018. The dataset was resampled to an hourly interval for analysis and modeling.

## Project Overview

1. **Data Preprocessing**: The dataset underwent preprocessing steps, including handling missing values, resampling, and extracting relevant features from timestamps.

2. **Exploratory Data Analysis (EDA)**: EDA was performed to understand the data distribution, trends, and seasonality. Notable findings include a trend of increasing bookings from March to August and daily seasonality.

3. **Feature Engineering**: Features such as day of the week and hour were extracted from timestamps. Lag and rolling mean features were also created to capture temporal patterns.

4. **Model Selection**: Four models were considered: Linear Regression, LightGBM, CatBoost, and Random Forest. A grid search was conducted to tune hyperparameters for each model.

5. **Model Evaluation**: The models were evaluated using cross-validation, and the best-performing model was selected based on the root mean squared error (RMSE).

6. **Testing**: The selected model, LightGBM, was tested on a separate test set. The RMSE achieved was 42.39, meeting the project's requirements.

## Getting Started

1. Clone this repository:

   ```
   git clone https://github.com/your-username/taxi-booking-prediction.git
   cd taxi-booking-prediction
Install the required packages using the provided requirements.txt file:

```
pip install -r requirements.txt
```
Run the Jupyter Notebook files in the notebooks directory to follow the project's steps.


## Project Structure

- `data/`: Contains the dataset files.
- `notebooks/`: Jupyter Notebook files detailing the project's steps.
- `README.md`: This file, providing an overview of the project.
- `requirements.txt`: List of required packages for reproducing the environment.


