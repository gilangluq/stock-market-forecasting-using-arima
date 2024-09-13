# Stock Market Forecasting using ARIMA

This repository presents a time series forecasting model using **ARIMA (AutoRegressive Integrated Moving Average)** to predict stock market prices based on historical price and volume data. The dataset used for this project is obtained from Kaggle and contains full historical daily price and volume data for all US-based stocks and ETFs trading on the NYSE, NASDAQ, and NYSE MKT, updated until **11/10/2017**.

---

## Overview

Stock market forecasting is a challenging task due to the stochastic nature of market prices. However, time series models such as ARIMA can provide insights into future price movements by analyzing historical trends and patterns. In this project, we utilize ARIMA for predicting stock prices using historical data.

The ARIMA model is widely used for financial market forecasting due to its ability to capture key elements of time series data like trend, seasonality, and noise. This repository provides a full pipeline from data preprocessing to model evaluation and prediction of future stock prices.

---

## Dataset

The dataset used in this project is obtained from **[Kaggle](https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs)** and provides:
- **Full historical daily price and volume data** for all US-based stocks and ETFs trading on NYSE, NASDAQ, and NYSE MKT.
- **Fields**: `Date`, `Open`, `High`, `Low`, `Close`, `Volume`, and `OpenInt` (Open Interest).
- **Format**: CSV files, updated until **11/10/2017**.

Make sure to download the dataset from Kaggle and place it in the appropriate directory as specified in the repository structure.

---

## Model Explanation

The **ARIMA (AutoRegressive Integrated Moving Average)** model is built in the following steps:
1. **Stationarity Check**: The data is tested for stationarity using methods such as the Augmented Dickey-Fuller (ADF) test.
2. **Differencing**: If the data is not stationary, differencing is applied to transform it into a stationary series.
3. **ARIMA Parameters**: The model parameters `(p, d, q)` are identified and tuned using grid search or the `auto_arima` function.
4. **Model Fitting**: The ARIMA model is fitted to the historical stock price data.
5. **Forecasting**: The model is used to generate future price forecasts, and predictions are compared to actual prices for validation.

---

## Results

- **Model Performance**: The model's performance is evaluated using metrics such as Mean Absolute Error (MAE) and Root Mean Square Error (RMSE).
- **Forecast Visualization**: Predictions of future stock prices are visualized using line plots, showing the actual vs. predicted prices.

---

