# Cryptocurrency Time Series Analysis: Bitcoin & Ethereum  

## Overview  
This project involves analyzing **6 years** of historical cryptocurrency data (2017–2023) to uncover trends, correlations, and patterns in Bitcoin and Ethereum price movements. It demonstrates expertise in time series analysis, data visualization, and merging datasets for comparative analysis.  

## Key Highlights  
- **Analyzed Data:** Processed and explored **over 2 million rows** of data.  
- **Techniques Used:**  
  - Time series resampling (daily, weekly, monthly averages).  
  - Rolling averages and Exponential Weighted Moving Averages (EWM).  
  - Correlation analysis to identify relationships between Bitcoin and Ethereum.  
- **Visualizations:** Created **10+** detailed plots to compare trends, including price movements in specific months and aggregated statistics.  

## Datasets  
- **Bitcoin Data:** Historical prices of Bitcoin from 2017 to 2023 (`bitcoin_2017_to_2023.csv`).  
- **Ethereum Data:** Historical prices of Ethereum (`ETH-USD.csv`).  

## Technologies  
- **Programming Language:** Python  
- **Libraries:**  
  - `pandas` for data manipulation and resampling.  
  - `matplotlib` for visualizations.  
  - `numpy` for numerical operations.  

## Key Code Snippets  

### 1. Time Series Analysis  
```python
# Load Bitcoin data
bitcoin = pd.read_csv('bitcoin_2017_to_2023.csv', index_col='timestamp', parse_dates=True)

# Resample and plot weekly and monthly trends
plt.figure(figsize=(12,7))
bitcoin.loc['2021', 'close'].plot()
bitcoin.loc['2021', 'close'].resample('W').mean().plot(label='Weekly Average', ls=':', lw=4, c='green')
bitcoin.loc['2021', 'close'].resample('M').mean().plot(label='Monthly Average', ls='--', lw=3, c='orange')
plt.legend()
plt.show()
