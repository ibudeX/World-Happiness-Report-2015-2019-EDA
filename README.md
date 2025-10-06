# 🌍 World Happiness Report (2015–2019) – Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellowgreen)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-teal)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📖 Overview

The **World Happiness Report** is an annual publication that ranks countries based on factors such as GDP per capita, health, freedom, social support, and generosity.

This project merges **five years of data (2015–2019)** and performs a comprehensive **Exploratory Data Analysis (EDA)** to uncover:
- 🌎 **Global happiness trends**
- 📈 **Key influencing factors**
- 🔍 **Patterns across countries & regions**

---

## 🎯 Objectives

1. Integrate datasets from 2015–2019 into a unified structure.
2. Perform thorough **data cleaning** and **profiling**.
3. Analyze **univariate** and **bivariate** distributions.
4. Identify **key correlations** with happiness scores.
5. Compare **top vs. bottom countries** in global rankings.

---

## 📂 Data Source

- **World Happiness Report (2015–2019)** from [Kaggle](https://www.kaggle.com)
- Extracted using [`kagglehub`](https://github.com/Kaggle/kagglehub)

---

## ⚙️ Step-by-Step Methodology

### **Step 1: Data Collection & Integration**
- Loaded datasets for **2015–2019**.
- Renamed inconsistent columns to a **unified schema**.
- Concatenated all datasets into a single DataFrame.
- Dropped redundant/incomplete columns (e.g., `Region`, `Standard Error`, `Dystopia.Residual`).

**Discovery:**  
- Different column names existed across years.
- Standardization was crucial for comparison.

**Insights:**  
- 750+ entries from 150+ countries.
- Clean schema allows **trend analysis** across years.

---

### **Step 2: Data Profiling & Cleaning**
- Removed irrelevant/inconsistent columns.
- Verified **data types**, **null values**, and **statistical ranges**.
- Ensured dataset was clean and analysis-ready.

**Discovery:**  
- Dataset had no missing values post-cleaning.
- Core variables: `Score`, `GDP`, `Family`, `Health`, `Freedom`, `Trust`, `Generosity`.

**Insights:**  
- Score range: ~2.8 to 7.8 across countries.

---

### **Step 3: Univariate Analysis**
- Created **histograms** and **KDE plots** for core variables.

**Discovery:**  
- GDP & Trust → **right-skewed**.
- Happiness Scores → **normally distributed** around 5.5–6.5.

**Insights:**  
- **Generosity & Trust** levels are low worldwide.
- GDP & Health skewness shows **global inequality**.

---

### **Step 4: Bivariate & Correlation Analysis**
- Generated **correlation matrix heatmap**.

**Discovery:**  
- Strong positive correlation between **GDP, Health, and Happiness Score**.
- Weak correlation for **Trust & Generosity**.

**Insights:**  
- Wealth & life expectancy are key happiness drivers.
- High GDP countries tend to have higher happiness scores.

---

### **Step 5: Country-Wise Insights**
- Visualized **Top 10** and **Bottom 10** countries.

**Discovery:**  
- Nordic countries dominate top rankings (Finland, Denmark, Norway).
- Economically unstable countries rank lowest (South Sudan, Afghanistan).

**Insights:**  
- Stability, trust, and wealth greatly impact happiness.
- Cultural & social systems in Scandinavia contribute to high well-being.

---

## 📊 Example Visuals

| Happiness Score Distribution | Correlation Heatmap |
|------------------------------|---------------------|
| ![Histogram](https://github.com/user-attachments/assets/82861531-d618-477e-88f6-43e50705af23) | ![Heatmap](https://github.com/user-attachments/assets/eaeed8eb-8f97-4deb-8f4d-e516b8eefa78) |

| Top 10 Countries | Bottom 10 Countries |
|------------------|---------------------|
| ![Top10](https://github.com/user-attachments/assets/143dd605-0483-401e-a0b6-a74ea3bd0407) | ![Bottom10](https://github.com/user-attachments/assets/b97dca99-cfa6-4991-9e34-b04715007daf) |


---

## 💡 Key Takeaways
- **GDP** and **Health** are the most influential factors for happiness.
- **Generosity** and **Trust** have minimal impact globally.
- Countries with **economic & political stability** tend to score highest.
- Scandinavian nations set the global benchmark for well-being.

---

## 🛠️ Tech Stack
- **Languages:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Kagglehub



⭐ If you like this project, **consider giving it a star** on GitHub!
