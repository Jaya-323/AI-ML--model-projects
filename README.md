#Project-1 description
# 🍷 Wine Quality Classification using Machine Learning

## 📌 Project Overview

This project focuses on predicting wine quality using Machine Learning techniques. The original wine quality scores were converted into a binary classification problem:

- GOOD Wine (1) → Quality ≥ 7
- BAD Wine (0) → Quality < 7

The goal is to classify wines based on their physicochemical properties and identify the most effective machine learning model for this task.

---

## 📊 Dataset Information

The dataset contains 1,599 wine samples with the following features:

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol
- Quality

### Target Variable

A new binary target column named `quality_label` was created:

```python
quality_label = 1 if quality >= 7 else 0
```

---

## 🔍 Project Workflow

### 1. Data Exploration and Analysis
- Dataset inspection
- Missing value analysis
- Statistical summary
- Correlation analysis
- Correlation heatmap visualization

### 2. Feature Engineering
- Created binary target variable (`quality_label`)
- Separated features and target variables

### 3. Data Preprocessing
- Train-Test Split
- Feature Scaling using StandardScaler

### 4. Model Building
The following classification models were trained and evaluated:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier

### 5. Model Evaluation
Models were compared using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

### 6. Hyperparameter Tuning
- Applied GridSearchCV on the best-performing model (KNN)
- Optimized model parameters to improve performance

### 7. Feature Importance Analysis
- Used Permutation Importance to identify the most influential features affecting wine quality prediction

---

## 🏆 Best Model

**K-Nearest Neighbors (KNN)**

### Final Accuracy

**88.75%**

The KNN model achieved the highest performance among all evaluated models and was selected as the final model.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Google Colab

---

## 📈 Key Findings

- Alcohol content was one of the strongest indicators of wine quality.
- Feature scaling significantly improved distance-based algorithms such as KNN.
- KNN outperformed Logistic Regression and Decision Tree on this dataset.
- Hyperparameter tuning helped optimize the final model performance.

---





Jaya Mishra

Machine Learning Project – Wine Quality Classification
