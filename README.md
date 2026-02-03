# 🎓 Predicting Student Test Scores  
*Kaggle Playground Series – Regression*

## 📌 Overview
This project was developed as part of a **Kaggle Playground Series competition** focused on predicting **student exam scores** using academic, behavioral, and environmental features.

The goal was to build an accurate regression model while exploring how different factors contribute to student performance.  
Through experimentation, I learned an important lesson: **simple models can outperform complex ones when the data is well-understood**.

---

## 📊 Dataset Description
The dataset contains **630,000 rows** and **13 features**, combining numerical and categorical variables.

### Features
| Column | Description |
|------|------------|
| age | Student age |
| gender | Gender |
| course | Academic course |
| study_hours | Daily study time |
| class_attendance | Attendance percentage |
| internet_access | Internet availability |
| sleep_hours | Sleep duration |
| sleep_quality | Quality of sleep |
| study_method | Preferred study method |
| facility_rating | Study facility quality |
| exam_difficulty | Exam difficulty level |
| exam_score | **Target variable** |

**Data size:** ~62.5 MB  
**Types:** Numerical + Categorical (handled via preprocessing pipeline)

---

## 🔍 Exploratory Data Analysis (EDA)
- Analyzed feature distributions and correlations
- Identified which variables contribute meaningfully to exam score prediction
- Removed or deprioritized weak or redundant signals
- Gained insights into student behavior and performance patterns

---

## 🧠 Modeling Approach
I experimented with multiple machine learning models:

- Linear Regression ✅
- Random Forest Regressor
- XGBoost
- Neural Networks

Despite trying more complex models, **Linear Regression consistently performed better**, demonstrating:
> *The power of simple models when features are well-engineered.*

---

## ⚙️ Machine Learning Pipeline
A complete **scikit-learn Pipeline** was built to ensure clean and reproducible training:

- **Numerical features:** StandardScaler
- **Categorical features:** OneHotEncoder
- **Model:** Linear Regression
- **Cross-validation:** 5-fold CV

### 📈 Performance
