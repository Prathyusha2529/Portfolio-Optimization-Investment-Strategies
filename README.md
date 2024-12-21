**Portfolio Optimization and Investment Strategies**

## 📌 Project Overview
This project explores multiple investment strategies to maximize portfolio returns while managing risks. By analyzing stock data from three distinct sectors—**Consumer Staples**, **Healthcare**, and **Communication Services**—over the period of 2017–2021, we employed techniques such as **Buy and Hold**, **Momentum Trading**, and **Portfolio Optimization**. The goal was to uncover valuable insights into the dynamics of the stock market and evaluate the effectiveness of various strategies.

## 🛠️ Workflow

### 1. **Data Collection**
   - Selected **30 stocks** from three sectors.
   - Utilized the **Yahoo Finance API** to gather historical data from January 1, 2017, to December 31, 2021.
   - Focused on **Adjusted Close Prices**, ensuring accurate representation of stock value trends over time.

### 2. **Data Preparation and Cleaning**
   - Created a ticker list and organized the stock data in a **dataframe** for analysis.
   - Extracted **daily adjusted closing prices** and computed **percentage changes** to analyze stock performance.
   - Calculated **8-day** and **21-day moving averages** for momentum analysis, dropping null values resulting from the rolling calculations.

### 3. **Exploratory Data Analysis (EDA)**
   - Visualized stock performances for each sector from 2017 to 2021.
   - Identified key performing stocks, such as:
     - **Consumer Staples:** SJM, WMT
     - **Healthcare:** BIIB, ELV
     - **Communication Services:** CHTR, GOOGL
   - Analyzed trends and variability to prepare for strategy implementation.

### 4. **Investment Strategies**
   - **Buy and Hold Strategy:**
     - Tracked **log closing values** and cumulative returns for long-term performance.
     - Evaluated portfolio returns over the three-year period.
   - **Momentum Trading Strategy:**
     - Used **8-day and 21-day moving averages** to identify buying/selling opportunities.
     - Introduced a **signal column** to differentiate investment days.
     - Calculated **momentum trading returns** and compared them with Buy and Hold.

### 5. **Top Stock Selection**
   - Based on performance metrics, narrowed down to **Top 9 Stocks** (3 per sector).
   - Further refined this list for portfolio optimization.

### 6. **Portfolio Optimization**
   - Calculated **covariance matrix** to measure stock variability and interdependencies.
   - Employed optimization models to:
     - Minimize risk.
     - Allocate investment proportions for maximum returns.
   - Tested risk limits and derived an **optimal risk level** (0.000246) for balanced allocation.

### 7. **Comparison and Benchmarking**
   - Compared portfolio performance against the **S&P 500 Index**, a widely recognized market benchmark.
   - Repeated Buy and Hold and Momentum Trading strategies on the S&P 500 for direct comparison.

### 8. **Final Analysis**
   - Evaluated the risk-return trade-offs of all strategies.
   - Analyzed cumulative portfolio returns and individual stock contributions.

## ✨ Key Features

- **Sector-Wise Insights:**
  - Identified sector leaders such as CHTR in Communication Services and SJM in Consumer Staples.
    
- **Strategy Evaluation:**
  - Momentum Trading outperformed Buy and Hold in the short term, especially for S&P 500 stocks.
  - MPT-based portfolios showed balanced risk-return performance over time.
    
- **Optimization:**
  - Effective use of covariance and risk limits to achieve an optimal portfolio.
    
- **Visualization:**
  - Sector and portfolio performance charts for easy interpretation.
    
- **Risk Analysis:**
  - Detailed exploration of variability and risk levels to ensure sustainable portfolio growth.


## 🧰 Tools and Technologies

- **Programming Language:** Python
- **Optimization Library:** Pyomo
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib
- **Data Source:** Yahoo Finance API

---

## 💡 Insights and Learnings

1. **Buy and Hold Strategy:**
   - Better suited for long-term investment, providing stable returns over time.
2. **Momentum Trading:**
   - Ideal for capturing short-term gains but requires active management and incurs higher risk.
3. **Optimization Models:**
   - Balancing risk and return is crucial for sustained portfolio performance.
4. **Sector Behavior:**
   - Stocks from Communication Services displayed higher variability compared to others.


## 🔭 Future Enhancements

- Integrate **machine learning models** for stock selection and risk prediction.
- Incorporate **macroeconomic indicators** for a holistic analysis.
- Extend analysis to include momentum trading for MPT-based portfolios.
- Explore real-time data integration for dynamic strategy testing.

