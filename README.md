# Decision Trees and Random Forests - AI & ML Internship Task

## 📌 Task Overview
This repository contains my solution for **Task 5** of the AI & ML Internship program.  
The goal of this task is to understand and implement **tree-based models** for classification & regression.

## 🎯 Objectives
- Train a **Decision Tree Classifier** and visualize the tree.
- Analyze **overfitting** and control tree depth.
- Train a **Random Forest Classifier** and compare accuracy with a single decision tree.
- Interpret **feature importances**.
- Evaluate models using **cross-validation**.

## 🛠 Tools & Libraries
- Python  
- Scikit-learn  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Graphviz (for decision tree visualization)

## 📊 Dataset
I used the **Cleveland Heart Disease Dataset** from the UCI repository:  
[Heart Disease Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data)  

## 🚀 Steps Performed
1. Data preprocessing and cleaning (handled missing values `?` in `ca` and `thal`).
2. Converted target into **binary classification** (0 = No Disease, 1 = Disease).
3. Trained a **full Decision Tree** and observed overfitting.
4. Trained a **constrained Decision Tree (max depth = 4)** to reduce overfitting.
5. Implemented a **Random Forest Classifier**.
6. Visualized the Decision Tree and Feature Importances.
7. Evaluated models using **10-Fold Cross-Validation**.

## 📈 Results
### Decision Tree (Max Depth = 4)
- Test Accuracy: **~0.78**  
- Overfitting reduced compared to full tree.  
- Classification report showed balanced performance.

### Random Forest (100 estimators, max depth = 8)
- Test Accuracy: **~0.85**  
- Better generalization compared to single Decision Tree.  
- Important features identified: **ca, thal, oldpeak, cp, thalach**  

### Cross-Validation
- **10-Fold CV Mean Accuracy:** ~0.82  
- **Standard Deviation:** small, proving stable performance.  

✅ Random Forest outperformed the Decision Tree due to bagging and reduced overfitting.

## 📂 Repository Structure
