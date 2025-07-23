# 🏙️ Profit Meets Precision: Apartment Pricing Powered by Machine Learning

**Capstone Project 3 by Dhika Wahyu Pratama**  
This project builds a machine learning-based pricing tool to predict apartment sale prices in Daegu. It aims to support strategic pricing decisions and help maximize profitability in the real estate market.

---

## 📌 Problem Statement

As the number of apartment units in the market grows, setting the right price becomes more critical to remain competitive without sacrificing potential profits.

---

## 🎯 Objectives

- Develop a machine learning model to predict apartment sale/rental prices.
- Provide fair and accurate price estimates based on property features.
- Help property owners and marketing teams determine optimal prices for new listings.
- Achieve the lowest possible RMSE, MAE, and MAPE to ensure predictive accuracy.

---

## 📊 Dataset Overview

- Total records: 4,123 apartment listings in Daegu
- After cleaning: 2,671 unique listings (duplicates and outliers removed)
- Key features: `Size (sqf)`, `YearBuilt`, `HallwayType`, `ParkingLot`, `N_facilitiesInApt`, `N_facilitiesNearby`, etc.

---

## 🔧 Project Workflow

### 1. Data Cleaning
- Removed duplicates and outliers
- Checked and handled missing values

### 2. Feature Engineering
- Data transformation (scaling, encoding)
- Built a preprocessing pipeline

### 3. Modeling
- Algorithm: Gradient Boosting (with hyperparameter tuning)
- Evaluation metrics: RMSE, MAE, MAPE
- Used 5-fold cross-validation

### 4. Interpretation
- Analyzed feature importance and SHAP values

---

## 🧠 Key Insights

- Most influential features:
  - `Size (sqf)`: Larger apartments tend to have higher prices
  - `HallwayType`: "Terraced" increases perceived value
  - `YearBuilt`: Newer constructions lead to higher prices
  - `ParkingLot` and `FacilitiesInApt`: More availability adds value

- Best model performance after tuning:
  - RMSE: ~44,172
  - MAPE: ~19% (average prediction error)

---

## ⚠️ Limitations

- Some prediction bias observed in extreme values
- Missing external factors such as:
  - Neighborhood safety
  - City view
  - Noise level
  - Access to public facilities and food
- Model is trained only on data from Daegu — limited generalization

---

## ✅ Recommendations

- **A/B Testing**: Compare the effectiveness of predicted vs. manually priced listings
- **Add contextual features**: Distance to city center, noise, convenience, etc.
- **Expand data coverage**: Include apartments from other cities
- **Explore deeper models**: Consider Neural Networks with larger datasets
- **Develop long-term forecasting**: Predict price trends for investment planning

---

## 🛠️ Technologies Used

- Python 3.9
- Scikit-learn
- XGBoost / Gradient Boosting
- SHAP for model interpretation
- Pandas, NumPy, Matplotlib
