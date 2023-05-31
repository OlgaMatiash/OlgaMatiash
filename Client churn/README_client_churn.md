# Customer Churn Prediction Project

This project aims to predict customer churn in a telecommunications company. It utilizes machine learning algorithms, specifically the Random Forest Classifier, to build predictive models.

## Table of Contents

- [Project Overview](#project-overview)
- [Data](#data)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

Customer churn, or the loss of customers, is a critical issue for businesses. The goal of this project is to develop a predictive model that can accurately identify customers who are likely to churn, enabling the company to take proactive measures to retain them.

The project involves several stages, including data preprocessing, exploratory data analysis, model training, hyperparameter tuning, and evaluation.

## Data

The dataset used for this project contains information about customer attributes, usage patterns, and churn status. It includes features such as customer demographics, service subscription details, call duration, and payment information.

## Dependencies

The following dependencies are required to run the project:

- Python (version X.X.X)
- Pandas (version X.X.X)
- NumPy (version X.X.X)
- Scikit-learn (version X.X.X)
- Matplotlib (version X.X.X)
- Seaborn (version X.X.X)

## Installation

1. Clone the repository: `git clone https://github.com/your-username/customer-churn-prediction.git`
2. Navigate to the project directory: `cd customer-churn-prediction`
3. Install the required dependencies: `pip install -r requirements.txt`

## Usage

1. Prepare the dataset by placing it in the `data` directory.
2. Open the Jupyter Notebook: `jupyter notebook churn_prediction.ipynb`
3. Execute each cell in the notebook to run the code and reproduce the results.

## Results

The project achieves the following results:

- The best-performing model is the Random Forest Classifier with 30 trees, achieving an F1 score of 0.56 on the validation dataset.
- After addressing class imbalance using upsampling, the Random Forest Classifier with the best hyperparameters achieves an F1 score of 0.57 and an AUC-ROC of 0.83 on the validation dataset.
- The final model is selected as the Random Forest Classifier with 30 trees, before addressing class imbalance, which achieves an F1 score of 0.56 on the validation dataset.

## Contributing

Contributions to this project are welcome. Feel free to open issues and submit pull requests to suggest improvements or add new features.

## License

This project is licensed under the [MIT License](LICENSE).

