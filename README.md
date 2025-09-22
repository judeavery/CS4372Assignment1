# CS4372 Assignment 1: Bike Sharing Linear Regression Project
Overview

This project predicts daily bike rental demand using historical data from the UCI Machine Learning Repository

Two regression models were built and compared:

Stochastic Gradient Descent (SGDRegressor) –
A machine learning algorithm for linear regression using iterative optimization.

Ordinary Least Squares (OLS) –
A traditional statistical regression model with interpretable coefficients and diagnostics.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The project includes:

Data cleaning and preprocessing

Feature engineering and encoding

Model training and evaluation

Visualization of results and interpretation

A final written report with conclusions and insights

Dataset
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
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


## How to Run
1. Open Notebook in Google Colab

Go to Google Colab

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

run all cells in order
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

How to Reproduce

Clone the repository:

git clone https://github.com/judeavery/CS4372Assignment1.git


Navigate to the project directory:

cd CS4372Assignment1

Install dependencies:

pip install -r requirements.txt

Open the notebook in Jupyter or Colab and run all cells.

Author

Jude Avery
University of Texas at Dallas

License

This project is for educational purposes only and is not intended for production use.
