# 🚦 Traffic Congestion Prediction using XGBoost

This project focuses on predicting **traffic congestion levels** using the **XGBoost regression algorithm**. The analysis and modeling were conducted in Google Colab. The goal is to build a reliable model that forecasts congestion based on temporal, weather, and traffic features.

---

## 📋 Project Overview

The dataset contains time-based and weather-related features such as:
- `date_time` (timestamp)
- `is_holiday` (binary flag)
- `weather_type` (categorical weather description)
- `temperature`, `humidity`, `wind_speed`
- `avg_speed` (average vehicle speed)
- `avg_volume` (average traffic volume)

**Target variable**: `congestion` (numerical congestion level)

---

## ⚙️ Methods Used

1. 🧼 **Data Preparation**
   - Feature extraction from datetime (`day`, `hour`, `weekday`)
   - One-hot encoding of categorical features (e.g., `weather_type`)
   - Scaling of numeric features using `MinMaxScaler`

2. 📈 **Modeling**
   - `XGBoostRegressor` used for regression
   - Evaluation metrics:
     - RMSE (Root Mean Squared Error)
     - MAE (Mean Absolute Error)
     - R² Score
   - Model validated using **5-fold cross-validation**

---

## 🧠 Results

Average metrics from 5-fold cross-validation:
- **RMSE:** ~6.53  
- **MAE:** ~5.03  
- **R² Score:** ~0.72

✅ These results show the model performs reasonably well and could serve as a foundation for real-time traffic prediction systems.

---

## 🔧 Technologies

- 🐍 Python 3 (Google Colab)
- 📦 Pandas, NumPy
- 📊 Matplotlib, Seaborn
- 🧪 Scikit-learn
- ⚡ XGBoost

---

## ▶️ Run the Notebook

Open in Google Colab:  
📎 [Open Notebook](https://colab.research.google.com/drive/1TRJDGhQju-BqhzLNmT8vi-rM4elUh6PK?usp=sharing)
