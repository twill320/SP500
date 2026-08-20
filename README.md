# S&P 500 Financial Market Visualizer

[![Python Version](https://img.shields.io/badge/Python-3.9+-3776AB?style=flat-square&logo=python&logoColor=white)]()
[![Pandas](https://img.shields.io/badge/Data-Pandas-150458?style=flat-square&logo=pandas&logoColor=white)]()
[![mplfinance](https://img.shields.io/badge/Visualization-mplfinance_|_Matplotlib-5f827d?style=flat-square)]()

A quantitative financial data analysis and visualization tool written in Python to track, model, and interpret market momentum and intraday volatility for the S&P 500 index.

---

## Overview

<div align="center">
  <img width="100%" alt="S&P 500 Candlestick and Volume Analysis Plot" src="https://github.com/user-attachments/assets/d5518694-3050-4b8d-aaad-302812c0e7dd" />
</div>

<br>

This project implements an automated data pipeline that ingests raw time-series market feeds, cleans and structures open-high-low-close-volume (OHLCV) datasets, and generates synchronized, publication-ready financial charts. By coupling directional price action with volume distributions on a shared timeline, the tool surfaces correlations between institutional market participation and asset valuation.

---

## Key Features

* **Quantitative Time-Series Pipeline:** Ingests and validates daily OHLCV records, correcting for missing intervals, splits, and timezone offsets using `pandas`.
* **Synchronized Multi-Panel Plots:** Uses dual-panel subplot geometry where daily trade volume bars are precisely aligned beneath primary candlestick price charts on a shared date axis.
* **Intraday Volatility & Momentum Indicators:** Visualizes daily price ranges via wick spreads and candlestick bodies to immediately signal buyer/seller dominance and reversal patterns.
* **Custom Dark Theme & Visual Hierarchy:** Engineered with high-contrast bullish/bearish color mapping, discrete grid lines, and legible typography to reduce visual fatigue during heavy analytical sessions.

---

## Tech Stack & Architecture

| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Core Runtime** | Python 3.9+ | Main application logic and data transformation pipeline |
| **Data Processing** | Pandas / NumPy | Time-series indexing, resampling, and dataframe cleanup |
| **Plotting Engine** | Matplotlib / mplfinance | Dual-axis rendering, custom gridlines, and figure export |

---

## Installation & Usage

**1. Clone the repository**
```bash
git clone [https://github.com/twill320/SP500.git
cd sp500-visualizer
