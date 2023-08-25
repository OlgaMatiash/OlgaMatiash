# Gold Recovery Prediction Project
## Project Overview
This project focuses on predicting the gold recovery efficiency in the process of gold-bearing ore enrichment. The project involves data preprocessing, exploratory data analysis, model selection, and evaluation to develop a predictive model. The main goal is to identify the best-performing model that accurately predicts the gold recovery coefficient from the provided dataset.
Data
The dataset used in this project consists of several features related to the gold recovery process, including concentrations of different metals (Au, Ag, Pb) at various stages of purification. The dataset also contains the target variables 'rougher.output.recovery' and 'final.output.recovery', which represent the efficiency of gold enrichment. The dataset was provided in three parts: full, training, and testing datasets.

## Installation
Clone this repository to your local machine using:
```
git clone https://github.com/your-username/gold-recovery-prediction.git
```
Install the required Python packages by running:

```
pip install -r requirements.txt
```
## Usage

Navigate to the project directory:
```

cd gold-recovery-prediction
```

Run the Jupyter notebook:

```
jupyter notebook Gold_Recovery_Prediction.ipynb
```
Follow the instructions within the notebook to execute the data analysis and modeling steps.

## Data Preprocessing
In this section, the data is prepared for analysis. Steps include handling missing values, dealing with outliers, and formatting the data for further analysis.

## Exploratory Data Analysis (EDA)
Here, the concentration changes of metals (Au, Ag, Pb) at different stages of purification are analyzed. Box plots and visualizations are used to show the distribution of these concentrations. The distribution of raw ore particle sizes is also compared between the training and test datasets.

## Model Selection
Different machine learning models are trained, including Decision Trees, Random Forest, Linear Regression, and Gradient Boosting. Model hyperparameters are tuned to find the best combination for prediction.

## Model Evaluation
The models are evaluated using cross-validation techniques to calculate the symmetric mean absolute percentage error (sMAPE) on both the training and test datasets. The chosen model's performance is compared to that of a dummy regressor to assess its adequacy.

## Conclusion
The final selected model is the Gradient Boosting Regressor with a maximum depth of 1. This model achieved a final sMAPE of 9.30% on the test dataset, indicating its effectiveness in predicting the gold recovery coefficient.

## Contributing
Contributions to this project are welcome. Feel free to open an issue or submit a pull request.





