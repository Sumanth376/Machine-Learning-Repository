# 🔐 Credit Card Fraud Detection

## 📌 Project Overview

Credit card fraud poses a major risk to both financial institutions and cardholders, resulting in significant financial and reputational damage. This project leverages machine learning techniques to build a robust fraud detection model capable of identifying fraudulent transactions with a high level of accuracy.

---

## 📊 Dataset Description

The dataset consists of simulated credit card transactions from **January 1, 2019, to December 31, 2020**, including both legitimate and fraudulent records.

- **Volume:** ~1.3 million transactions  
- **Customers:** 1000  
- **Merchants:** 800  
- **Features:** 21 including demographics, location, and transaction details

### 🔑 Key Features
- `trans_date_trans_time`: Transaction date and time  
- `cc_num`: Credit card number (anonymized)  
- `merchant`: Merchant name or ID  
- `category`: Transaction category (e.g., retail, travel)  
- `amt`: Transaction amount  
- `gender`, `job`, `dob`, `city`, `state`, `zip`, etc.  
- `is_fraud`: Target variable (1 = Fraudulent, 0 = Genuine)  

Additional features include geographic coordinates (`lat`, `long`, `merch_lat`, `merch_long`) to support location-based fraud detection analysis.

---

## ⚙️ Project Workflow

### 1. **Data Preprocessing**
- Loaded CSV data and handled missing values  
- Converted date columns and engineered time-based features  
- Scaled features using MinMaxScaler  

### 2. **Handling Class Imbalance**
- Applied **SMOTE** and **undersampling** techniques  
- Evaluated impact through visualization and metrics  

### 3. **Feature Selection**
- Implemented **Boruta** algorithm to identify top features  

### 4. **Model Building**
- Trained and compared:
  - **Logistic Regression**
  - **Decision Tree**
  - **Random Forest**
  - **XGBoost**

### 5. **Evaluation Metrics**
- Emphasized:
  - **Recall** (minimize false negatives)  
  - **Precision**  
  - **F1-Score**  
  - **ROC-AUC Score**  
- Plotted ROC curves for visual insights

---

## 🧠 Technologies Used

- Python (Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Plotly)  
- Imbalanced-learn (SMOTE)  
- BorutaPy (Feature Selection)  
- XGBoost (Modeling)  
- Jupyter Notebook  

---

## ✅ Outcomes

- Achieved strong recall and ROC-AUC on test set  
- Demonstrated the impact of resampling and feature selection  
- Built a scalable and interpretable fraud detection pipeline  
