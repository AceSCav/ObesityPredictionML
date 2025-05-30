# Obesity Level Estimation using Decision Tree Classifier

This project applies machine learning techniques to estimate obesity levels based on eating habits and physical condition. The dataset is sourced from the UCI Machine Learning Repository.

## 📊 Dataset

* **Source:** [UCI ML Repository - Obesity Levels](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition)
* **Features:** Age, Gender, Height, Weight, family history of overweight, smoking habits, eating habits, water consumption, and physical activity.

## 🎯 Objective

Build a classification model that predicts an individual's obesity level based on clinical and behavioral attributes.

## ⚙️ Project Pipeline

1. **Library imports and dataset loading**
2. **Initial data exploration and descriptive analysis**
3. **IMC (BMI) calculation and obesity level categorization**
4. **Data cleaning**

   * Handling missing values
   * Removing duplicates
   * One-hot encoding of categorical variables
5. **Outlier removal using z-score**
6. **Feature standardization**
7. **Mapping target variable (obesity level) to numerical values**
8. **Splitting the dataset into training and testing sets**
9. **Model training with Decision Tree Classifier**
10. **Model evaluation using classification report and confusion matrix**

## 🧠 Machine Learning Model

* **Algorithm:** `DecisionTreeClassifier` from `scikit-learn`
* **Features used for training:**

  * `family_history_with_overweight`
  * `FAVC` (Frequent consumption of high-caloric food)
  * `NCP` (Number of main meals per day)
  * `CH2O` (Daily water consumption)
  * `FAF` (Frequency of physical activity)

## 📈 Results

* Classification performance metrics such as **precision**, **recall**, and **f1-score** are displayed.
* A **confusion matrix** is printed to evaluate prediction accuracy across categories.

## 📦 Requirements

* Python 3.7+
* Libraries:

  * `pandas`
  * `numpy`
  * `scikit-learn`
  * `scipy`
  * `ucimlrepo`

Install requirements using:

```bash
pip install pandas numpy scikit-learn scipy ucimlrepo
```

## ▶️ How to Run

```bash
python obesity_estimation.py
```

> Note: Make sure you are connected to the internet, as the dataset is fetched via the `ucimlrepo` API.

## 🚀 Future Improvements

* ✅ **Model Comparison:** Evaluate performance across different classifiers like Random Forest, SVM, KNN, and Logistic Regression.
* ✅ **Hyperparameter Tuning:** Use grid search or randomized search for optimizing Decision Tree parameters.
* ✅ **Feature Expansion:** Include more features such as calorie intake, dietary patterns, or genetic predispositions if available.
* ✅ **Cross-Validation:** Implement k-fold cross-validation for more reliable model evaluation.
* ✅ **Visualization:** Add feature importance plots and performance visualization (e.g., confusion matrix heatmap).
* ✅ **Deployment:** Convert the notebook or script into a web app using Flask, Streamlit, or FastAPI.


