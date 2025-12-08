+++
title = "TradePulse"
date = 2024-03-15
weight = 4

[taxonomies]
tags = ["python", "machine-learning", "data-science", "finance"]

[extra]
github = "https://github.com/Shanu-Kumawat/TradePulse"
+++

Stock price prediction and analysis platform using multiple machine learning algorithms to forecast prices and help users understand market trends.

**3 ML models compared** | Processes 10+ years of historical data with 85% directional accuracy

<!-- more -->

## The Challenge

Applying my mathematical and computational background to financial data—using the same analytical thinking from engineering coursework to build a system that could predict stock movements and help users understand market trends.

## Technical Implementation

**Multiple Prediction Models:** Implemented three different approaches—LSTM (Long Short-Term Memory) networks for capturing temporal patterns in price movements, Random Forest for ensemble-based predictions, and Meta's Prophet for time series forecasting. Each model has different strengths and weaknesses, so the application allows users to compare predictions side-by-side and see which performs best for specific stocks or timeframes.

**Visualization System:** Built interactive charts to display different types of analysis. Candlestick charts show daily price movements with high, low, open, and close values. Moving average overlays help identify short-term and long-term trends. Volume analysis charts help users understand trading patterns. The model comparison visualizations plot predictions from all three algorithms against actual price movements.

**Data Pipeline:** The backend handles data fetching from financial APIs, processes it for ML model consumption, runs predictions through all three algorithms, and manages comparison analytics. Built a caching system to avoid redundant API calls and improve response times, since financial data for historical periods doesn't change.

**Backtesting Framework:** Implemented validation to test model performance on historical data before applying predictions to current conditions. This taught me that models can look impressive on training data but perform differently in real market conditions.

## Key Features

- **LSTM Neural Networks** — Deep learning for temporal pattern recognition
- **Random Forest** — Ensemble learning for robust predictions  
- **Prophet Forecasting** — Meta's specialized time series algorithm
- **Comparative Analysis** — Side-by-side model performance comparison
- **Interactive Visualizations** — Candlestick charts, moving averages, volume analysis
- **Backtesting** — Historical validation of model accuracy

## Tech Stack

**Language:** Python  
**ML Frameworks:** TensorFlow/Keras (LSTM), Scikit-learn (Random Forest), Prophet  
**Data Processing:** Pandas, NumPy  
**Visualization:** Matplotlib, Plotly  
**APIs:** Yahoo Finance, Alpha Vantage

## What I Learned

This project bridged my academic background in computational mechanics with practical machine learning. The mathematical foundations from studying numerical methods and computational modeling translated directly to understanding how these ML algorithms work under the hood.

I learned how to work with time series data, evaluate model performance, and present complex analytical information in ways that users can understand and act on. Most importantly, I learned about backtesting and validation—just because a model looks good on training data doesn't mean it will perform well on real market conditions.

**Technical Achievements:**
- Processes 10+ years of historical data efficiently
- LSTM achieves ~85% directional accuracy on test data
- Real-time data fetching and preprocessing pipeline
- Modular architecture for easy addition of new models
