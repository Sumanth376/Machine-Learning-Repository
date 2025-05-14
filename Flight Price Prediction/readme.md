# ✈️ Flight Price Prediction using Machine Learning

This project focuses on building a machine learning model that predicts flight ticket prices based on several features such as airline, source, destination, departure time, number of stops, and more. The goal is to enable travel agencies or users to estimate the cost of a flight ticket and make informed booking decisions.

---

## 📁 Dataset Overview

The dataset contains details about past flight bookings, including:

- **Airline** – Airline company (e.g., Indigo, Air India)
- **Date_of_Journey** – Date of the journey
- **Source & Destination** – Cities of departure and arrival
- **Route** – Path taken by the flight
- **Dep_Time & Arrival_Time** – Departure and arrival timestamps
- **Duration** – Total time of the journey
- **Total_Stops** – Number of stops during the journey
- **Additional_Info** – Any other remarks (e.g., no info, in-flight meal not included)
- **Price** – Target variable (ticket price in INR)

---

## 🛠️ Tools & Technologies

- Python
- Jupyter Notebook
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (train_test_split, LinearRegression, RandomForest, etc.)
- Feature Engineering & Encoding
- GridSearchCV for Hyperparameter Tuning

---

## 📈 Project Workflow

1. **Data Cleaning & Preprocessing**
   - Converted `Date_of_Journey`, `Dep_Time`, and `Arrival_Time` to datetime format
   - Extracted day, month, hour, minute for modeling
   - Processed `Duration` field and removed inconsistencies
   - Handled null values and duplicates

2. **Feature Engineering**
   - Categorical features were encoded using one-hot encoding and label encoding
   - `Total_Stops`, `Airline`, `Route`, etc., were transformed for modeling
   - Dropped irrelevant columns like `Route`, `Additional_Info`

3. **Model Building**
   - Trained multiple regression models:
     - Linear Regression
     - Decision Tree Regressor
     - Random Forest Regressor (best performer)
   - Evaluated models using:
     - R² Score
     - Mean Absolute Error (MAE)
     - Root Mean Squared Error (RMSE)

4. **Hyperparameter Tuning**
   - Used GridSearchCV to optimize Random Forest Regressor
   - Final model chosen based on best cross-validation score

5. **Prediction**
   - Created a function to predict flight prices for new user input

---

## ✅ Results

- The best model achieved an **R² Score > 0.9** on training data.
- Successfully predicted flight prices based on user-entered features.
- Feature importance showed:
  - **Airline**, **Total_Stops**, and **Duration** were most influential in determining price.

---

## 📊 Visualizations

- Heatmap of correlation between features
- Count plots for airlines and total stops
- Price distribution plots for each category
