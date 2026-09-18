# 🏠 Airbnb Accommodation Price Prediction in Bologna

Predictive modeling project to estimate Airbnb listing prices in Bologna using real-world data from **Inside Airbnb** (~4,600 listings and 80 initial features).

---

## 📌 Project Overview
The main goal of this project is to build an end-to-end Machine Learning pipeline to predict accommodation prices per night in Bologna, handling missing data mechanisms, complex JSON feature extractions, and non-linear feature relationships.

---

## ⚙️ Key Steps & Methodology

### 1. Data Cleaning & Encoding Correction
- Resolved encoding errors across textual attributes.
- Standardized price targets and currency formatting.
- Corrected geographical boundaries and invalid values.

### 2. Feature Engineering & Extraction
- Extracted nested structural data from JSON fields (amenities, host verification metrics).
- Created domain-specific composite metrics (host experience, listing density, proximity indicators).

### 3. Missing Data Analysis (MCAR / MAR / MNAR)
- Analyzed missingness patterns using nullity matrices and correlation maps (`missingno`).
- Diagnosed missing host response times as **MAR (Missing at Random)** correlated with listing creation date.
- Implemented context-aware imputation strategies based on missing data mechanisms.

### 4. Exploratory Data Analysis & Feature Selection
- Detected and handled multicollinearity via Variance Inflation Factor (VIF).
- Treated high-leverage outliers in target price and cleaning fees.

### 5. Machine Learning Modeling & Evaluation
- Trained multiple predictive algorithms (Linear Models, Tree-Based Ensembles).
- Cross-validated results using MAE, RMSE, and R² metrics.

---

## 🛠️ Tech Stack & Libraries
- **Language:** Python 3.x
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Seaborn, Matplotlib, Missingno
- **Machine Learning:** Scikit-Learn

