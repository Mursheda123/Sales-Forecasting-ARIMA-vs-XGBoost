# Sales-Forecasting-ARIMA-vs-XGBoost
A comprehensive project on sales forecasting for strategic demand planning using ARIMA and XGBoost models. This comparative study explores the strengths and limitations of classical time series methods versus modern machine learning techniques using real-world retail sales data.

OVERVIEW
This project focuses on building predictive models to forecast daily sales using:

ARIMA (AutoRegressive Integrated Moving Average) — a classical time series model

XGBoost — a machine learning model leveraging lag features and time-based attributes

The objective is to compare both approaches for 30-day sales forecasting and evaluate their performance using error metrics like RMSE and MAE.

📄 Dataset

Source: Superstore-style retail dataset (order-level)

Fields: Order Date, Sales, Product, Region, etc.

Time Period: Up to 2018-12-12

Preprocessing: Missing value imputation, duplicate removal, feature engineering

 Techniques & Tools

Languages: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, XGBoost, statsmodels, scikit-learn

Modeling Steps:

Time-based feature extraction (month, weekday, weekend indicator)

Lag feature creation (previous 5 days' sales)

Stationarity check using Augmented Dickey-Fuller test

Model training and evaluation

Forecast visualization and comparison

🔢 Model Comparison

ARIMA

Model: ARIMA(2, 0, 2)

Strength: Interpretable, good for stationary univariate series

Weakness: Struggles with nonlinearities or external regressors

RMSE: ~2558.62

XGBoost

Input: Lagged features + date-based features

Strength: Adaptable to trends, nonlinearities, and exogenous variables

RMSE: ~466.06

 Key Insights

ARIMA gave stable forecasts but lacked adaptability

XGBoost captured complex patterns with engineered features

Business recommendation:

Use ARIMA for short-term, interpretable use cases

Use XGBoost for long-term, feature-rich, dynamic forecasting

📊 Visual Output

Time series trend plots

Sales distribution and boxplots

30-day forecast comparison chart: ARIMA vs XGBoost

📆 Future Scope

Integrate exogenous variables (promotions, holidays)

Experiment with LSTM/Prophet models

Build a dashboard for real-time forecasting

 How to Run

Clone the repository

Install dependencies from requirements.txt

Run PROJECT.BEAT.ipynb in Jupyter


