# Titanic Survival Prediction 🚢

## 📌 Project Overview

This project aims to predict whether a passenger survived the Titanic shipwreck using various features such as age, gender, passenger class, fare, etc. It uses supervised machine learning techniques and is a classic binary classification problem, based on the Titanic dataset made famous by Kaggle.

---

## 📊 Dataset Description

The dataset used is split into:

- **train.csv**: Contains the features and survival labels (used to train the model).
- **test.csv**: Contains features without the survival label (used for prediction).

### Key Columns:
- `PassengerId`: Unique ID for each passenger.
- `Survived`: Target variable (0 = No, 1 = Yes).
- `Pclass`: Passenger class (1st, 2nd, 3rd).
- `Name`, `Sex`, `Age`: Personal details.
- `SibSp`, `Parch`: Family relationships aboard.
- `Ticket`, `Fare`: Travel information.
- `Cabin`, `Embarked`: Additional ship details.

---

## 🧠 Steps Performed in Notebook

### 1. **Data Cleaning & Preprocessing**
- Handled missing values (`Age`, `Embarked`, `Cabin`).
- Converted categorical variables using label encoding or one-hot encoding.
- Feature engineering (e.g., extracted titles from names, grouped age ranges).

### 2. **Exploratory Data Analysis (EDA)**
- Visualized survival rates by gender, class, age group, and family size.
- Identified important features contributing to survival using plots.

### 3. **Model Building**
- Models trained: 
  - **Logistic Regression**
  - **Decision Tree**
  - **Random Forest**
  - **K-Nearest Neighbors**
  - **Support Vector Machine (SVM)**
- Used cross-validation and hyperparameter tuning for model optimization.

### 4. **Evaluation Metrics**
- Accuracy, Confusion Matrix, and ROC-AUC Score were used.
- Best model selected based on performance on validation set.

### 5. **Prediction**
- Final predictions made on `test.csv` using the best-performing model.

---

## ✅ Results & Insights

- **Sex** and **Pclass** were among the most influential features.
- Women and children had higher survival probabilities.
- Feature engineering and imputation of missing values significantly improved model accuracy.
- Achieved high accuracy with ensemble models like Random Forest.

---

## 🛠️ Technologies Used
- Python
- NumPy & Pandas
- Matplotlib & Seaborn
- Scikit-learn
- Jupyter Notebook
