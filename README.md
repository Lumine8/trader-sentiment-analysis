#  Trader Sentiment Analysis

##  Overview

In this project, the relationship between market sentiment (Fear-Greed Index) and the behavior and performance of a trader of cryptocurrencies is analyzed. The aim is to discover the patterns of behavior, compare the variations in performance under various sentiment conditions and provide actionable trading insights based on data science and machine learning methods.

---

##  Objectives

- Understand how market sentiment influences trader profitability
- Analyze behavioral changes in trading activity under different sentiment conditions
- Segment traders into behavioral archetypes
- Build a predictive model to estimate trader profitability outcomes

---

## Dataset Description

Two datasets were used:

### 1 Market Sentiment Data
- Fear–Greed classification by date
- Indicates overall market mood

### 2️ Historical Trader Data
Includes:
- Account ID
- Execution price
- Trade size
- Buy/Sell direction
- Closed Profit & Loss
- Trade timestamps

---

##  Methodology

###  Data Preparation
- Cleaned and standardized timestamps
- Merged sentiment and trading datasets
- Created daily trader-level metrics

###  Feature Engineering
Key features derived:
- Daily Profit/Loss per trader
- Trade frequency
- Average trade size
- Activity segmentation

---

## Exploratory Analysis

Key analysis performed:

- Trader performance across sentiment states
- Behavioral changes in trade frequency
- Profitability distribution under Fear vs Greed
- Activity-based trader segmentation

---

## Predictive Modeling

A Random Forest classifier was built to predict trader profitability buckets:

**Target Classes:**
- Loss
- Neutral
- Profit

**Features Used:**
- Market sentiment
- Trade frequency
- Average trade size

Evaluation included:
- Accuracy score
- Classification report
- Confusion matrix

---

## Trader Clustering (Bonus Analysis)

KMeans clustering was applied to identify behavioral archetypes:

### Identified Trader Types:
1. **Conservative Traders**
   - Low activity and smaller trades
   - Lower profitability

2. **Active Balanced Traders**
   - High activity with moderate risk
   - Stable performance

3. **Aggressive High-Value Traders**
   - Large positions and high exposure
   - Highest profitability

Cluster quality was validated using:
- Elbow method
- Silhouette score

---

##  Key Insights

- Trading activity increases significantly during fear-driven markets
- Extreme sentiment leads to higher volatility in trader performance
- High-frequency traders tend to achieve higher average profitability
- Position size and trading frequency strongly influence outcomes

---

##  Strategy Recommendations

1. **Avoid overtrading during extreme fear periods** to reduce risk exposure.
2. **Adopt structured high-frequency trading with risk controls** rather than sporadic trading.
3. **Limit aggressive leverage during emotionally volatile markets.**

---

## Tools & Technologies

- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Jupyter Notebook


---

## How to Run

1. Clone the repository
2. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
Open the Jupyter notebook and run all cells

---

### Conclusion

This study shows that the market sentiment plays a huge role in dictating the behavior of traders and the patterns of profits. Sentiment indicators of behavioral metrics are useful in creating smarter trading programs.

