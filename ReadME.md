# 📊 The Effect of Outlier Treatment on Predictive Modeling Performance

## 🚀 Overview

This project investigates how different outlier treatment techniques affect the performance of machine learning models.

We perform a **comparative study** using real-world weather data and evaluate how preprocessing decisions influence predictive accuracy.

---

## 🌐 Dataset Source

The dataset used in this project was obtained from NASA's POWER (Prediction Of Worldwide Energy Resources) Data Access Viewer:

👉 https://power.larc.nasa.gov/data-access-viewer/

NASA POWER provides **satellite-based meteorological data**, widely used in climate, agriculture, and energy research.

---

## 📊 Dataset Details

* 📍 Location: Hyderabad, India
* 📅 Time Period: 1984 – 2025 (Daily data)
* 📁 Format: CSV
* 📡 Source: NASA Langley Research Center

### Features Used:

* T2M_MAX → Maximum Temperature
* T2M_MIN → Minimum Temperature
* RH2M → Humidity
* PRECTOTCORR → Rainfall
* WS2M → Wind Speed
* ALLSKY_SFC_SW_DWN → Solar Radiation

---

## 🎯 Objectives

* Analyze the impact of outliers on model performance
* Compare different outlier treatment techniques
* Evaluate model sensitivity to outliers
* Provide practical insights for preprocessing decisions

---

## ⚙️ Methodology

### 🔹 Outlier Detection

* Interquartile Range (IQR)

### 🔹 Outlier Treatment Techniques

* Trimming (Removal of outliers)
* Winsorization (Capping extreme values)
* Log Transformation
* Box-Cox Transformation

---

## 🤖 Models Used

* Multiple Linear Regression
* XGBoost (Extreme Gradient Boosting)

---

## 📈 Results

### 🔹 Linear Regression Performance

| Method                 | R² Score |
| ---------------------- | -------- |
| With Outliers          | 0.5783   |
| Trimming               | 0.5308   |
| Winsorization          | 0.5900   |
| Log Transformation     | 0.5363   |
| Box-Cox Transformation | 0.5900   |

👉 **Best Methods:** Winsorization & Box-Cox

---

### 🔹 XGBoost Performance

| Method                 | R² Score |
| ---------------------- | -------- |
| With Outliers          | 0.7497   |
| Trimming               | 0.7237   |
| Winsorization          | 0.7475   |
| Log Transformation     | 0.7563   |
| Box-Cox Transformation | 0.7534   |

👉 **Best Method:** Log Transformation

---

## 🔍 Key Insights

* Linear Regression is highly sensitive to outliers
* Winsorization and Box-Cox improve linear model performance
* XGBoost is robust to outliers
* Tree-based models require less preprocessing
* Outlier treatment should be applied based on model type

---

## 🧠 Conclusion

Outlier handling is not a one-size-fits-all approach.

* For **Linear Models** → Proper treatment improves accuracy
* For **Tree-Based Models** → Minimal preprocessing is sufficient

Careful selection of preprocessing techniques leads to better model performance.

---

## 📊 Visualizations

(Add your plots in `/images` folder and link them here)


```markdown
![Rain Distribution](images/rain_distribution.png)
![Outlier Comparison](images/boxplot.png)
```

---

## 🛠️ Tech Stack

* Python / R
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Matplotlib, Seaborn

---

## 📎 Research Paper

Full paper available in this repository:
📄 *The Effect of Outlier Treatment on Predictive Modeling Performance*

---

## 🙌 Author

**Aditya Charan Eranki**
M.Sc Mathematics (Data Science)
Vellore Institute of Technology

---
