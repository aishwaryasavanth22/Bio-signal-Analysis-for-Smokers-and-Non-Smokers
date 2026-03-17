# 🚬 Biological Analysis for Smokers and Non-Smokers Classification Using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-black?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?style=for-the-badge&logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge&logo=scikitlearn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-yellow?style=for-the-badge&logo=plotly)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-4C78A8?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📌 Project Overview

Smoking is one of the major public health concerns and is strongly associated with several health disorders, including cardiovascular disease, respiratory problems, and metabolic abnormalities.  
This project uses **biological and medical health indicators** to build a **machine learning classification system** that predicts whether a person is a **smoker** or **non-smoker**.

The main objective of this project is to analyze health-related bio-signals and develop predictive models that can accurately classify smoking behavior.

---

## 🎯 Problem Statement

Over the years, a company has collected a large amount of biological and medical information about individuals.  
Management wants to build an **intelligent system** that can determine the **presence or absence of smoking behavior** in a person using bio-signals.

This project solves that problem by applying **data analysis, feature selection, preprocessing, and machine learning classification algorithms**.

---

## 🗂️ Dataset Information

The dataset contains **55,692 rows** and **27 columns**.

### Target Variable
- **Smoking**
  - `0` → Non-Smoker
  - `1` → Smoker

### Features Included
- ID
- Gender
- Age
- Height (cm)
- Weight (kg)
- Waist (cm)
- Eyesight (Left / Right)
- Hearing (Left / Right)
- Haemoglobin
- Systolic
- Relaxation
- Fasting Blood Sugar
- Cholesterol
- Triglyceride
- HDL
- LDL
- Urine Protein
- Serum Creatinine
- AST
- ALT
- Gtp
- Oral
- Dental Caries
- Tartar
- Smoking

---

## 📖 Dataset Description

| Feature | Description |
|--------|-------------|
| ID | Index / Unique identifier |
| Gender | Gender of the person |
| Age | Age of the person |
| Height(cm) | Height in centimeters |
| Weight(kg) | Weight in kilograms |
| Waist(cm) | Waist circumference |
| Eyesight(left/right) | Eyesight values for both eyes |
| Hearing(left/right) | Hearing status for both ears |
| Systolic | Upper blood pressure |
| Relaxation | Lower blood pressure |
| Fasting Blood Sugar | Blood sugar test result |
| Cholesterol | Total cholesterol |
| Triglyceride | Lipid found in blood |
| HDL | High-density lipoprotein |
| LDL | Low-density lipoprotein |
| Haemoglobin | Oxygen-carrying protein in blood |
| Urine Protein | Protein present in urine |
| Serum Creatinine | Kidney function indicator |
| AST / ALT | Liver enzyme indicators |
| Gtp | Gamma-glutamyl transferase |
| Oral | Oral examination status |
| Dental Caries | Tooth decay status |
| Tartar | Tartar status |
| Smoking | Target label |

---


## ⚙️ Project Workflow

### 1. Import Necessary Libraries
The following libraries were used:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `warnings`
- `scikit-learn`

### 2. Data Loading and Inspection
Performed:
- Displayed top 5 rows
- Checked dataset shape
- Examined column names
- Inspected data types using `.info()`
- Generated statistical summary using `.describe()`

### 3. Data Cleaning and Preprocessing
Performed:
- Checked missing values
- Checked duplicate records
- Validated data types

### 4. Exploratory Data Analysis (EDA)
Performed:

- Smoking vs non-smoking distribution analysis

