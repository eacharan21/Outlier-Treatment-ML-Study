# 📊 The Effect of Outlier Treatment on Predictive Modeling Performance

## 📌 Overview

This project analyzes how different outlier treatment techniques impact machine learning model performance.

We compare:

* No treatment
* Trimming
* Winsorization
* Log Transformation
* Box-Cox Transformation

Models used:

* Linear Regression
* XGBoost

---

## 🎯 Objectives

* Evaluate how outliers affect prediction accuracy
* Compare different outlier handling techniques
* Analyze model sensitivity (Linear vs Tree-based models)

---

## 📂 Dataset

* Weather dataset (Hyderabad region)
* Source: NASA POWER dataset
* Features include:

  * Temperature
  * Humidity
  * Rainfall
  * Wind Speed
  * Radiation

---

## ⚙️ Methods Used

### 🔹 Outlier Detection

* Interquartile Range (IQR)

### 🔹 Outlier Treatment Techniques

* Trimming (Removal)
* Winsorization (Capping)
* Log Transformation
* Box-Cox Transformation

---

## 🤖 Models Used

* Multiple Linear Regression
* XGBoost

---

## 📈 Results

### 🔹 Linear Regression

| Method        | R²     |
| ------------- | ------ |
| With Outliers | 0.5783 |
| Trimming      | 0.5308 |
| Winsorization | 0.5900 |
| Log Transform | 0.5363 |
| Box-Cox       | 0.5900 |

👉 Best: Winsorization & Box-Cox

---

### 🔹 XGBoost

| Method        | R²     |
| ------------- | ------ |
| With Outliers | 0.7497 |
| Trimming      | 0.7237 |
| Winsorization | 0.7475 |
| Log Transform | 0.7563 |
| Box-Cox       | 0.7534 |

👉 Best: Log Transformation

---

## 🔍 Key Insights

* Linear Regression is highly sensitive to outliers
* Winsorization & Box-Cox improve performance
* XGBoost is robust to outliers
* Tree-based models require less preprocessing

---

## 🧠 Conclusion

Outlier treatment should not be blindly applied.
The choice depends on:

* Model type
* Data distribution

---

## 📎 Research Paper

You can read the full paper here:
👉 `The_Effect_of_Outlier_Treatment_on_Predictive_Modeling_Performance.pdf`

---

## 🛠️ Tech Stack

* Python / R
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Matplotlib / Seaborn

---

## 🙌 Author

**Aditya Charan Eranki**
B.Sc/M.Sc Mathematics – VIT

---
