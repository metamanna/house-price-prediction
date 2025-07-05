
# 🏠 House Price Prediction (Kaggle: Advanced Regression Techniques)

This project aims to predict house prices using various regression models, advanced feature engineering, and model evaluation techniques. The dataset comes from the [Kaggle House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) competition.

---

## 📁 Project Structure

1.app.py # Gradio web app for manual predictions
2. notebook.ipynb # Full data exploration, modeling, and training
3. xgb_model.pkl # Trained XGBoost model
4. scaler.pkl # Scaler for feature normalization
5. feature_columns.pkl # Final features used in model
6. train.csv # Training data (from Kaggle)
7. test.csv # Test data (from Kaggle)
8. submission.csv # Final predictions for Kaggle submission
9. requirements.txt # All dependencies
10. README.md # Project overview and instructions

## 🚀 Features

-  Full EDA & visualization (Seaborn, Matplotlib)
-  Feature engineering (ratios, aggregates, binary flags)
-  Outlier detection and removal
-  Scaling, encoding, and data preprocessing
-  Model comparison with RMSE & R² metrics
-  Cross-validation for robustness
-  Final model trained on log-transformed target
-  Gradio app for manual prediction

---

## Model Performance (Cross-Validation)

| Model              | RMSE  | R² Score |
|-------------------|-------|----------|
| XGBoost           | 0.13  | 0.8630   |
| Gradient Boosting | 0.13  | 0.8629   |
| Random Forest     | 0.14  | 0.8500   |
| ElasticNet        | 0.15  | 0.8168   |
| Ridge             | 0.17  | 0.7715   |
| Lasso             | 0.17  | 0.7621   |
| KNN               | 0.19  | 0.7168   |
| Linear Regression | 0.19  | 0.6714   |

---

## Local Setup

### 1. Clone the repo

```bash
git clone https://github.com/your-username/house-price-prediction.git
cd house-price-prediction

2. Create virtual environment (optional but recommended)
bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # on Windows: venv\Scripts\activate

3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt

4. Run the app locally
bash
python app.py
or using Gradio:

bash

python app.py

## Requirements
See requirements.txt, which includes:

gradio
numpy
pandas
xgboost
scikit-learn
joblib
matplotlib
seaborn


✍️ Author
Tamanna Aggarwal
