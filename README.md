
# 🧠 Machine Learning Projects — Skillfied Mentor Internship

> Projects completed during my Data Science & Machine Learning internship at **Skillfied Mentor**.  
> This repository contains end-to-end ML pipelines covering EDA, preprocessing, modeling, and evaluation.

---


# Project 1 — Bank Marketing Data Analysis

## Overview
Analysis of a bank's telemarketing campaign dataset to understand customer behavior and predict whether a client will subscribe to a **term deposit**.

### 📊 Dataset
| Property | Value |
|----------|-------|
| Rows | 41,188 |
| Features | 21 |
| Target Column | `y` (yes / no) |
| Class Distribution | No: 36,548 (88.7%) · Yes: 4,640 (11.3%) |

**Key Features:** age, job, marital, education, contact, duration, campaign, poutcome, emp.var.rate, euribor3m


## Bank_Marketing_Inspection_test.ipynb — Data Inspection
- Dataset loading and structure review
- Missing value check
- Summary statistics
- Target variable distribution plot
- Correlation heatmap for numerical features

## Advance_Bank_Term_Deposit.ipynb — Advanced Analysis & Modeling
- **Customer Demographics Analysis** — Age distribution, job category breakdown
- **Campaign Effectiveness** — Contact method vs subscription, number of contacts analysis
- **Balance & Duration Trends** — Average call duration by subscription outcome
- **Correlation Heatmap** — Relationships between numerical variables
- **Predictive Modeling** — Logistic Regression with one-hot encoding
- **Feature Importance** — Top predictors for term deposit subscription

##  Tech Stack
python
pandas · matplotlib · seaborn · scikit-learn (LogisticRegression, train_test_split)


### 📈 Key Findings
- Cellular contact method has higher subscription rates than telephone
- Longer call duration strongly correlates with successful subscriptions
- Certain job categories (management, retired) show higher subscription likelihood
- Logistic Regression identifies `duration`, `poutcome_success`, and `euribor3m` as top predictors

---

# Project 2 — Colorectal Cancer Risk & Survival Prediction

## Overview
A classification project to predict the **survival status** of colorectal cancer patients based on demographics, medical history, lifestyle factors, and treatment details.

### 📊 Dataset
| Property | Value |
|----------|-------|
| Rows | 89,945 |
| Features | 30 |
| Target Column | `Survival_Status` (Survived / Deceased) |
| Class Distribution | Survived: 67,341 (74.9%) · Deceased: 22,604 (25.1%) |

**Key Features:** Age, Gender, Stage_at_Diagnosis, Tumor_Aggressiveness, Chemotherapy_Received, Surgery_Received, Smoking_Status, BMI, Family_History, Screening_Regularity

## colorectal_cancer_prediction_test.ipynb

#### Step-by-step Pipeline:
1. **Data Loading & Exploration** — Shape, dtypes, first look
2. **EDA** — Survival status distribution, recurrence patterns, correlation heatmap
3. **Data Preprocessing**
   - Dropped irrelevant columns: `Patient_ID`, `Recurrence`, `Time_to_Recurrence`
   - Label Encoding for all categorical variables
   - StandardScaler for feature normalization
4. **Train-Test Split** — 80% train / 20% test (`random_state=42`)
5. **Model Training** — Logistic Regression
6. **Evaluation**
   - Accuracy Score
   - Classification Report (Precision, Recall, F1)
   - Confusion Matrix heatmap

### Tech Stack
python
pandas · numpy · seaborn · matplotlib
scikit-learn (LogisticRegression, LabelEncoder, StandardScaler, train_test_split, classification_report, confusion_matrix)


### 📈 Key Findings
- Stage at diagnosis and tumor aggressiveness are critical survival predictors
- Patients who received surgery and chemotherapy show higher survival rates
- Screening regularity and colonoscopy access positively impact early detection and survival
- Logistic Regression provides a solid baseline for clinical prediction
---

## 🧰 Libraries Used

| Library | Purpose |
|---------|---------|
| pandas | Data loading and manipulation |
| numpy | Numerical operations |
| matplotlib | Data visualization |
| seaborn | Statistical plots and heatmaps |
| scikit-learn | ML models, preprocessing, evaluation |
| jupyter | Interactive notebook environment |

---

## Internship Details

| | |
|--|--|
| **Company** | Skillfied Mentor |
| **Domain** | Data Science & Machine Learning |
| **Projects** | Bank Marketing Analysis · Colorectal Cancer Prediction |
| **Skills Gained** | EDA · Feature Engineering · Classification · Model Evaluation |

---

## 📄 License

This repository is for educational and portfolio purposes only.  
Datasets are used solely for learning and non-commercial analysis.

---

 *This repository is submitted as part of my Data Analyst Internship at SkillFied Mentor.*
