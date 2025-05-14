# 🏥 Insurance Charges Prediction Using Machine Learning

This project focuses on predicting medical insurance charges based on individual demographic and health information. By leveraging regression algorithms, the model aims to estimate insurance premiums with high accuracy.

---

## 📁 Dataset Overview

The dataset (`insurance.csv`) includes the following features:

| Feature       | Description                        |
|---------------|------------------------------------|
| age           | Age of the policyholder            |
| sex           | Gender                             |
| bmi           | Body Mass Index                    |
| children      | Number of dependents               |
| smoker        | Smoking status (yes/no)            |
| region        | Residential region in the US       |
| charges       | Medical insurance cost (target)    |

---

## 🛠️ Tools & Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Statsmodels
- Jupyter Notebook

---

## 🚀 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Visualized distributions of numerical features
- Checked correlation between variables and charges
- Observed strong relationship between **smoking**, **BMI**, **age**, and **charges**

### 2. Data Preprocessing
- Encoded categorical variables using Label Encoding / One-Hot Encoding
- Handled skewness and outliers in BMI and charges
- Normalized or scaled numerical features where needed

### 3. Feature Engineering
- Created interaction features (e.g., smoker\*age, bmi\*smoker)
- Converted children count into categorical labels (e.g., `Zero`, `One`, etc.)

### 4. Model Training

| Model              | Technique     |
|--------------------|---------------|
| Linear Regression  | Baseline model |
| Ridge & Lasso      | Regularization |
| Decision Tree      | Non-linear model |
| Random Forest      | Ensemble method |
| XGBoost Regressor  | Gradient boosting |

---

## 📊 Evaluation Metrics

| Model            | MAE     | RMSE    | R² Score |
|------------------|---------|---------|----------|
| Linear Regression| 4200    | 6100    | 0.76     |
| Random Forest    | 2600    | 3700    | 0.89     |
| XGBoost          | 2400    | 3500    | 0.91     |

➡️ **XGBoost Regressor** gave the most accurate predictions.

---

## 📈 Visual Results

- Feature importance analysis showed **smoker**, **age**, and **BMI** as the top predictors.
- Residual plots confirmed minimal overfitting for ensemble models.
- Correlation heatmaps and pairplots enhanced understanding of data.

---

## 🔍 Insights

- Smokers are charged significantly more.
