# Cryptocurrency Price Prediction

This project demonstrates various techniques for predicting cryptocurrency prices using data analysis, machine learning, and deep learning models. The code is designed to work with historical price data of a given cryptocurrency (e.g., Bitcoin) and employs models such as Linear Regression, ARIMA, Prophet, and LSTM.

## Table of Contents
- [Requirements](#requirements)
- [Data Collection](#data-collection)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering](#feature-engineering)
- [Time Series Analysis](#time-series-analysis)
- [Predictive Modeling](#predictive-modeling)
- [Results](#results)
- [References](#references)

## Requirements
Ensure you have the following libraries installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow yfinance statsmodels prophet
```

## Data Collection
Historical data is collected from Yahoo Finance using the `yfinance` library. You can specify the cryptocurrency symbol, start date, and end date to fetch the data.

## Data Cleaning and Preprocessing
- Missing values are removed.
- Data is scaled to a range of 0 to 1 using `MinMaxScaler` for models requiring normalized input.

## Exploratory Data Analysis (EDA)
- Visualization of closing prices over time.
- Calculation of moving averages (MA50, MA200).

## Feature Engineering
- Creation of lag features to enhance predictive power.

## Time Series Analysis
- **ARIMA:** A statistical model applied to predict future prices based on historical trends.
- **Prophet:** A model by Facebook designed for forecasting time series data, which is particularly useful for capturing seasonality and trends.

## Predictive Modeling
- **Linear Regression:** Uses lag features and moving averages for prediction.
- **LSTM (Long Short-Term Memory):** A neural network model designed to work with sequential data, trained on sequences of past prices.

## Results
- Comparison of model performance using metrics like Mean Squared Error (MSE).
- Visualizations comparing predictions against actual values.

## References
- [yfinance Documentation](https://github.com/ranaroussi/yfinance)
- [Prophet Documentation](https://facebook.github.io/prophet/)
- [Statsmodels Documentation](https://www.statsmodels.org/)

