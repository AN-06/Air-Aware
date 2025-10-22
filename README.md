# 🌍 Air Aware — Smart Air Quality Prediction System

## 🧩 Milestone 1: Data Collection & Preprocessing

### 🔹 Overview
Collected and preprocessed historical air quality data to prepare for time-series forecasting of **AQI** and major pollutants.

### 📊 Data Source
- [World Air Quality Dataset (Kaggle)](https://www.kaggle.com/datasets/mexwell/world-air-quality)
- Accessed using **Kaggle API** in **Google Colab**

### 🧹 Key Steps
- Parsed timestamps and selected key columns  
- Resampled data (daily) and handled missing values (interpolation + fill)  
- Removed outliers using **IQR clipping**  
- Normalized pollutant values with **MinMaxScaler**  
- Added temporal features → `dayofweek`, `month`, `season`

### 📈 Output
- Cleaned dataset saved as **`openaq_preprocessed_daily.csv`**
- Basic **EDA** done: distributions, correlations, and sample time-series trends  
---

## 🧩 **Milestone 2: Model Training & Evaluation**

### 🔹 **Overview**  
Trained and compared three forecasting models — **ARIMA**, **Prophet**, and **LSTM** — to predict daily **PM2.5** pollutant levels.

### 🧠 **Key Steps**  
- Split dataset into **80% train** and **20% test**  
- Trained **ARIMA (5,1,2)**, **Prophet**, and **LSTM** models  
- Evaluated performance using **RMSE** and **MAE**  
- Visualized forecasts and compared model accuracy  
- Selected and saved the **best model** for inference  

### 📈 **Results**  
- **ARIMA** performed best for short, stable data  
- **Prophet** struggled due to lack of seasonality  
- **LSTM** underperformed due to limited data
  
---
---

💾 **Output**  
- **Best model:** ARIMA  
- **Saved as:** `best_model_arima.pkl` (using **joblib**)  

