# Real-time-stock-forecasting

## Description

📌 Project Description (Technical Version)

This repository contains an end-to-end deep learning time-series forecasting system using a Multivariate Multi-Step LSTM architecture trained on 10 years of historical OHLC data for a specific stock symbol.

All historical market data was:

• Programmatically retrieved using the Alpha Vantage API

• Persisted in PostgreSQL

• Engineered into rolling 60-day sequences

• Scaled using MinMax normalization

• The model predicts the next 10 future trading days of closing prices in a single forward pass, reducing recursive error accumulation.

The system includes:

• Automated live daily data ingestion

• PostgreSQL-backed historical storage

• Saved model and scaler persistence

• Real-time multi-step inference pipeline

This project reflects production-oriented ML engineering practices suitable for financial portfolio analytics and deployment scenarios.



Designed for portfolio monitoring and production deployment.

🚀 This system performs :-

📥 Live daily stock data ingestion from Alpha Vantage

🗄 PostgreSQL storage of historical OHLC data.

🧠 LSTM-based next-day closing price prediction

🔁 Automated daily execution

📊 Real-time inference using the most recent 60 trading days

The model captures temporal patterns in stock price movements using deep learning.


📦 Tech Stack

•  Python 3.x

• TensorFlow / Keras

• scikit-learn
 
• PostgreSQL

• psycopg2

• Alpha Vantage API

• dotenv



⚙️ Installation & Setup
1️⃣ Clone Repository
2️⃣ Create Virtual Environment
3️⃣ Install Dependencies
4️⃣ Configure Environment Variables


The system will :-

1.Fetch latest daily stock data

2.Insert into PostgreSQL

3.Retrieve last 60 days

4.Predict next-day closing price

🔄 Workflow

- Fetch latest daily OHLC from Alpha Vantage

- Insert or update record in PostgreSQL

- Retrieve latest 60 trading days

- Scale using saved MinMaxScaler

- Reshape for LSTM

- Predict next-day closing price

- Output prediction

Runs daily via:

Infinite loop (24-hour sleep), or
Cron job (recommended for production)



## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

AKSHAY KUMAR DHAR

Project Link: [https://github.com/username/real-time-stock-forecasting](https://github.com/username/real-time-stock-forecasting)
