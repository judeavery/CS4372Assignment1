# CS4372 Assignment 1: Bike Sharing Linear Regression Project
Overview

This project predicts daily bike rental demand using historical data from the UCI Machine Learning Repository
.

Two regression models were built and compared:

Stochastic Gradient Descent (SGDRegressor) –
A machine learning algorithm for linear regression using iterative optimization.

Ordinary Least Squares (OLS) –
A traditional statistical regression model with interpretable coefficients and diagnostics.

The project includes:

Data cleaning and preprocessing

Feature engineering and encoding

Model training and evaluation

Visualization of results and interpretation

A final written report with conclusions and insights

Dataset

The dataset consists of two main files:

File	Description
day.csv	Daily bike sharing data – used for this project
hour.csv	Hourly bike sharing data – not used in this project

These files are stored in the /data/ folder of this repository.

Load the dataset directly into a notebook:

import pandas as pd

url = "https://raw.githubusercontent.com/judeavery/CS4372Assignment1/main/data/day.csv"
df = pd.read_csv(url)
df.head()

Folder Structure
CS4372Assignment1/
│
├── data/            # Dataset files
│   ├── day.csv
│   └── hour.csv
│
├── notebooks/       # Jupyter/Colab notebooks
│   └── final_notebook.ipynb
│
├── plots/           # Saved plots and visualizations
│   ├── actual_vs_predicted.png
│   ├── residuals_vs_predicted.png
│   ├── qq_plot.png
│   ├── mse_comparison.png
│   └── r2_comparison.png
│
├── report/          # Final report (PDF)
│   └── Bike_Sharing_Demand_Prediction.pdf
│
├── requirements.txt # Python dependencies
└── README.md        # Project documentation

How to Run
1. Open Notebook in Google Colab

Go to Google Colab
.

File → Open Notebook → GitHub.

Paste this repository URL:

https://github.com/judeavery/CS4372Assignment1


Open final_notebook.ipynb under /notebooks/.

2. Install Dependencies

Install the required libraries:

pip install -r requirements.txt


Dependencies:

pandas

numpy

matplotlib

seaborn

scikit-learn

statsmodels

Project Goal

The purpose of this assignment is to:

Understand and clean real-world data.

Build two regression models and compare their performance.

Interpret model results and identify key predictors of bike demand.

Communicate findings through visualizations and a clear, structured report.

Methodology

Data Preprocessing:

Dropped irrelevant columns (instant, dteday, casual, registered).

Converted categorical variables to dummy variables:

season, mnth, weekday, weathersit

Standardized continuous variables:

temp, atemp, hum, windspeed

Split into 80% training and 20% testing sets.

Models Implemented:

Model	Description
SGDRegressor	Scikit-learn implementation of linear regression with gradient descent.
OLS Regression	Statsmodels implementation of ordinary least squares.
Results
Model	MSE	R² Score
SGDRegressor	646,328.54	0.8388
OLS Regression	634,351.36	0.8418

Interpretation:

OLS slightly outperformed SGD in both MSE and R², making it the preferred model.

Temperature and good weather conditions strongly increase rentals, while poor weather and high humidity decrease demand.

Key Visualizations
Actual vs Predicted (OLS)

Residuals vs Predicted (OLS)

Q-Q Plot of Residuals (OLS)

Final Report

The detailed analysis, interpretations, and conclusions can be found in the final report:

📄 Bike_Sharing_Demand_Prediction.pdf

How to Reproduce

Clone the repository:

git clone https://github.com/judeavery/CS4372Assignment1.git


Navigate to the project directory:

cd CS4372Assignment1


Install dependencies:

pip install -r requirements.txt


Open the notebook in Jupyter or Colab and run all cells.

Summary of Findings

OLS Regression achieved a slightly better fit and interpretability than SGD.

Temperature, year, and good weather are strong positive predictors of bike demand.

High humidity and bad weather significantly reduce rentals.

Bike usage increased from 2011 to 2012, suggesting growth in popularity.

Author

Jude Avery
University of Texas at Dallas

License

This project is for educational purposes only and is not intended for production use.


---

