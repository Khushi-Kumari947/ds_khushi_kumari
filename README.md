# Trading Behavior Analysis with Fear–Greed Index  

This project explores how **market sentiment (Fear–Greed Index)** influences trading behavior and profitability. Using real transaction data combined with daily sentiment scores, we uncover patterns, correlations, and trader archetypes.  

---

##  Project Overview  
- **Goal:**  
  To analyze how market psychology (Fear vs. Greed) affects trader profitability, risk-taking, and behavior trends.  

- **Data Sources:**  
  - `fear_greed_index.csv` → Daily market sentiment values and classifications (Fear / Greed).  
  - `historical_data.csv` → Trader-level historical transactions including Closed PnL, timestamps, and accounts.  

- **Notebook:**  
  All analysis and visualizations are in `analysis.ipynb`.  

---

##  Key Insights  
1. **Profitability & Sentiment**  
   - Trades during **Greed** periods were more frequently profitable than during Fear.  
   - **Average Closed PnL** is positively correlated with sentiment index value.  

2. **Behavioral Trends**  
   - Traders showed **overconfidence** in Greed → higher profits but more risk-taking.  
   - **Loss aversion** in Fear → many closed trades prematurely, locking in losses.  
   - Evidence of **herding behavior** → most traders react after sentiment shifts.  

3. **Trader Segmentation (Clustering)**  
   - **Cluster A (Greed Specialists):** Profitable in Greed, lose in Fear.  
   - **Cluster B (Fear Survivors):** Manage steady performance even in Fear.  
   - **Cluster C (Consistent Losers):** Negative PnL in both conditions.  
   - **Cluster D (Balanced Traders):** Small but stable profits in both conditions.  

---

##  Tech Stack  
- **Python Libraries:**  
  - `pandas`, `numpy` → Data cleaning & transformation  
  - `matplotlib`, `seaborn` → Data visualization  
  - `scikit-learn` → Clustering (KMeans)  
  - `nbformat` → Notebook parsing  

---

##  Visualizations  
- Correlation plots (Closed PnL vs. Sentiment Index)  
- Dual-axis time series (Daily Avg Closed PnL vs. Sentiment Value)  
- Scatter plots with regression lines  
- Trader clustering (Fear vs. Greed profitability patterns)  

---

##  How to Run  
1. Clone the repo  
   ```bash
   git clone https://github.com/your-username/trading-sentiment-analysis.git
   cd trading-sentiment-analysis
