# SWYNEX Final Data Science Project: Used Car Price Classification

Welcome to the repository for my capstone project (Task 4), marking the final milestone of my Data Science Internship at **SWYNEX Technologies**! 

This project demonstrates a complete end-to-end data science lifecycle—from raw data ingestion and exploratory data analysis to feature engineering, predictive modeling, and model evaluation.

---

## 📈 Project Architecture & Workflow

1. **Data Ingestion & Inspection:**
   * Loaded the `ford.csv` dataset.
   * Inspected structural properties, data shapes, summary statistics, and missing value checks.

2. **Exploratory Data Analysis (EDA) & Visualizations:**
   * Generated distribution histograms for vehicle prices.
   * Constructed medium-dark themed box plots mapping price variations across different car models.
   * Computed and visualized numerical feature correlation heatmaps.

3. **Data Cleaning & Feature Engineering:**
   * Filtered anomalies in manufacturing years.
   * Transformed the continuous target variable (`price`) into discrete classification brackets (`0: Budget`, `1: Mid-Range`, `2: Premium`) using quantile binning (`pd.qcut`).
   * Applied One-Hot Encoding to categorical features (`model`, `transmission`, `fuelType`).

4. **Preprocessing, Scaling & Splitting:**
   * Partitioned the dataset using an 80-20 train-test split (`train_test_split`).
   * Standardized feature inputs using scikit-learn's `StandardScaler`.

5. **Model Training & Cross-Validation:**
   * Trained a robust **RandomForestClassifier** ensemble model (`n_estimators=100`).
   * Executed **5-Fold Cross-Validation** to validate model stability and generalize accuracy metrics.

6. **Evaluation & Performance Metrics:**
   * Measured classification efficacy using **Accuracy Score** and **Weighted F1-Score**.
   * Generated a **Confusion Matrix Heatmap** and a detailed **Classification Report** (Precision, Recall, F1-Score breakdown).
   * Extracted and visualized the **Top 10 Feature Importances** driving the model's decision-making process.

---

## 🛠️ Tech Stack & Dependencies
* **Programming Language:** Python
* **Data Processing:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn`

---

## 📂 Repository Contents
* `final_project.ipynb`: The complete Jupyter Notebook containing the full code script, custom styling, and output visualizations.
* `ford.csv`: The dataset used for training and testing.
* `README.md`: Project documentation.

---
*Developed with dedication by **Chetan Rathore***  
*Data Science Intern at SWYNEX Technologies*

