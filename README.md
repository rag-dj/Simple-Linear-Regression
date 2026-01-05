# 📈 Simple Linear Regression: Height vs Weight (From Scratch)

This project demonstrates a **complete end-to-end implementation of Simple Linear Regression** using **Python and scikit-learn**, applied to a real-world style dataset (Height vs Weight).

The notebook walks through **data exploration, visualization, preprocessing, model training, prediction, and evaluation** in a clear and structured way.

---

## 🎯 Objective

To understand and implement **Simple Linear Regression** by predicting **height** based on **weight**, while covering the full ML workflow:

* Exploratory Data Analysis (EDA)
* Feature selection
* Train–test split
* Feature scaling (Z-score)
* Model training
* Prediction
* Performance evaluation

---

## 📂 Project Structure

```
.
├── height-weight.csv        # Dataset
├── linear_regression.ipynb  # Jupyter notebook
└── README.md                # Project documentation
```

---

## 🧠 Workflow Overview

```
Load Data
   ↓
Exploratory Analysis (Scatter, Correlation)
   ↓
Feature Selection (X, Y)
   ↓
Train–Test Split
   ↓
Standardization (Z-score)
   ↓
Linear Regression Model
   ↓
Prediction
   ↓
Model Evaluation
```

---

## 🔹 Step-by-Step Explanation

### 1️⃣ Import Dependencies

Core libraries used:

* `pandas`, `numpy` → data handling
* `matplotlib`, `seaborn` → visualization
* `scikit-learn` → modeling & evaluation

---

### 2️⃣ Data Loading & Visualization

* Dataset loaded from `height-weight.csv`
* Scatter plot used to visually inspect the relationship
* Correlation matrix and heatmap used to confirm linear dependency

✔️ Confirms strong linear correlation between height and weight.

---

### 3️⃣ Feature Selection

* **Independent variable (X):** Weight
* **Dependent variable (Y):** Height

Handled correctly:

* `X` as **2D array**
* `Y` as **1D array**

---

### 4️⃣ Train–Test Split

* Split performed using `train_test_split`
* Test size: **25%**
* `random_state=42` for reproducibility

---

### 5️⃣ Feature Scaling (Standardization)

* Applied **Z-score normalization**
* Used `StandardScaler`
* Fitted on training data only to avoid data leakage

✔️ Improves numerical stability and model behavior.

---

### 6️⃣ Model Training (Linear Regression)

* Used `LinearRegression` from scikit-learn
* Model learns:

  * **Coefficient (slope)**
  * **Intercept**

These define the best-fit line.

---

### 7️⃣ Model Visualization

* Scatter plot of training data
* Best-fit regression line plotted
* Helps visually validate model performance

---

### 8️⃣ Prediction on Test Data

* Predictions generated on unseen test samples
* Uses learned regression equation

---

### 9️⃣ Model Evaluation Metrics

Evaluated using standard regression metrics:

* **Mean Absolute Error (MAE)**
* **Mean Squared Error (MSE)**
* **Root Mean Squared Error (RMSE)**
* **R² Score**

These metrics quantify:

* Prediction error
* Model accuracy
* Variance explained by the model

---

## 📊 Key Learnings

* How linear regression works mathematically and practically
* Importance of feature scaling
* How evaluation metrics reflect model quality
* End-to-end ML pipeline for regression problems

---

## 🛠️ Tech Stack

* Python 3.11
* Pandas
* NumPy
* Matplotlib
* Seaborn
* scikit-learn

