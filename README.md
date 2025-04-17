# Diabetes Risk Prediction

## Overview

This project aims to predict whether a patient is at risk of developing diabetes using machine learning models. It involves exploratory data analysis (EDA), feature preprocessing, and the implementation of various classification algorithms. The project compares the performance of these models to identify the most effective one for diabetes prediction.

---

## Dataset Description

The dataset consists of diagnostic information for female patients, with 8 medical attributes:

- **Pregnancies**: Number of pregnancies
- **Glucose**: Plasma glucose concentration
- **BloodPressure**: Diastolic blood pressure (mm Hg)
- **SkinThickness**: Triceps skinfold thickness (mm)
- **Insulin**: 2-Hour serum insulin (mu U/ml)
- **BMI**: Body mass index (weight in kg/(height in m)^2)
- **DiabetesPedigreeFunction**: Likelihood of diabetes based on family history
- **Age**: Age in years
- **Outcome**: Class variable (1 = diabetic, 0 = non-diabetic)

---

## Exploratory Data Analysis (EDA)

- Identified relationships between features using **pairplots**, **boxplots**, and a **heatmap**.
- Analyzed class balance and feature distributions.
- Observed:
  - Higher glucose, BMI, and insulin levels tend to correlate with diabetes.
  - Diabetic patients typically have a higher number of pregnancies and older age groups.

---

## Preprocessing

- Missing values in features like `Insulin` and `SkinThickness` were handled by replacing zeroes with the column mean.
- Feature scaling was done using **MinMaxScaler** to normalize values between 0 and 1.
- Dataset was split into training and testing sets (80:20 split).

---

## Model Training

The following classification algorithms were implemented:

- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Classifier (SVC)**
- **Decision Tree Classifier**
- **Random Forest Classifier**

---

## Evaluation Metrics

Each model was evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**

Performance was measured using classification reports and accuracy on the test set.

---

## Results

| Model                  | Accuracy |
|------------------------|----------|
| Logistic Regression    | ~0.79    |
| K-Nearest Neighbors    | ~0.74    |
| Support Vector Machine | ~0.76    |
| Decision Tree          | ~0.72    |
| Random Forest          | ~0.75    |

**Logistic Regression** gave the best results in terms of accuracy and interpretability.

---

## Conclusion

This project demonstrates a complete machine learning pipeline for diabetes risk classification — from EDA and preprocessing to model training and evaluation. It highlights the role of medical features like glucose level, BMI, and insulin in predicting diabetes.

---

## Future Improvements

- Apply cross-validation for more robust performance.
- Use techniques like **SMOTE** to address data imbalance.
- Try advanced models like XGBoost or neural networks.
- Perform feature selection to improve efficiency.
