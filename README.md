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


