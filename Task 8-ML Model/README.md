# Task 8 - Machine Learning Model: Student Performance Prediction

## Problem Statement
Build a linear regression model to predict student's final grades (G3) based on demographic, social and academic features, and evaluate the impact of including prior grades (G1, G2) on prediction accuracy.

## 📊 Dataset
- **Source:** [Student Alcohol Consumption (Kaggle/UCI)](https://www.kaggle.com/datasets/uciml/student-alcohol-consumption)
- **File:** student-mat.csv
- **Size:** 395 students, 33 columns

## 🔬 Approach
1. **Exploratory Analysis:** Examined distribution of final grades (G3) — most students scoring 8-20, plus a cluster at 0 representing likely droputs/abstentees

2. **Correlation Analysis:** Identified G1 and G2 (prior period grades) as by far the strongest predictors of G3 (correlations of 0.80 and 0.90), while `failures` showed 
the strongest negative correlation (-0.36).

3. **Model 1 (without G1/G2):** Used demographic/behavioral features only.

4. **Model 2 (with G1/G2):** Same features plus prior grades

## 🔑 Key Results
1. Including prior grades improved accuracy from **10% to 77%**, confirming academic history as the dominant predictor of future performance

2. The model shows a **understimation bias** - skewing predictions for low-performing students, highlighting the limits of ML in capturing factors like motivation

## 🔨 Tools Used
- Python, Pandas, Matplotlib, Seaborn, Scikit-learn
- Jupyter Notebook (VS Code)
- Model: Linear Regression

## 📂 Files
- `student_ml.ipynb` — Full analysis and model notebook
- `student-mat.csv` — Dataset