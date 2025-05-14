# 🧑‍💼 Employee Treatment Prediction

## 📌 Project Overview

This project aims to build a machine learning model that predicts whether an employee feels fairly treated at the workplace. The goal is to help HR departments proactively address issues by identifying at-risk employees through patterns in historical data.

---

## 📊 Dataset Description

The dataset contains demographic, professional, and behavioral attributes of employees. It is split into training and testing datasets.

- **Training Set:** 1048 records with 28 features  
- **Testing Set:** 210 records with 27 features  
- **Target Variable:** `treatment_flag` (1 = feels treated fairly, 0 = does not)

### 🔑 Key Features
- Demographics: `gender`, `dob`, `city`, `state`, `zip`  
- Job details: `job`, `company`, `hire_date`, `last_review`, `experience`  
- Work metrics: `avg_monthly_hours`, `last_evaluation`, `salary`, `number_project`  
- Behavioral data: `work_accident`, `promotion_last_5years`, `left_company`

---

## ⚙️ Project Workflow

### 1. **Data Preprocessing**
- Loaded and combined train/test datasets for uniform preprocessing  
- Handled missing values and anomalies  
- Converted date fields and extracted age-related features  
- Scaled features using **MinMaxScaler**

### 2. **Feature Engineering**
- Created derived metrics like:
  - Employee tenure
  - Age from date of birth
- Encoded categorical variables

### 3. **Feature Selection**
- Used **Boruta** algorithm to select top predictive features

### 4. **Model Building**
- Trained and compared several classifiers:
  - **Logistic Regression**
  - **Decision Tree**
  - **Random Forest**
  - **XGBoost**

### 5. **Model Evaluation**
- Used:
  - **Accuracy**
  - **Cross-validation score**
  - **Classification report**  
- Analyzed feature importance and confusion matrix

---

## 🧠 Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn, Plotly)  
- Scikit-learn (Modeling and preprocessing)  
- BorutaPy (Feature selection)  
- XGBoost (Ensemble modeling)  
- Jupyter Notebook (Development environment)

---

## ✅ Outcomes

- Built a classification model capable of predicting employee treatment perception  
- Identified key factors affecting employee satisfaction  
- Delivered insights to guide HR decisions for better retention and engagement strategies
