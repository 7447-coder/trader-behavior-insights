# trader-behavior-insights
Analysis of trader behavior using market sentiment
# Trader Behavior Insights: Market Sentiment Analysis

## 📌 Project Overview
This project analyzes the relationship between **trader performance** and **Bitcoin market sentiment** (Fear & Greed Index).  
By combining historical trader data from Hyperliquid with daily market sentiment, the goal is to uncover behavioral patterns that can inform smarter trading strategies.

This assignment is part of the **Junior Data Scientist – Trader Behavior Insights** hiring process.

---

## 📂 Datasets Used

### 1. Historical Trader Data (Hyperliquid)
Key columns:
- Account
- Coin
- Execution Price
- Size Tokens
- Size USD
- Side (Buy/Sell)
- Timestamp IST
- Closed PnL

### 2. Bitcoin Market Sentiment (Fear & Greed Index)
- date
- classification (Fear / Greed)

---

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🔄 Methodology

1. **Data Loading**
   - Imported both datasets using pandas.

2. **Data Cleaning & Preprocessing**
   - Converted timestamp columns to datetime format.
   - Extracted trade date for merging.
   - Handled missing values safely using left joins.

3. **Data Integration**
   - Merged trader data with sentiment data based on trade date.

4. **Feature Engineering**
   - Created profit/loss indicator from Closed PnL.

5. **Exploratory Data Analysis (EDA)**
   - Analyzed PnL distribution by market sentiment.
   - Compared win rates during Fear vs Greed.
   - Studied average trade size under different sentiments.
   - Performed account-level performance analysis.

---

## 📊 Key Insights

- Traders tend to achieve **higher average profits during Greed periods**, indicating increased risk-taking.
- Losses are also more extreme during Greed, suggesting possible overconfidence.
- During Fear periods, traders reduce trade size, leading to lower volatility.
- A subset of traders performs consistently well during Fear, indicating disciplined and defensive strategies.

---

## ✅ Conclusion
Market sentiment plays a significant role in trader behavior and performance.  
Understanding these patterns can help design sentiment-aware trading strategies and improve risk management.

---

## 🚀 Future Work
- Include leverage-based risk analysis if data becomes available.
- Extend analysis with predictive modeling.
- Perform clustering to identify trader archetypes.

---



## Dataset Note

The original historical trader dataset is large (>100MB) and exceeds GitHub’s file size limit.
For this repository, a representative sample (`historical_data_sample.csv`) is included.

The full dataset was used locally for analysis and can be provided upon request.