![percentage of Smoker Vs Non-Smoker](https://github.com/aishwaryasavanth22/Bio-signal-Analysis-for-Smokers-and-Non-Smokers/blob/22f3dce0eed0132b8273341265131666ba1ce8f6/Visualizations/Percentage(%25)%20of%20Smoker%20Vs%20Non-Smokers.png)

- Gender distribution analysis

![Gender Distribution](https://github.com/aishwaryasavanth22/Bio-signal-Analysis-for-Smokers-and-Non-Smokers/blob/22f3dce0eed0132b8273341265131666ba1ce8f6/Visualizations/Gender%20Distribution.png)

- Age-based smoking analysis

![Age Vs Smoking Distribution](https://github.com/aishwaryasavanth22/Bio-signal-Analysis-for-Smokers-and-Non-Smokers/blob/22f3dce0eed0132b8273341265131666ba1ce8f6/Visualizations/Age%20Vs%20Smoke%20Distribution.png)

### 5. Feature Engineering and Selection
Performed:
- Label Encoding on categorical columns
- Feature importance using **Extra Trees Classifier**
- Selected **Top 15 most important features**
- Standardization using **StandardScaler**

### 6. Model Building and Evaluation
Built and evaluated:
- Logistic Regression
- Decision Tree Classifier
- Bagging Classifier
- Extra Trees Classifier
- Random Forest Classifier

---

## 🧹 Data Cleaning & Preprocessing

### ✅ Missing Values
- No missing/null values were found in the dataset.

### ✅ Duplicate Values
- Duplicate values were checked.
- Duplicates were retained because similar biological measurements can naturally occur across different individuals.

### ✅ Categorical Encoding
The following categorical columns were converted into numerical format using **Label Encoding**:
- Gender
- Tartar
- Dental Caries
- Oral

### ✅ Feature Scaling
- Applied **StandardScaler** to standardize the feature values and bring them onto the same scale.

---

## 📊 Exploratory Data Analysis (EDA)

### Gender Distribution
- Male count: **35,401**
- Female count: **20,291**

### Smoking Distribution
- Non-Smokers: **35,237**
- Smokers: **20,455**

### Smoking Percentage
- Smokers: **36.73%**
- Non-Smokers: **63.27%**

### Gender-wise Smoking Analysis
- Female smokers: **859**
- Male smokers: **19,596**

### Age Group Insight
- Individuals around the **35-year age group** were found to be more prone to smoking.

### Outlier Analysis
Outliers were found in several features such as:
- Age
- Height
- Weight
- Waist
- Eyesight
- Hearing
- Systolic
- Relaxation
- Fasting Blood Sugar
- Cholesterol
- Triglyceride
- HDL
- LDL
- Haemoglobin
- Urine Protein
- Serum Creatinine
- AST
- ALT
- Gtp
- Dental Caries

**Observation:**  
These outliers were retained because they represent **true biological variations in the population** rather than data errors.

---

## 🧠 Feature Selection

Feature importance was calculated using **Extra Trees Classifier**.  
Based on feature importance scores, the **top 15 most important features** were selected for model development.

This step helped:
- Reduce irrelevant features
- Improve model efficiency
- Focus on the most predictive biological indicators

---

## 🤖 Machine Learning Models Used

### 1. Logistic Regression
Used as a **baseline classification model** for binary classification.

### 2. Decision Tree Classifier
Used to capture **non-linear decision boundaries** and generate interpretable rules.

### 3. Bagging Classifier
Implemented on **Decision Tree with 1000 estimators** to improve stability and reduce variance.

### 4. Extra Trees Classifier
Used as an ensemble-based tree model with increased randomness for robust classification.

### 5. Random Forest Classifier
Used to improve predictive performance through multiple decision trees and majority voting.

---

## 📈 Model Evaluation Metrics

The models were evaluated using:
- Accuracy Score
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

## 🧪 Model Performance

### Logistic Regression
- Accuracy: **0.74**
- Precision: **0.69**
- Recall: **0.63**
- F1-Score: **0.66**

**Confusion Matrix**
```text
[[5363, 1286],
 [1664, 2826]]
```

### Decision Tree Classifier
- Accuracy: 0.78
- Precision: 0.70
- Recall: 0.70
- F1-Score: 0.70

**Confusion Matrix**
```text
[[5779, 1234],
 [1248, 2878]]
```

**Classification Report**
              precision    recall  f1-score   support

           0       0.82      0.82      0.82      7013
           1       0.70      0.70      0.70      4126

    accuracy                           0.78     11139
   macro avg       0.76      0.76      0.76     11139
weighted avg       0.78      0.78      0.78     11139

### Bagging Classifier

- Accuracy: 0.83
- Precision: 0.75
- Recall: 0.80
- F1-Score: 0.77

**Confusion Matrix**
```text
[[5979, 1070],
 [ 841, 3271]]
```

**Classification Report**

              precision    recall  f1-score   support

           0       0.88      0.85      0.86      7027
           1       0.75      0.80      0.77      4112

    accuracy                           0.83     11139
   macro avg       0.81      0.82      0.82     11139
weighted avg       0.83      0.83      0.83     11139

### Extra Trees Classifier

- Accuracy: 0.82
- Precision: 0.75
- Recall: 0.80
- F1-Score: 0.77

**Classification Report**

              precision    recall  f1-score   support

           0       0.88      0.84      0.86      7027
           1       0.75      0.80      0.77      4112

    accuracy                           0.82     11139
   macro avg       0.81      0.82      0.81     11139
weighted avg       0.83      0.82      0.83     11139

### Random Forest Classifier

- Accuracy: 0.83
- Precision: 0.79
- Recall: 0.76
- F1-Score: 0.77

**Confusion Matrix**

```text
[[5972, 1055],
 [ 850, 3262]]
```

**Classification Report**

              precision    recall  f1-score   support

           0       0.85      0.88      0.86      6822
           1       0.79      0.76      0.77      4317

    accuracy                           0.83     11139
   macro avg       0.82      0.82      0.82     11139
weighted avg       0.83      0.83      0.83     11139

📌 Model Comparison

| Model                    | Accuracy | Precision | Recall | F1-Score |
| ------------------------ | -------- | --------- | ------ | -------- |
| Logistic Regression      | 0.74     | 0.69      | 0.63   | 0.66     |
| Decision Tree            | 0.78     | 0.70      | 0.70   | 0.70     |
| Bagging Classifier       | 0.83     | 0.75      | 0.80   | 0.77     |
| Extra Trees Classifier   | 0.82     | 0.75      | 0.80   | 0.77     |
| Random Forest Classifier | 0.83     | 0.79      | 0.76   | 0.77     |

✅ Final Conclusion

This project successfully demonstrates how biological and medical indicators can be used to classify individuals as smokers or non-smokers using machine learning.

Key Findings

- Smoking prevalence is much higher among males in this dataset.
- Individuals around the age of 35 years were found to be more prone to smoking.
- Ensemble learning methods outperformed individual baseline models.
- Bagging Classifier and Random Forest Classifier achieved the best overall performance with an accuracy of approximately 83%.

This indicates that bio-signal based classification can be highly useful for predictive healthcare and health-risk analysis.

🚀 Future Improvements

Possible improvements for this project:

- Hyperparameter tuning using GridSearchCV or RandomizedSearchCV
- Cross-validation for more reliable evaluation
- ROC-AUC score and ROC curve analysis
- Feature importance interpretation in more detail
- Model deployment using Flask / Streamlit
- Testing advanced models like XGBoost, LightGBM, and CatBoost

🛠️ Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- VS Code

💼 Why This Project Matters

This project demonstrates practical skills in:

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Feature Selection
- Data Preprocessing
- Classification Modeling
- Ensemble Learning
- Model Evaluation
- Healthcare Data Analysis

### 👩‍💻 Author

Aishwarya Savanth
Aspiring Data Scientist | Machine Learning Enthusiast | Python & SQL Learner
