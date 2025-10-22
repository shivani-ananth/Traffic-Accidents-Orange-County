# 🚗 Traffic Accident Injury Prediction – Orange County, FL

This project uses machine learning to predict the **severity of injuries** resulting from traffic accidents in **Orange County, Florida**, using real-world data from the Florida Department of Transportation (FDOT). The goal is to identify key risk factors that contribute to injury severity and support data-driven road safety improvements.

---

## 📘 Project Overview
- Analyzed **12,000+ accident records (2020)** from FDOT’s State Safety Office GIS tool.  
- Preprocessed and merged monthly CSV datasets into a single structured dataset.  
- Engineered features for driver behavior, environmental conditions, and road factors.  
- Built multi-class classification models to predict **injury severity**:  
  **0:** No injury · **1:** Minor · **2:** Severe · **3:** Fatality  
- Evaluated models using **F1-score** and **accuracy** to account for class imbalance.

---

## 🧠 Key Insights
- Alcohol or drug involvement and reckless driving were major predictors of severe injuries.  
- Most fatal accidents occurred during **late evening hours**.  
- Boosting models (especially **CatBoost**) performed best with a weighted F1 ≈ 0.61.  
- Synthetic Minority Oversampling (SMOTE) improved recall for minority (severe/fatal) classes.  

---

## ⚙️ Modeling Techniques
- **Data Cleaning & Preprocessing:** Pandas, feature reduction, encoding, imputation  
- **Machine Learning Models:** Logistic Regression, KNN, SVM, CatBoost, XGBoost, LightGBM  
- **Balancing & Evaluation:** SMOTE, train-test split, F1-score prioritization  
- **Visualization:** Matplotlib, Seaborn  

---

## 📁 Files Included
- `data/` → Monthly CSV datasets from FDOT (Jan–Dec 2020)  
- `Final Report_Group3.pdf` → Full research report and methodology  
- `Traffic_Accidents_Orange_County.ipynb` → Jupyter Notebook with analysis and models  

> Note: Large CSV files may not render in GitHub due to file size limits.  
> You can download or clone the repository to explore them locally.

---

## 🧰 Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, CatBoost, XGBoost, LightGBM, Jupyter Notebook  

---

## 🏁 Conclusion
Machine learning provides valuable insights into **traffic accident injury patterns**, but data imbalance and feature overlap limit predictive precision. Future work could include gathering richer data (driver demographics, vehicle types, weather conditions) and exploring binary models (injury vs. no injury) for improved reliability.
