# House Price Prediction using Machine Learning

A machine learning pipeline for predicting house prices based on features like area, bedrooms, location amenities, and furnishing status. Built with `pandas`, `scikit-learn`, `XGBoost`, and `matplotlib`, this project includes data preprocessing, feature engineering, model training, evaluation, and visualization.

---

## Project Overview

This project aims to accurately estimate house prices using regression techniques. We performed:

- Data Cleaning & Feature Engineering  
- Stacking Ensemble (Random Forest + XGBoost)  
- Log transformation of target variable  
- Standardization and Imputation  
- Evaluation using RMSE, R² Score, and Relative Accuracy  
- Model Export for Deployment

---

## Dataset

The dataset consists of residential house listings with the following key features:

- `price`, `area`, `bedrooms`, `bathrooms`, `stories`
- Amenities: `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `parking`
- Preferences: `prefarea`, `furnishingstatus`

Sample (cleaned data):

| price     | area | bedrooms | bathrooms | mainroad | guestroom | ... |
|-----------|------|----------|-----------|----------|-----------|-----|
| 13300000  | 7420 | 4        | 2         | yes      | no        | ... |

---

## Model Architecture

The pipeline includes:

- **Preprocessing**: Imputation + Scaling using `StandardScaler`
- **Feature Engineering**: Total rooms, area per room, etc.
- **Model**: Stacking Regressor (Random Forest + XGBoost + RidgeCV)

---

## Results

| Metric                | Value             |
|-----------------------|------------------|
| RMSE                  | ₹1,447,704.47     |
| R² Score              | 0.5854            |
| Relative Accuracy     | 71.09%            |

>  **Note**: Further tuning or using deep learning methods may improve performance.

---

## Visualizations

More visualizations available in the notebook:
- Feature Distributions
- Correlation Heatmap
- Residual Plot


## 📄 License

This project is licensed under the **MIT License**.  
Feel free to use, modify, and share it with attribution.

---

⭐ If you liked this repo, don’t forget to star it and share it with others!
