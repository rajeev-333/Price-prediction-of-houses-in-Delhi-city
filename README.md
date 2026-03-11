#  Delhi House Price Prediction

A machine learning project that predicts house prices in Delhi based on property features such as area, BHK, bathrooms, locality, furnishing status, parking, and property type.

---

##  Project Objective

The objective of this project is to build a regression model that accurately estimates house prices using historical real estate data. The project demonstrates end-to-end data analysis including data cleaning, feature engineering, exploratory data analysis (EDA), model building, and evaluation.

---

## 📊 Dataset Information

- Source: Kaggle (Public Dataset)
- Total Records: ~1259
- Target Variable: `Price`
- Key Features:
  - Area
  - BHK
  - Bathroom
  - Locality
  - Parking
  - Furnishing Status
  - Property Type

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

##  Data Preprocessing Steps

- Removed irrelevant and redundant columns
- Handled missing values using:
  - Mode imputation for categorical/discrete features
  - Logical derivation (Per_Sqft = Price / Area)
- Removed outliers using Z-score method
- Encoded categorical variables using Label Encoding
- Scaled numerical features where required
- Prevented data leakage by removing derived target-related features

---

## 📈 Exploratory Data Analysis (EDA)

Key insights:

- Area, BHK, Bathrooms, and Locality significantly influence house prices.
- Premium localities consistently show higher pricing trends.
- Under-construction properties tend to have higher price expectations.
- Price distribution is right-skewed, indicating presence of high-value outliers.

---

##  Models Implemented

1. Decision Tree Regressor (Baseline Model)
2. Random Forest Regressor (Final Model)

Hyperparameter tuning was performed using GridSearchCV to optimize performance.

---

## 📊 Model Performance

Random Forest Regressor achieved:

- R² Score: ~0.85  
- MAE: 0.053  
- RMSE: 0.079  

The model explains approximately 85% of the variance in house prices.

---

## 📎 Key Learnings

- Practical handling of missing values and outliers
- Avoiding data leakage in ML models
- Importance of feature engineering
- Understanding regression evaluation metrics (R², MAE, RMSE)
- Model comparison and hyperparameter tuning
