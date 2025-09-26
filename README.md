# 🐊 Crocodile EDA + Insights + ML  

This repository contains a full **Exploratory Data Analysis (EDA)** and **Machine Learning workflow** on a crocodile observation dataset.  
The dataset includes biological and observational details such as species, scientific classification, length, weight, age class, sex, and observation dates.  

---

## 📂 Project Structure  

- `crocodiles.csv` → dataset (observations of crocodiles)  
- `notebook.ipynb` → Jupyter/Kaggle notebook with analysis & model  
- `README.md` → project documentation  

---

## 🚀 Objectives  

1. **Data Cleaning & Preparation**  
   - Handle missing values in `Sex` and `Age Class`  
   - Convert observation dates to datetime format  
   - Ensure numerical columns (`Observed Length`, `Observed Weight`) are valid  

2. **Exploratory Data Analysis (EDA)**  
   - Distribution of crocodile lengths  
   - Relationship between length and weight  
   - Most frequently observed species  
   - Sex distribution across observations  
   - Observation counts over time  

3. **Machine Learning (ML)**  
   - Predict **Observed Weight (kg)** using features such as length, age class, and species  
   - Model used: **Random Forest Regressor**  
   - Evaluation metric: **Mean Absolute Error (MAE)**  

---

## 📊 Exploratory Data Analysis  

Some of the key insights from EDA include:  

- Most crocodiles fall into common adult size ranges (peaks in length distribution).  
- **Length strongly correlates with weight**, as expected biologically.  
- A few species dominate the dataset (Morelet's Crocodile, Nile Crocodile).  
- More males are recorded than females, with some unknowns.  
- Observations have increased in recent years, showing improved collection/monitoring.  

Visualizations include histograms, scatter plots, bar charts, and time-series plots.  

---

## 🤖 Machine Learning Model  

- **Target:** `Observed Weight (kg)`  
- **Features:** Common Name, Scientific Name, Family, Genus, Age Class, Sex, Observed Length  
- **Approach:**  
  1. Encode categorical variables with Label Encoding  
  2. Train/test split (80/20)  
  3. Train a Random Forest Regressor (200 estimators)  

- **Performance:**  
  - Achieved **MAE ≈ 14 kg**  
  - Considering crocodiles range from **a few kg to 700+ kg**, this is highly accurate  

- **Feature Importance:**  
  - `Observed Length (m)` was the strongest predictor  
  - `Age Class` and `Species` also contributed significantly  

---

## ✅ Summary  

This project demonstrates how to:  
- Clean and preprocess real-world biological datasets  
- Perform meaningful EDA with visualizations  
- Build and evaluate a predictive ML model  
- Extract biological insights from data science workflows  

---

