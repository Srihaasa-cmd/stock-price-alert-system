# Stock Price Alert System

## Overview
Built a production level stock monitoring system that fetches 
real-time NSE stock prices via an official API, stores historical 
data in a SQLite database, calculates trading signals and sends 
automated Gmail alerts when prices breach user-defined thresholds.

## Problem Statement
Investors manually check stock prices multiple times a day 
wasting time and often missing critical price movements. 
This system automates monitoring and alerts instantly.

## Features
- Fetches real-time stock prices from Alpha Vantage official API
- Stores historical price data in SQLite database
- Calculates 7-day and 21-day moving averages
- Generates BULLISH or BEARISH signals based on moving average crossover
- Sends automated Gmail alerts when stocks cross target prices
- Saves daily analysis report as CSV
- Visualises price history with moving averages and alert levels

## Key Concepts Used
- **Moving Average** — smooths daily price noise to show real trend
- **Golden Cross** — when 7-day MA crosses above 21-day MA = bullish signal
- **Death Cross** — when 7-day MA crosses below 21-day MA = bearish signal
- **Price Alerts** — automated notifications on threshold breaches

## Tools Used
- Python
- Requests — API calls to Alpha Vantage
- Pandas — data cleaning and analysis
- SQLite3 — local database storage
- Matplotlib — price history charts
- SMTP — automated Gmail alerts
- Alpha Vantage API — official real-time stock data

## Files
- `Stock_Alert.ipynb` — main project notebook
- `stock_monitor.png` — stock price charts with signals
- `stock_report.csv` — latest analysis report
- `stocks.db` — SQLite database with price history

## How to Run
1. Get free API key from alphavantage.co
2. Clone this repository
3. Open `Stock_Alert.ipynb` in Jupyter Notebook
4. Replace API key in Cell 2
5. Add Gmail app password in Cell 7
6. Run all cells top to bottom

## API Used
Alpha Vantage — Free official financial data API
Get your free key at alphavantage.co

## Dataset
Real-time NSE stock data — Reliance, TCS — fetched live via API
