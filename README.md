# Diabetes Risk Prediction

## Machine Learning Major Project

A machine learning project that predicts diabetes risk and helps prioritize patients for further testing when healthcare facilities have limited testing capacity.

## 1. Project Overview

This project uses machine learning techniques to identify patients who may be at higher risk of diabetes based on medical measurements. It focuses on prioritizing approximately 30% of patients for further testing.

## 2. Problem Statement

A rural health clinic has limited laboratory testing capacity and can test only around 30% of daily walk-in patients. This project develops a data-driven approach to rank patients according to predicted diabetes risk while considering false alarms.

## 3. Project Objectives

- Load and inspect the diabetes dataset.
- Handle zero-coded missing medical values.
- Apply feature scaling using StandardScaler.
- Split the dataset using stratification.
- Train and compare machine learning models.
- Evaluate model performance using classification metrics.
- Apply threshold tuning and top-30% patient selection.
- Save, reload and test the selected model.

## 4. Dataset Description

**Dataset:** Pima Indians Diabetes Database

The dataset contains 768 records and 9 columns.

Features include:
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome

Outcome:
- 0 – Non-Diabetic
- 1 – Diabetic

## 5. Tools and Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

## 6. Machine Learning Models

The following algorithms were trained and compared:

1. K-Nearest Neighbors (KNN)
2. Logistic Regression
3. Decision Tree

## 7. Model Evaluation

The models were evaluated using accuracy, precision, recall and F1-score.

### Top-30% Patient Selection Results

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| KNN | 79.87% | 74.47% | 64.81% | 69.31% |
| Logistic Regression | 78.57% | 72.34% | 62.96% | 67.33% |
| Decision Tree | 77.27% | 70.21% | 61.11% | 65.35% |

**Selected Model:** K-Nearest Neighbors (KNN)

KNN achieved the highest F1-score in the top-30% comparison.

## 8. Model Saving and Testing

The selected KNN pipeline was saved using Joblib as:

`diabetes_knn_model.pkl`

The saved model was loaded and tested successfully.

## 9. Project Files

- `diabetes.csv` – Dataset
- `Diabetes_Risk_Prediction.ipynb` – Google Colab notebook
- `diabetes_risk_prediction.py` – Python source code
- `diabetes_knn_model.pkl` – Trained KNN model
- `Diabetes_Prediction_Results.csv` – Prediction results

## 10. Conclusion

This project demonstrates how machine learning can support diabetes risk prioritization when testing resources are limited. Among the three evaluated models, KNN achieved the highest F1-score in the top-30% comparison.

**Note:** This project is an academic screening and prioritization demonstration. It is not a medical diagnostic tool.

## 11. Author

**Name:** Deepak  
**Course:** Machine Learning  
**Project:** Major Project – Diabetes Risk Prediction
