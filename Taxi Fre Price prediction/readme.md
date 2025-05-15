# 🚖 Taxi Fare Prediction Project

This project aims to predict the fare amount of New York City taxi rides using machine learning techniques. It involves cleaning and exploring a real-world dataset, performing feature engineering, training multiple regression models, and evaluating their performance. The dataset includes pickup and dropoff locations, datetime, and number of passengers.

---

## 📁 Project Structure

- `Taxi Fare Prediction By Jeevan Raj.ipynb` – Main notebook containing all steps from EDA to model building and evaluation.
- `TaxiFare.csv` – Dataset with NYC taxi trip records and corresponding fare amounts.

---

## 📊 Dataset Overview

The dataset includes the following columns:

- `pickup_datetime` – Date and time of the ride.
- `pickup_longitude` & `pickup_latitude` – Coordinates of the pickup location.
- `dropoff_longitude` & `dropoff_latitude` – Coordinates of the dropoff location.
- `passenger_count` – Number of passengers.
- `fare_amount` – Target variable to predict (fare in USD).

---

## 🔍 Exploratory Data Analysis (EDA)

Key steps in the EDA include:

- **Missing Value Treatment** – Removed rows with missing or invalid fare amounts and coordinates.
- **Outlier Detection** – Removed extreme fare amounts and unrealistic coordinates.
- **Date-Time Features** – Extracted hour, day, and weekday from the pickup timestamp.
- **Distance Feature** – Calculated Haversine distance between pickup and dropoff points.

---

## 🧪 Feature Engineering

- Converted `pickup_datetime` to datetime object and extracted relevant time features.
- Computed **Haversine Distance** as a new numerical feature.
- Removed outliers based on logical thresholds (e.g., number of passengers between 1 and 6).

---

## 🤖 Model Building

Several regression models were trained and compared:

- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **XGBoost Regressor**

Evaluation metrics used:

- **R² Score**
- **Root Mean Squared Error (RMSE)**

---

## 🏆 Best Model

- **Random Forest Regressor** performed the best among all models with a high R² score and lower RMSE.
- Model showed good generalization on test data after hyperparameter tuning.

---

## 📈 Results & Insights

- Trip **distance** and **time of day** had significant influence on fare.
- Fare prediction models can be highly effective with proper feature engineering and tuning.
- Random Forest provided a strong balance between performance and interpretability.

---

## 📌 Requirements

- Python 3.7+
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- xgboost
