# Assignment-Primetrade.AI
README — Bitcoin Sentiment vs Trader Performance Analysis
📍 Project Overview

This project analyzes how Bitcoin market sentiment (Fear vs Greed) impacts the trading performance of users on the Hyperliquid exchange. By combining sentiment data with historical trading records, the goal is to uncover patterns that influence profitability and risk behavior.

📂 Datasets Used
1️⃣ Bitcoin Market Sentiment Dataset
Column	Description
date	Calendar date
classification	Market sentiment label (Fear or Greed)
value (optional)	Numerical sentiment score
2️⃣ Hyperliquid Historical Trading Dataset
Column	Description
account	Trader wallet/account ID
coin	Asset being traded (BTC, etc.)
size tokens / size usd	Trade position size
side	Long or Short direction
timestamp	Timestamp of execution
closed pnl	Profit or loss realized
leverage (if available)	Position leverage / exposure
🛠️ Technical Workflow

Load both datasets

Clean and standardize column names

Convert timestamps to date format

Merge sentiment with trading data on date

Engineer new features for analysis

Win/Loss flag

% Return (PnL%)

Sentiment binary encoding (Fear=0, Greed=1)

Perform comparative analysis

Performance during Fear vs Greed

Long vs Short profitability by sentiment

Win-rate impact and behavioral patterns

📊 Key Insights & Questions Answered
Analysis Question	Purpose
Are traders more profitable in Fear or Greed?	Determine best market conditions
Do Longs or Shorts win more often depending on sentiment?	Strategy alignment
Does sentiment influence win-rate probability?	Risk-based deployment
Does leverage amplify gains/losses based on mood?	Optimal position sizing
📈 Core Metrics

Avg PnL by sentiment

Win rate % under Fear vs Greed

Long/Short performance breakdown

Risk-adjusted PnL based on leverage

💡 Early Observations (Example)

These will vary depending on your results — update after running analysis.

Greed periods show higher average profits, suggesting momentum-driven trend trading.

Fear periods often reward short strategies and disciplined risk control.

High leverage performs well in Greed markets but becomes destructive during Fear.

Sentiment classification may serve as a directional bias indicator.

📁 Files Included
File	Purpose
Sentiment_Trader_Analysis.ipynb	Full Colab notebook with code & analysis
fear_greed_index.csv	Sentiment dataset
historical_data.csv	Hyperliquid trades dataset
README.md	Project documentation
🚀 How to Run (Colab Instructions)

Upload both CSV files to /content/

Open the notebook:

Sentiment_Trader_Analysis.ipynb


Run all cells in order

View summary analytics at the end

📌 Future Improvements

Add chart visualizations (matplotlib/plotly)

Build a sentiment-driven PnL prediction model

Create automated trading signals based on Fear/Greed thresholds

Add real-time sentiment API integration

