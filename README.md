# 📈 Tesla Stock Price Prediction using LSTM

This repository contains a deep learning pipeline for predicting Tesla's stock closing prices using LSTM (Long Short-Term Memory) networks. The project features data preprocessing, model training, FastAPI deployment, and a Streamlit dashboard for visualization.

---

## 🚀 Features

- ✅ Tesla stock historical data processing
- 🧠 LSTM model trained on technical indicators
- 📊 Feature engineering with Moving Averages, RSI, and more
- 🌐 FastAPI-based real-time prediction service
- 📈 Streamlit dashboard for visualization and testing

---

## 🛠️ Tech Stack

- Python 3.10+
- TensorFlow / Keras
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- FastAPI
- Streamlit
- Docker & Nginx *(for deployment, optional)*

---

## 📁 Project Structure

```bash
.
├── Tesla_price_prediction_modelipynb.ipynb   # Notebook with model pipeline
├── app/
│   ├── main.py                               # FastAPI backend
│   └── model/                                # Trained model + scaler
├── dashboard/
│   └── streamlit_app.py                      # Streamlit frontend
├── requirements.txt                          # All dependencies
├── Dockerfile                                # For Docker deployment
└── README.md                                 # This file
```

---

## 📉 Model Summary

- **Architecture**: LSTM Recurrent Neural Network
- **Lookback Window**: 30 time steps (days)
- **Target Variable**: Tesla's `Close` price
- **Key Features**:
  - OHLCV
  - 30-day and 90-day Moving Averages
  - RSI (Relative Strength Index)
  - Hourly returns
  - Timestamp-based features (e.g., hour)

---

## 🧪 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/tesla-stock-lstm.git
cd tesla-stock-lstm
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Model / API / Dashboard

- Train the model using the notebook, or load the saved weights
- Launch the API:

```bash
uvicorn app.main:app --reload
```

- Launch the dashboard:

```bash
streamlit run dashboard/streamlit_app.py
```

---

## 🌐 Live Demo

- 🔗 Frontend: [https://waywise.co.uk](https://waywise.co.uk)
- 🧠 API: FastAPI server running behind Nginx *(optional)*

> Replace the links above with actual deployment URLs

---

## 📌 Roadmap

- [ ] Integrate additional macro and sentiment indicators
- [ ] Expand to multi-stock support
- [ ] Add backtesting and portfolio simulation
- [ ] Implement CI/CD pipelines for MLOps

---

## 👨‍💻 Author

**Chaitanya**  
🎓 BSc Computer Science Graduate  
🔗 [LinkedIn](https://www.linkedin.com/in/your-profile)  
🌍 [waywise.co.uk](https://waywise.co.uk)

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
