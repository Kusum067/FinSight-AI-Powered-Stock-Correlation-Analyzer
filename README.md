# 📊 FinSight: AI-Powered Stock Correlation Analyzer

A machine learning project that predicts the correlation between two financial assets using a hybrid ARIMA-LSTM model.
The goal is to help investors understand diversification risk and make smarter portfolio decisions by analyzing relationships between stocks.

---

# 🚀 Features

📊 Fetches real-time stock data using yfinance
📉 Calculates rolling correlation between assets
🤖 Uses ARIMA to capture linear trends in time series
🧠 Uses LSTM to model nonlinear patterns
🔗 Combines ARIMA + LSTM for improved prediction accuracy
🌐 Provides REST API using FastAPI for real-time predictions
📌 Generates actionable insights for portfolio diversification

---

# 🛠️ Tech Stack

Python 🐍
Pandas, NumPy → Data processing
Statsmodels → ARIMA modeling
TensorFlow / Keras → LSTM neural network
Matplotlib → Data visualization
FastAPI → Backend API
Google Colab → Development environment

---

# 📂 Project Workflow

### 1️⃣ Data Collection

Fetched historical stock data using yfinance API for selected assets (e.g., INFY, TCS, RELIANCE).

---

### 2️⃣ Data Preprocessing

Converted stock prices into returns
Computed rolling correlation between assets
Handled missing values and cleaned dataset

---

### 3️⃣ Time Series Modeling

Applied ARIMA model to capture linear components
Extracted residuals from ARIMA model

---

### 4️⃣ Deep Learning Modeling

Used LSTM neural network to learn nonlinear patterns from residuals
Trained model on sequential time-series data

---

### 5️⃣ Hybrid Model

Combined ARIMA predictions with LSTM output
Generated final correlation prediction

---

### 6️⃣ API Development

Built REST API using FastAPI
Enabled real-time prediction using endpoints

---

# 📊 Results

Final Model: ARIMA + LSTM Hybrid Model
Output: Predicted correlation value between two assets

Example:

```json
{
  "correlation": 0.80,
  "suggestion": "High correlation → avoid combining assets ⚠️"
}
```

📌 Impact:
Helps investors identify diversification opportunities and reduce portfolio risk

---

# 📌 How to Use

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/FinSight.git
```

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3️⃣ Run the API

```bash
uvicorn app:app --reload
```

---

### 4️⃣ Open in Browser

```bash
http://127.0.0.1:8000/docs
```

---

### 5️⃣ Test API

```bash
/predict?stock1=INFY.NS&stock2=TCS.NS
```

---

# 📈 Future Improvements

🚀 Pre-trained model deployment (avoid retraining on each request)
📊 Interactive dashboard (Streamlit / React)
📦 Multi-asset portfolio analysis
☁️ Cloud deployment (AWS / GCP)

---
