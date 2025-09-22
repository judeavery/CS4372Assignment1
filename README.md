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
