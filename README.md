# AAL Stock Price Forecasting (2010–2025) 📈

Forecasting the daily opening stock prices of **American Airlines (AAL)** using both traditional statistical models and deep learning architectures.

---

## 🔍 Overview

This project aims to analyze and forecast the stock prices of American Airlines from **2010 to 2025**. The following models were implemented and compared:

- **ARIMA** (AutoRegressive Integrated Moving Average)
- **Simple RNN** (Recurrent Neural Network)
- **LSTM** (Long Short-Term Memory)
- **GRU** (Gated Recurrent Unit)

Performance metrics like **RMSE**, **MAPE**, **SMAPE**, and **MSLE** were used for evaluation.

---

## 📦 Project Structure

```

📁 AAL-Price-Prediction-2010-2025
├── Time Series Forecasting of AAL Stock Prices Using ARIMA and Deep Learning Models (2010–2025)            # Jupyter notebooks for modeling and evaluation
├── requirements.txt                                                                                        # Python dependencies
├── README.md                                                                                               # Project overview

````

---

## 🧠 Models Implemented

| Model   | RMSE ↓     | MAPE (%) ↓ | SMAPE (%) ↓ | MSLE ↓       |
|---------|------------|-------------|--------------|---------------|
| **ARIMA** | **0.0079** | **2.95**   | **2.94**     | **0.0000427** |
| LSTM    | 0.0104     | 4.15       | 4.19         | 0.0000732     |
| RNN     | 0.0120     | 5.46       | 5.26         | 0.0000989     |
| GRU     | 0.0186     | 9.23       | 8.70         | 0.0002408     |

✅ **ARIMA(0,1,0)** outperformed all deep learning models on test data.

---

## 📌 Key Features

- Data Collection using **Yahoo Finance (yfinance)**
- Data Preprocessing: scaling, differencing
- White noise & stationarity testing (ADF, Ljung-Box)
- Hyperparameter tuning (grid search for ARIMA)
- Deep learning with **TensorFlow/Keras**
- Clear visualization of predictions vs actual

---

## 📊 Visualizations

- Time Series Plots
- ACF & PACF plots
- Predicted vs Actual plots for each model

---

## 🛠️ Technologies Used

- Python 3.12
- Pandas, NumPy, Scikit-learn
- Statsmodels (ARIMA)
- TensorFlow / Keras (RNN, LSTM, GRU)
- Matplotlib, Seaborn

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Error-Makes-Clever/AAL-Price-Prediction-2010-2025.git
cd AAL-Price-Prediction-2010-2025
````

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run Jupyter notebooks

```bash
jupyter notebook
```

---

## 🧾 Conclusion

> The ARIMA(0,1,0) model provided the **most accurate** forecast of AAL opening prices from 2010 to 2025.
> While deep learning models like LSTM and GRU showed promise, they require rich features to outperform statistical models in this case.

---
