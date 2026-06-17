# project-06

# Student Mental Health and Academic Performance Analysis

## Project Overview

This project analyzes the relationships between student lifestyle, mental health, academic engagement, and academic performance in a hybrid learning environment. The dataset contains information from 500 university students, including demographic characteristics, study habits, mental health indicators, and CGPA.

The project focuses on two main objectives:

1. Predicting student mental health risk using classification models.
2. Predicting student academic performance (CGPA) using regression models.

---

## Dataset

The dataset includes variables related to:

* Demographics (Age, Gender, Year of Study, Major)
* Lifestyle Factors (Sleep Hours, Screen Time, Physical Activity)
* Mental Health Measures (PHQ-9, GAD-7, Perceived Stress Scale)
* Academic Behaviors (Study Hours, Attendance)
* Learning Experience (Online Learning Satisfaction)
* Financial Stress
* Academic Performance (CGPA)

Dataset Size: 500 records

---

## Methodology

### Data Preprocessing

* Removed Student ID from modeling.
* Handled missing values using median imputation where appropriate.
* Removed observations with missing target variables.
* Applied standardization to numerical features.
* Applied one-hot encoding to categorical variables.

### Mental Health Risk Classification

Target Variable:

* High Mental Health Risk

  * PHQ-9 ≥ 10 or GAD-7 ≥ 10

Models Evaluated:

* Logistic Regression
* Random Forest Classifier
* Gradient Boosting Classifier

Best Model:

* Logistic Regression

Performance:

* Accuracy: 0.80
* ROC-AUC: 0.90

### CGPA Prediction

Target Variable:

* CGPA

Models Evaluated:

* Ridge Regression
* Random Forest Regressor
* Gradient Boosting Regressor

Best Model:

* Ridge Regression

Performance:

* MAE: 0.252
* RMSE: 0.307
* R²: 0.336

---

## Key Findings

### Mental Health Risk

* Perceived stress was the strongest predictor of mental health risk.
* Higher physical activity was associated with lower mental health risk.
* Higher CGPA was associated with lower mental health risk.
* The model correctly identified approximately 87% of high-risk students.

### Academic Performance

* Weekly study hours and class attendance were the strongest positive predictors of CGPA.
* Higher anxiety levels were associated with lower academic performance.
* Sleep habits also showed a positive relationship with CGPA.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook / Quarto

---

## Conclusion

The results suggest that student mental health and academic performance are influenced by a combination of behavioral, psychological, and academic factors. Stress management, regular study habits, consistent class attendance, and healthy lifestyle behaviors appear to be important factors associated with student success in a hybrid learning environment.
