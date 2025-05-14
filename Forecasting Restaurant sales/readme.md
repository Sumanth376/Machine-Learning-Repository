# 📊 Forecasting Monthly Restaurant Sales Using Time Series Analysis

This project focuses on analyzing and forecasting monthly restaurant sales using advanced time series techniques. The goal is to accurately predict future sales, helping businesses make informed decisions regarding inventory, staffing, and marketing.

---

## 📁 Dataset Overview

The dataset (`Restaurant Sales.csv`) contains monthly sales data for a restaurant chain, covering:

- **Date** – Monthly timestamps (e.g., Jan-2010, Feb-2010)
- **Sales** – Monthly revenue in USD

It’s a univariate time series dataset, ideal for forecasting with models like ARIMA, SARIMA, Prophet, and XGBoost.

---

## 🛠️ Tools & Technologies Used

- Python
- Jupyter Notebook
- Pandas, NumPy
- Matplotlib, Seaborn (for visualizations)
- Statsmodels (ARIMA/SARIMA)
- Facebook Prophet
- XGBoost
- scikit-learn
- Mean Absolute Error (MAE), RMSE for evaluation

---

## 📈 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Visualized monthly sales trends
- Checked for seasonality, trends, and cyclic behavior
- Performed decomposition using `seasonal_decompose`

### 2. Data Preprocessing
- Converted `Date` to datetime and set as index
- Resampled data (if needed) to monthly frequency
- Handled any missing values

### 3. Model Building

#### 🧮 ARIMA (AutoRegressive Integrated Moving Average)
- Used ACF and PACF plots to identify p, d, q
- Performed stationarity check using Augmented Dickey-Fuller (ADF) test

#### 📉 SARIMA (Seasonal ARIMA)
- Accounted for seasonality in the data
- Tuned parameters for best AIC/BIC

#### 📅 Prophet (Facebook)
- Simple and intuitive model for seasonality
- Captures trends and holiday effects

#### 🚀 XGBoost Regressor
- Feature engineering: month, year, lag values
- Used gradient boosting on tabular time-series data

---

## 📊 Evaluation Metrics

| Model     | MAE        | RMSE       |
|-----------|------------|------------|
| ARIMA     | 1524.38    | 1731.45    |
| SARIMA    | 1450.22    | 1605.31    |
| Prophet   | 1379.89    | 1540.60    |
| XGBoost   | 1290.55    | 1495.18    |
