# Stock Price Prediction (GOOGLE DEVELOPER GROUPS, IIT KANPUR)

This repository contains a comparative study and implementation of traditional statistical models and deep learning models for stock price forecasting. The project evaluates performance across multiple stocks using real-world data and standard evaluation metrics.

---

## 🎯 Objective

To analyze and compare the effectiveness of traditional time series forecasting models (ARIMA/SARIMA) and deep learning models (LSTM) in predicting stock closing prices.

---

## Approach

### Data Exploration & Preprocessing
- Collected historical stock price data for three publicly traded companies.
- Examined time series properties using:
  - **Rolling statistics** for trend detection
  - **Augmented Dickey-Fuller (ADF) test** for stationarity
  - **ACF and PACF plots** to identify autoregressive and moving average components
- Applied **differencing** techniques to eliminate non-stationarity where needed.

### Traditional Models
- Implemented **ARIMA** and **SARIMA** models using the `statsmodels` library.
- Used **Akaike Information Criterion (AIC)** for automated parameter selection.
- Fitted models separately for each stock and forecasted future prices.

### Deep Learning Model (LSTM)
- Scaled stock prices using `MinMaxScaler` for LSTM input compatibility.
- Used a **sliding window approach** to prepare sequences of past prices.
- Trained a **Long Short-Term Memory (LSTM)** neural network using `Keras`.
- Evaluated model using **Root Mean Squared Error (RMSE)** and **Mean Absolute Percentage Error (MAPE)**.

---

## 📊 Results

**LSTM consistently outperformed SARIMA**, showing better generalization and lower error metrics(RMSE and MAPE) on test data.

---

## 🛠 Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Statsmodels (ARIMA, SARIMA)
- Scikit-learn (Scaling, Evaluation Metrics)
- TensorFlow / Keras (LSTM)
- Google Collab

---
