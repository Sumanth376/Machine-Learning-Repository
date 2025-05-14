# 🎯 Predicting the Status of the Interview — Skillenza Hackathon

This machine learning project aims to **predict the outcome of job interviews** based on applicant information and feedback. It was originally part of a **Skillenza Hackathon** challenge, and the goal is to classify whether a candidate will be **selected** or **rejected** based on various attributes captured during the interview process.

---

## 📁 Dataset Overview

The dataset includes various candidate features collected during interviews. These features reflect candidate background, performance, and evaluator feedback.

### Sample Features:
| Feature                  | Description                                                 |
|--------------------------|-------------------------------------------------------------|
| Candidate_ID             | Unique ID of the candidate                                  |
| Candidate_Name           | Name of the candidate                                       |
| Gender                   | Gender of the candidate                                     |
| Candidate_Location       | City/location of the candidate                              |
| Interview_Type           | Type of interview (e.g., Telephonic, F2F, etc.)             |
| Interview_Rating         | Performance rating (0–5 scale)                              |
| Qualification            | Academic qualification (e.g., B.Tech, MBA)                  |
| Total_Experience         | Total years of experience                                   |
| Relevant_Experience      | Relevant years of experience for the job                    |
| Communication_Skill      | Verbal communication skill rating                           |
| Domain_Knowledge         | Domain knowledge evaluation rating                          |
| Decision                 | Final interview outcome (Selected / Rejected)               |

---

## 🚀 Project Objectives

- Clean and preprocess messy real-world interview data
- Perform Exploratory Data Analysis (EDA)
- Build classification models to predict interview results
- Evaluate models using metrics such as accuracy and F1-score

---

## 🔧 Technologies Used

- Python (Pandas, NumPy)
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 📊 Exploratory Data Analysis (EDA)

- Checked and handled missing values in `Interview_Rating`, `Domain_Knowledge`
- Analyzed the impact of features like experience and skills on the final decision
- Visualized class imbalance between "Selected" and "Rejected" candidates
- Discovered trends based on gender, experience, and communication skills

---

## 🛠️ Data Preprocessing

- Encoded categorical variables (`Gender`, `Qualification`, etc.) using Label Encoding
- Handled missing values with imputation strategies
- Converted ratings to numerical format
- Addressed class imbalance using SMOTE (Synthetic Minority Oversampling Technique)

---

## 🤖 Model Development

### Models Used:
- **Logistic Regression**
- **Random Forest Classifier**
- **Decision Tree**
- **Support Vector Machine (SVM)**

### Model Metrics:
| Model                | Accuracy | F1 Score |
|----------------------|----------|----------|
| Logistic Regression  | ~83%     | ~81%     |
| Random Forest        | ~88%     | ~86%     |
| Decision Tree        | ~85%     | ~83%     |

---

## 📈 Results & Insights

- **Communication skills**, **domain knowledge**, and **relevant experience** were among the most influential features.
- Random Forest outperformed other models in prediction accuracy and generalization.
- Class imbalance was successfully handled using SMOTE.
