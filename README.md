# Fully-Automated-Nifty-50-Stock-Screener-using-Python-yFinance
📈 Nifty 50 Stock Screener (Python)
Live Price Analysis + Technical Indicators + Fundamental Metrics + Automated Buy/Hold/Sell Recommendation
🚀 Project Overview

This project is a fully automated stock analysis system built using Python.
It analyzes all Nifty 50 companies and gives a real-time Buy / Hold / Sell recommendation based on:

📉 Technical Indicators

📊 Fundamental Metrics

💹 Live Market Prices

🔍 Rule-based scoring model

The tool runs inside a Jupyter Notebook and includes an interactive dropdown UI to instantly analyze any stock from the Nifty 50.

🎯 Features
🔹 1. Real-Time Price Fetching

Fetches near-live/latest market price via yfinance.Ticker.fast_info and .info

Displays both last EOD close and latest live quote

🔹 2. Technical Indicator Analysis

Automatically calculates:

20-day Moving Average (MA20)

50-day Moving Average (MA50)

200-day Moving Average (MA200)

RSI-14 (Relative Strength Index)

🔹 3. Fundamental Analysis (Live from yFinance)

Pulls key company fundamentals:

PE Ratio

ROE (%)

Debt/Equity Ratio

🔹 4. Scoring & Recommendation System

Rule-based scoring across:

Trend

Momentum

Valuation

Profitability

Leverage

Output:

BUY

HOLD

SELL

🔹 5. Clear Human-Readable Explanations

The tool prints:

Why the score was given

Technical reasons

Fundamental reasons

Final interpretation

🔹 6. Interactive User Interface

A dropdown menu lets you select any Nifty 50 company.
Analysis runs instantly and fetches fresh data each time.
