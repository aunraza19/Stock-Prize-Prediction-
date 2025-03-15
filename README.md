## Stock-Prize-Prediction
# Stock Prize Prediction Using LSTM
# Overview

This project predicts Apple Inc. (AAPL) stock prices using a Long Short-Term Memory (LSTM) model. LSTMs are well-suited for time series forecasting, making them ideal for stock price prediction.

# Features

Fetches stock data from Yahoo Finance.

Preprocesses data by cleaning, normalizing, and splitting it.

Uses a 4-layer LSTM model with dropout for prediction.

Evaluates performance with Mean Absolute Error (MAE).

Visualizes original vs. predicted stock prices.

# Installation

Install the required dependencies:

pip install tensorflow keras pandas numpy matplotlib scikit-learn yfinance

# Dataset

Source: Yahoo Finance (AAPL stock data from 2015-present).

# Preprocessing:

Drop unnecessary columns.

Normalize stock prices between 0 and 1.

Split into 70% training and 30% testing data.

# Model Architecture

LSTM Layers: 4 layers with 50, 60, 80, and 120 units.

Dropout Layers: Prevent overfitting.

Dense Output Layer: Predicts stock price.

Loss Function: Mean Squared Error (MSE).

Optimizer: Adam.

# Training

Run the training script:

python train.py

Epochs: 50

Validation Split: 10%

Testing & Prediction

Run the evaluation script:

python evaluate.py

Mean Absolute Error (MAE) is computed.

Prediction Visualization:

Original vs. Predicted stock prices plotted.

# Visualization

Run the prediction script to plot results:

python predict.py

# Results

Predicted prices closely follow actual prices.

Minor deviations exist due to market volatility.

# Future improvements:

Add external factors (trading volume, market news).

Use Transformer-based models for better accuracy.
