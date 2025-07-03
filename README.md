# Financial-Market-Prediction

This project builds a predictive model for **S&P 500 returns** using a combination of **technical indicators**, **macro-economic data**, and multiple machine learning algorithms. For the regression task, it employs **Linear Regression**, **XGBoost**, and a **Long Short-Term Memory** (LSTM).  For the classification task, it utilizes both a **Forward Neural Network**(FNN) and **Long Short-Term Memory** (LSTM) network.

## Regression Approach:



---

## Objective

Predict short-term daily returns of the S&P 500 index using both price-based indicators and macroeconomic variables, and evaluate multiple ML models for forecasting accuracy.

---

## Data Sources

- **S&P 500 Historical Data** via `yfinance`
- **Macroeconomic Indicators** via FRED API:
  - **GDP** (Quarterly)
  - **UNRATE** (Unemployment Rate)
  - **UMCSENT** (Consumer Sentiment Index)

---

## Feature Engineering

- **Lagged Returns**: `Lag1`, `Lag2`, `Lag3`
- **Technical Indicators** from `ta` library:
  - RSI (Relative Strength Index)
  - MACD (Moving Average Convergence Divergence)
  - ATR (Average True Range)
  - ADX (Average Directional Index)
- **Macroeconomic Features**:
  - GDP
  - Unemployment Rate
  - Consumer Sentiment

---

## Models Used
- `LinearRegression` (scikit-learn)
- `XGBoostRegressor` (XGBoost)
- `LSTM` Recurrent Neural Network (Keras)

---

## Evaluation Metrics

- **Mean Squared Error (MSE)**: Measures prediction error.
- **Directional Accuracy**: Percentage of times the model predicted the correct direction (up/down).

---

## Results Summary

Each model is evaluated on unseen test data. Comparison includes:
- **Actual vs Predicted Returns (plot)**
- **MSE and Accuracy** for all models

---

## Visualization

The final section of the notebook plots predictions from all models against actual returns for the last 500 trading days, providing a visual sense of how closely the models track market behavior.

---
