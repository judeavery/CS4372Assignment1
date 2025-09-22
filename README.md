# CS4372 Assignment 1: Bike Sharing Linear Regression Project

## Overview
This project analyzes bike rental data to **predict the total number of bikes rented (`cnt`)** using two regression models:

1. **Stochastic Gradient Descent (SGDRegressor)** – A machine learning algorithm for linear regression with iterative optimization.
2. **Ordinary Least Squares (OLS)** – A traditional statistical regression model.

The project involves **data cleaning, preprocessing, feature analysis, model training, and result interpretation**.

---

## Dataset
The dataset is from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset).

There are two main files:

| File      | Description              |
|-----------|--------------------------|
| `day.csv` | Daily bike sharing data  |
| `hour.csv`| Hourly bike sharing data |

The datasets are stored in the `/data/` folder of this repository.

**Example public link for `day.csv`:**  


You can load the dataset directly into a notebook using:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/judeavery/CS4372Assignment1/main/data/day.csv"
df = pd.read_csv(url)
df.head()
```

CS4372Assignment1/
│
├── data/                <- Datasets
│   ├── day.csv
│   └── hour.csv
│
├── notebooks/           <- Google Colab/Jupyter notebooks
│   └── main_analysis.ipynb
│
├── plots/               <- Saved plots and visualizations
│
├── report/              <- Final report
│
├── README.md
└── requirements.txt

How to Run

Open the notebook in Google Colab:

Go to Colab → File → Open Notebook → GitHub

Paste this repository URL:

https://github.com/judeavery/CS4372Assignment1


Install dependencies:

pip install -r requirements.txt


Run the notebook step-by-step to reproduce the results.

Dependencies

Install required libraries with:

pip install -r requirements.txt


Libraries included:

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

Interpret model results and explain findings in a clear report.

Author

Jude Avery
University of Texas at Dallas


---

