# 🧠 Stroke Prediction using Binary Classification – Intelligent Systems Project

This project was developed for the **Intelligent Systems** course and applies theoretical and practical concepts learned in lab (Logistic Regression, Decision Trees, Random Forest) on a new real-world binary classification dataset – `healthcare-dataset-stroke-data.csv`.

## 👨‍💻 Author
**Maxim Francesco** – 3rd Year, Group 30234, UTCN

---

## 🎯 Project Objective

The main goal was to understand and apply:

- **Logistic Regression** with regularization and polynomial expansion
- **Data preprocessing** (handling missing values, normalization, polynomial features)
- **Tree-based algorithms** (Decision Trees and Random Forest)
- **Underfitting vs Overfitting** behavior
- **Feature Importance** interpretation to understand model decision-making

---

## 📊 Code Summary

### 🔍 Data Exploration (EDA)

- Loaded the dataset using `pandas` and checked shape, types, and target (`stroke`) distribution
- Identified class imbalance (only ~5% positive examples)
- Filled missing values in the `bmi` column using mean imputation
- Investigated feature correlation with the target

### 🛠️ Preprocessing

- Normalized numerical features using `StandardScaler`
- Applied `PolynomialFeatures` (degree 2) to expand feature space
- Performed train/validation/test split using `train_test_split` with stratification

### 🧪 Model Training

#### 1. Logistic Regression
- Tested different regularization strengths (C = 0.1, 1.0, 10.0)
- Compared base model vs polynomial expansion
- Evaluated using accuracy, recall, ROC-AUC

#### 2. Decision Tree
- Tuned `max_depth`, `min_samples_split`, `min_samples_leaf`
- Overfitting observed on deeper trees

#### 3. Random Forest
- Used `n_estimators=100` and `max_depth=7`
- Achieved best validation performance

### ✅ Evaluation

- Used `accuracy_score`, `classification_report`, `roc_auc_score`
- Plotted confusion matrices and ROC curves
- Analyzed `feature_importances_` to understand key predictors

---

## 📘 What I Learned

- How to work with real-world, imbalanced data and handle missing values
- Importance of scaling and polynomial expansion in logistic regression
- Impact of tree depth and splitting parameters in preventing overfitting
- How Random Forests reduce variance compared to single decision trees
- How to interpret model behavior through feature importance

---

## 📦 Tech Stack

- Python 3.10
- Jupyter Notebook
- pandas, numpy
- matplotlib, seaborn
- scikit-learn

---

## 📁 Project Structure

```
.
├── Untitled4.ipynb
├── data/
│   └── healthcare-dataset-stroke-data.csv
├── README.md
```

---

## 📈 Sample Results (may vary)

- Logistic Regression (AUC ≈ 0.78)
- Decision Tree (AUC ≈ 0.75)
- Random Forest (AUC ≈ 0.81)
- F1 Score for positive class ≈ 0.45

---

## 📬 Contact

Questions or suggestions?

**Email**: maaximfrancesco@gmail.com  
**LinkedIn**: [linkedin.com/in/francescomaxim](https://www.linkedin.com/in/francescomaxim)

---
