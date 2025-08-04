# AAL Stock Price Forecasting (2010–2025) 📈

Forecasting the daily opening stock prices of **American Airlines (AAL)** using both traditional statistical models and deep learning architectures.

---

## 🔍 Overview

This project aims to analyze and forecast the stock prices of American Airlines from **2010 to 2025**. The following models were implemented and compared:

* **ARIMA** (AutoRegressive Integrated Moving Average)
* **Simple RNN** (Recurrent Neural Network)
* **LSTM** (Long Short-Term Memory)
* **GRU** (Gated Recurrent Unit)

Performance metrics like **RMSE**, **MAPE**, **SMAPE**, and **MSLE** were used for evaluation.

---

## 📦 Project Structure

```
📁 AAL-Price-Prediction-2010-2025
├── Time Series Forecasting of AAL Stock Prices Using ARIMA and Deep Learning Models (2010–2025)  # Jupyter notebooks for modeling and evaluation
├── requirements.txt                                                                              # Python dependencies
├── README.md                                                                                     # Project overview
```

---

## 🧠 Models Implemented

| Model     | RMSE ↓     | MAPE (%) ↓ | SMAPE (%) ↓ | MSLE ↓        |
| --------- | ---------- | ---------- | ----------- | ------------- |
| **ARIMA** | **0.0079** | **2.94**   | **2.94**    | **0.0000424** |
| RNN       | 0.0085     | 3.20       | 3.23        | 0.0000487     |
| LSTM      | 0.0101     | 3.87       | 3.93        | 0.0000686     |
| GRU       | 0.0111     | 4.71       | 4.85        | 0.0000852     |

✅ **ARIMA(0,1,0)** outperformed all deep learning models on test data.

---

## 📌 Key Features

* Data Collection using **Yahoo Finance (yfinance)**
* Data Preprocessing: scaling, differencing
* White noise & stationarity testing (ADF, Ljung-Box)
* Hyperparameter tuning (grid search for ARIMA)
* Deep learning with **TensorFlow/Keras**
* Clear visualization of predictions vs actual

---

## 📊 Visualizations

* Time Series Plots
* ACF & PACF plots
* Predicted vs Actual plots for each model

---

## 🛠️ Technologies Used

* Python 3.12
* Pandas, NumPy, Scikit-learn
* Statsmodels (ARIMA)
* TensorFlow / Keras (RNN, LSTM, GRU)
* Matplotlib, Seaborn

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Error-Makes-Clever/AAL-Price-Prediction-2010-2025.git
cd AAL-Price-Prediction-2010-2025
```

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

> The **ARIMA(0,1,0)** model delivered the **most accurate and consistent** forecast for AAL opening prices from 2010 to 2025 across all key metrics.
> Among deep learning models, **RNN** showed stronger performance than LSTM and GRU, indicating that simpler architectures can still be effective on relatively linear, univariate data.
> Deep learning models may yield better results in the future if trained with additional external features like trading volume, news sentiment, or economic indicators.


