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

📂 Project Structure
Nifty50-Stock-Screener/
│
├── nifty50_screener.ipynb      # Main Jupyter Notebook
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
├── images/                     # Screenshots (recommended)
│   ├── dropdown_ui.png
│   ├── output_sample.png
│   └── recommendation.png
└── LICENSE                     # Optional

🛠️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/<your-username>/Nifty50-Stock-Screener.git
cd Nifty50-Stock-Screener

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Launch Jupyter Notebook
jupyter notebook

4️⃣ Open
nifty50_screener.ipynb

🧠 How the Analysis Works
📌 Step 1 — Fetch Price Data

Downloads 2 years of daily OHLCV data.

📌 Step 2 — Compute Indicators

MA20, MA50, MA200

RSI(14)

📌 Step 3 — Fetch Live Price

Shows the latest available quote.

📌 Step 4 — Fetch Fundamentals

PE

ROE (%)

D/E Ratio

📌 Step 5 — Score the Stock

Each category contributes to final score:

Technical Scoring Examples
Condition	Score
Price > MA20 > MA50 > MA200	+2
Price < MA200	-1
RSI < 40	-1
RSI between 50–70	+1
Fundamental Scoring Examples
Condition	Score
PE ≤ 20	+1
PE > 35	-1
ROE ≥ 15%	+1
D/E ≤ 0.5	+1
📌 Step 6 — Final Recommendation
Total Score	Recommendation
≥ +3	BUY
+1 to +2	HOLD
≤ 0	SELL
🖥 Example Output
Analyzing RELIANCE (RELIANCE.NS)
------------------------------------------------------------
Last EOD Close: 2514.25
Live / Latest Quote: 2521.80
MA20: 2488.40, MA50: 2456.10, MA200: 2369.45
RSI14: 55.23

Fundamentals:
PE: 26.5
ROE: 14.8%
Debt/Equity: 0.35

=== RECOMMENDATION ===
Overall Score: 3  (Tech: 2, Fundamental: 1)
FINAL VIEW: BUY

Reasons (Technicals):
- Price > MA50 > MA200 → Uptrend
- RSI is healthy (55)

Reasons (Fundamentals):
- Reasonable valuation (PE=26)
- Healthy ROE
- Low leverage

📝 Future Improvements

Add candlestick charts

Add Bollinger Bands / MACD

Export results as PDF report

Compare stock vs sector average

Build a Streamlit web dashboard

Train ML models for prediction

📜 License

This project can be used, modified, or shared freely for educational or personal purposes.

❤️ Credits

Developed by Piyush Prabhat
Using Python, Pandas, NumPy, yFinance, TA-Lib, and ipyWidgets.
