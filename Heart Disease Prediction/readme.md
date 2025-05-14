# ❤️ Heart Disease Prediction Using Decision Tree

This project focuses on building a machine learning model to **predict the presence of heart disease** in a patient based on various health-related attributes. We employ classification algorithms, particularly the **Decision Tree Classifier**, to assist in medical diagnostics and early risk detection.

---

## 📊 Dataset Overview

The dataset (`heart-disease.csv`) contains 14 attributes related to patient health and lifestyle:

| Feature           | Description                                               |
|------------------|-----------------------------------------------------------|
| age              | Age of the patient                                        |
| sex              | 1 = male, 0 = female                                      |
| cp               | Chest pain type (0–3)                                     |
| trestbps         | Resting blood pressure (in mm Hg)                         |
| chol             | Serum cholesterol (mg/dl)                                 |
| fbs              | Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)     |
| restecg          | Resting ECG results (0–2)                                 |
| thalach          | Maximum heart rate achieved                               |
| exang            | Exercise induced angina (1 = yes, 0 = no)                 |
| oldpeak          | ST depression induced by exercise                         |
| slope            | Slope of the peak exercise ST segment                     |
| ca               | Number of major vessels colored by fluoroscopy (0–3)      |
| thal             | 3 = normal, 6 = fixed defect, 7 = reversible defect        |
| target           | 1 = disease, 0 = no disease (label column)                |

---

## 🔧 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🚀 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Checked for missing values and feature distributions
- Analyzed correlations between predictors and the target
- Visualized risk patterns using histograms and heatmaps

### 2. Data Preprocessing
- Handled categorical features (e.g., `cp`, `thal`, `slope`) via encoding
- Standardized numerical variables for better model performance
- Split dataset into **training** and **testing** sets (80/20)

### 3. Model Training
- Trained a **Decision Tree Classifier**
- Tuned hyperparameters (max depth, splitting criteria)
- Compared accuracy against other models like Logistic Regression and Random Forest

---

## 📈 Evaluation Metrics

| Metric          | Value     |
|-----------------|-----------|
| Accuracy        | ~85%      |
| Precision       | ~86%      |
| Recall          | ~84%      |
| F1 Score        | ~85%      |

Confusion matrix and classification report were also generated for detailed evaluation.

---

## 🧠 Model Insights

- **Chest pain type** and **thalassemia** showed strong influence on heart disease prediction.
- Decision Tree models are interpretable and visually explainable.
- Feature importance plot shows top predictors such as `cp`, `thal`, `oldpeak`, and `ca`.

---

## 📁 Project Structure

├── heart-disease.csv # Dataset
├── Predicting Heart Disease using Decision Tree.ipynb # Jupyter Notebook
├── README.md # Documentation

yaml
Copy
Edit

---

## 🔍 Key Takeaways

- Predictive models can significantly support early detection of heart disease.
- Decision Trees are great for interpretable healthcare applications.
- Proper feature engineering and scaling are essential in classification tasks.
