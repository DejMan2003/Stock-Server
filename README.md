# Stock-Server
# Stock Volatility Prediction Model (VFV.TO, AAPL, GOOGL)

This project builds a machine learning model that predicts short-term market volatility using data from three major tickers: **VFV.TO (S&P 500 ETF), AAPL, and GOOGL**.  
The goal is to generate a simple **investment-risk alert system** based on historical price behaviour and technical indicators.

## 🔍 Project Overview
The model downloads historical daily data and engineers several key features:
- Daily returns  
- Rolling 10-day volatility  
- RSI (Relative Strength Index)  
- Future volatility (5-day forward window)

Volatility is then classified into:
- **Low**
- **Medium**
- **High**

A **Random Forest classifier** predicts these categories and assigns a probability that volatility will be **High**, generating a traffic-light alert:
- **RED** → High risk  
- **YELLOW** → Moderate risk  
- **GREEN** → Low risk  

## 📊 Features Included
- Automated data extraction with `yfinance`
- Technical analysis indicators (Volatility + RSI)
- Train/test split for proper evaluation
- Classification model with probability scoring
- Visualization of price movements and predictions

## 🧠 Machine Learning Model
- **Model:** Random Forest Classifier  
- **Labels:** Volatility tiers via quantile cuts  
- **Evaluation:** Classification report (precision, recall, f1)

## 📈 Visualizations
- Ticker price history (VFV.TO, AAPL, GOOGL)
- Last 20 predictions with alert output

## 🚀 How To Run
1. Install dependencies:
