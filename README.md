# 📊 Cryptocurrency Price Prediction Using LSTM

🚀 Project Overview

This project implements a Time-Series Forecasting Model using Long Short-Term Memory (LSTM) networks to predict cryptocurrency prices.

The model analyzes historical price data of a cryptocurrency (e.g., Bitcoin) and forecasts future price movements based on learned patterns.

🎯 Objective

Collect historical cryptocurrency price data

Preprocess and normalize time-series data

Build and train an LSTM deep learning model

Predict future prices

Evaluate model performance using RMSE and MAE

Visualize actual vs predicted prices

🛠️ Technologies Used

Python

Google Colab

NumPy

Pandas

Matplotlib

Scikit-learn

TensorFlow / Keras

yFinance API

📂 Dataset

The dataset is fetched using the Yahoo Finance API via yfinance.

Example:

Bitcoin (BTC-USD)

Ethereum (ETH-USD)

Historical data includes:

Open

High

Low

Close

Volume

For prediction, the Close price is used.

🔄 Project Workflow

1️⃣ Data Collection

Download historical cryptocurrency data using yFinance.

2️⃣ Data Preprocessing

Select Close price

Normalize data using MinMaxScaler

Create 60-day time sequences

Reshape data for LSTM input

3️⃣ Model Building

Build Sequential LSTM model

Add Dropout layers to prevent overfitting

Compile using Adam optimizer

Loss function: Mean Squared Error

4️⃣ Model Training

Train model on historical data

Epochs: 20

Batch Size: 32

5️⃣ Prediction & Visualization

Predict prices

Inverse transform scaled data

Plot actual vs predicted prices

🧠 Model Architecture

LSTM Layer (50 units, return sequences=True)

Dropout (0.2)

LSTM Layer (50 units)

Dropout (0.2)

Dense Layer (1 unit)

📈 Evaluation Metrics

RMSE (Root Mean Squared Error)

MAE (Mean Absolute Error)

Lower values indicate better prediction accuracy.

📊 Output

Trained LSTM model

Actual vs Predicted Price Graph

Cryptocurrency price forecasting system

▶️ How to Run the Project

Open Google Colab

Install dependencies:

pip install yfinance


Run all notebook cells sequentially

View prediction results and visualization
<img width="868" height="547" alt="image" src="https://github.com/user-attachments/assets/3c3eee6e-facb-4c0f-94c3-6af61dac5c34" />
