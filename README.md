# Ethereum Price Analysis with Machine Learning

## Overview
This repository contains a detailed analysis of **Ethereum (ETH) price trends** using machine learning techniques and statistical analysis. The work includes data visualization, time-series forecasting, and predictive modeling to understand ETH price movements. 

## Contents
### **1. Documents and Code**
- **`ETHPrice_DSBDA Paper.pdf`**  
  - A research paper analyzing Ethereum price trends using various machine learning algorithms. 
  - Covers data collection, feature engineering, model selection, evaluation, and results.
  
- **`Eth_analysis - Jupyter Notebook.pdf`**  
  - A Jupyter Notebook capturing exploratory data analysis (EDA), moving averages, candlestick charts, and return calculations for Ethereum.
  - Uses Python libraries (`pandas`, `matplotlib`, `seaborn`, `mplfinance`).

- **`ETH-USD.csv`**  
  - Historical Ethereum price data, including Open, High, Low, Close prices, and Trading Volume.
  - Used for training machine learning models and visualizing ETH price trends.

## **Project Methodology**
### **1. Data Preprocessing**
   - Load Ethereum price dataset (`ETH-USD.csv`).
   - Remove unnecessary columns (`Adj Close`).
   - Compute moving averages (100-day MA) for trend analysis.

### **2. Exploratory Data Analysis (EDA)**
   - Visualize price trends over time.
   - Analyze trading volume and total traded value.
   - Identify significant price fluctuations.

### **3. Candlestick Charting**
   - Generate candlestick charts for Ethereum’s price movement.
   - Highlight price increase (green) and decrease (red) using `mplfinance`.

### **4. Returns Calculation**
   - Compute daily percentage change in Ethereum prices.
   - Analyze volatility trends.

### **5. Machine Learning Models** *(Discussed in Paper)*
   - Regression models (Linear, ARIMA, LSTM, Random Forest, etc.)
   - Sentiment analysis for ETH price predictions.
   - Model evaluation using MSE, RMSE, R² score.

## **Installation & Usage**
To run the analysis on your local system, follow these steps:

### **1. Clone the Repository**
```bash
 git clone https://github.com/your-username/ethereum-price-analysis.git
 cd ethereum-price-analysis
```

### **2. Install Dependencies**
Ensure Python is installed, then install the required libraries:
```bash
pip install numpy pandas matplotlib seaborn mplfinance
```

### **3. Run the Jupyter Notebook**
If using Jupyter:
```bash
jupyter notebook
```
Then open `Eth_analysis.ipynb` and execute the code cells.

If running as a Python script:
```bash
python eth_analysis.py
```

## **Results & Insights**
The analysis produced significant insights into Ethereum price behavior. Key findings include:

- **Price Trends:** The Ethereum price has seen substantial fluctuations, with major spikes observed during market surges in 2017 and 2021.
- **100-Day Moving Average:** The moving average helped smooth price variations and provided insights into long-term trends.
- **Trading Volume Influence:** High trading volumes correlate with increased price volatility, indicating strong market reactions to high-activity periods.
- **Highest Trading Day:** The highest trading activity was recorded on **May 13, 2021**, with a total traded value surpassing **$300 billion**.
- **Candlestick Patterns:** Green candles indicate price growth, while red candles indicate declines, providing insights into bullish and bearish trends.
- **Daily Returns Analysis:** High variance in daily returns suggests a volatile market, making Ethereum a high-risk, high-reward asset.
- **Model Performance:**
  - **ARIMA** showed moderate performance but struggled with sudden spikes.
  - **LSTM** outperformed traditional models by capturing long-term dependencies.
  - **Random Forest Regression** provided strong feature importance analysis but lacked temporal understanding.

## **Future Improvements**
- Implement **deep learning models (LSTM, Transformer)** for improved predictions.
- Integrate **macro-economic indicators (inflation, Bitcoin price, regulations)**.
- Perform **real-time Ethereum price analysis using API-based live data**.
- Explore **reinforcement learning techniques for adaptive trading strategies**.

## **Contributors**
- **Shreyas Khandale** – Research & Development
- **Rohan Patil** – Machine Learning & Financial Analysis

## **License**
This project is licensed under the **MIT License**.
