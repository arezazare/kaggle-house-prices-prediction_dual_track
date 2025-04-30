# 🏡 Kaggle House Prices – Advanced Regression & Learn Track Submissions

## 🚀 **Overview**  
This project tackles both versions of the Kaggle House Prices competition:  
1. **House Prices - Advanced Regression Techniques** (log-RMSE based)  
2. **Housing Prices Competition for Kaggle Learn Users** (raw-RMSE based)  

A fully structured machine learning pipeline was developed to predict house sale prices in Ames, Iowa. The project includes both log-transformed and raw-target modeling for optimized performance across both competitions.

- ✅ Full EDA, feature engineering, cleaning, and preprocessing  
- ✅ Modeling with Ridge, XGBoost, and more — with hyperparameter tuning (GridSearchCV)  
- ✅ Dual prediction strategy: log-target submission + raw-target model  
- ✅ Final leaderboard submission with Ridge + XGBoost model blending

🎯 **Current Kaggle Scores (First Try):**  
- 🧪 Advanced Regression Techniques → `0.12885` RMSE (log-transformed target) — **Rank: 1130 / 4711 teams**  
- 📘 Kaggle Learn Users → `14556.14` RMSE (raw target) — **Rank: 525 / 6639 teams**

---

## 📊 Dataset
- **Source:** Kaggle House Prices Dataset  
- **Training Set:** 1460 rows × 81 columns  
- **Test Set:** 1459 rows × 80 columns  
- **Features Include:**  
  - LotFrontage, LotArea, OverallQual, YearBuilt, Neighborhood, GrLivArea, GarageCars, and more  
- **Target:**  
  - SalePrice (continuous value in USD)

---

## 🧪 Key Tasks

- Log transformation of target variable for Advanced competition
- Feature engineering:
  - TotalSF, TotalBathrooms, HouseAge, TotalPorchSF
- One-Hot and Ordinal Encoding for categorical variables
- MinMaxScaler for continuous features
- Modeling with multiple regressors: Ridge, XGBoost, Gradient Boosting, etc.
- Hyperparameter tuning via GridSearchCV
- Blending Ridge and XGBoost for final predictions
- Submission generation for both competitions

---

## 🔍 Key Steps

### Data Cleaning

- Handling missing values (mode, median, and 'None' fill-ins)
- Dropping low-variance or redundant features
- Correcting inconsistent text entries

### Exploratory Data Analysis (EDA)

- Distribution and skewness visualizations
- Outlier detection using IQR and boxplots
- Correlation analysis with heatmaps and scatterplots

### Modeling

- Ridge Regression
- Random Forest Regressor
- Decision Tree Regressor
- Gradient Boosting Regressor
- AdaBoost Regressor
- K-Nearest Neighbors (KNN)
- XGBoost Regressor
- LightGBM Regressor

### Evaluation

- R² Score, MAE, RMSE on both log-transformed and raw targets
- Cross-validation (CV R²)
- Performance comparison via barplots
- Final model chosen based on best log RMSE

### Submission

- `submission_log.csv` → for **Advanced Regression Techniques** (uses `np.expm1(...)`)  
- `submission_raw.csv` → for **Kaggle Learn Users** (raw predictions)

---

## 🔧 Technologies Used

- Python (NumPy, Pandas, Seaborn, Matplotlib, Scikit-learn, XGBoost, LightGBM)
- Jupyter Notebook
- GridSearchCV for tuning
- Joblib for saving model and scaler
- Git & GitHub for version control
- Kaggle APIs and CSV-based submission

---

## 🧠 What I Learned

- Why log-transforming skewed targets is crucial for regression tasks  
- How Ridge Regression can outperform boosted trees with proper scaling  
- How to optimize models for **two different competition metrics**  
- Importance of encoding, scaling, and outlier handling in tabular datasets  
- Blending models can consistently outperform individual ones  
- Reproducibility via clean separation of modeling and submission stages

---

## 👏 Author

**Reza Zare** — Full pipeline built, evaluated, and deployed from scratch.  
Experienced in regression, classification, clustering, and real-world Kaggle modeling.

---

## 📎 Resources

- [Advanced Regression Techniques Competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)  
- [Housing Prices for Kaggle Learn Users](https://www.kaggle.com/competitions/home-data-for-ml-course)

---

## 📎 Credits

Dataset and competition hosted by Kaggle.  
All rights belong to the original dataset contributors.

---
