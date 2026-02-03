# 📊 Trader Sentiment Analysis  
### Exploring Trader Behavior Under Fear & Greed Market Conditions

---

## 📌 Project Overview

Financial markets are strongly influenced by **human emotions**, particularly **Fear** and **Greed**.  
This project analyzes how market sentiment impacts **trader performance, trading behavior, risk-taking, and outcome stability** by combining Bitcoin market sentiment data with real historical trading data from Hyperliquid.

The goal is to **uncover hidden behavioral patterns** and deliver **data-driven insights** that can guide **smarter and more disciplined trading strategies**.

---

## 🧠 Problem Statement

The objective of this project is to explore the relationship between **market sentiment (Fear vs Greed)** and:

- Trader profitability  
- Trading activity  
- Risk-taking behavior  
- Win/loss outcomes  
- Stability and consistency of performance  

---

## 📂 Datasets Used

### 1️⃣ Bitcoin Market Sentiment Dataset
This dataset captures **daily market emotion** for Bitcoin.

**Key columns:**
- `timestamp` – Unix timestamp of sentiment
- `value` – Sentiment score (0–100)
- `classification` – Market emotion (Fear / Greed)
- `date` – Calendar date

---

### 2️⃣ Historical Trader Data (Hyperliquid)
This dataset captures **real executed trades**.

**Key columns:**
- `Account` – Trader identifier
- `Execution Price` – Trade execution price
- `Size USD` – Trade size (used as risk proxy)
- `closedPnL` – Realized profit or loss
- `Timestamp` – Trade execution time

---

## ⚙️ Setup & How to Run

### Step 1: Clone the Repository
```bash
git clone https://github.com/your-username/Trader_Sentiment_Analysis.git
cd Trader_Sentiment_Analysis
Run the Project
jupyter notebook
Open this Notebook
trader_sentiment_analysis.ipynb


## 1️⃣ Data Preparation & Feature Engineering

The sentiment and trade datasets were first aligned to a common **daily date format** to enable accurate merging. A left join was used to combine trade-level data with daily market sentiment while preserving all trade records.  
A separate analysis-ready dataset was created containing only trades with available sentiment information.

Key features engineered include:
- **Trade Outcome**: Each trade was classified as Win, Loss, or Breakeven based on realized closed PnL.
- **Risk Proxy**: Trade size in USD was used as a proxy for risk exposure, as explicit leverage data was unavailable.
- **Sentiment Simplification**: Extreme Fear and Fear were grouped as Fear, and Extreme Greed and Greed were grouped as Greed.

---

## 2️⃣ Analysis Framework

A structured analysis framework was applied to study trader behavior under Fear and Greed:

- **Average PnL by Sentiment** to compare profitability
- **Trade Frequency Analysis** to understand trader activity
- **Risk-Taking Analysis** using trade size as risk exposure
- **Win vs Loss Distribution** to evaluate trade success rates
- **Trader-Level Behavioral Analysis** to study how the same trader behaves under different sentiments
- **Stability and Volatility Analysis** to assess consistency of outcomes

---

## 3️⃣ Outputs Generated

### Charts
- Average Closed PnL by Market Sentiment  
- Trade Frequency under Fear vs Greed  
- Risk (Trade Size USD) Distribution  
- Win vs Loss Distribution by Sentiment  
- Risk vs PnL Scatter Plot  
- PnL Volatility by Sentiment  

### Tables
- Average PnL by Sentiment  
- Trade Count by Sentiment  
- Average Risk by Sentiment  
- Win/Loss Percentage Distribution  
- Trader-Level Behavioral Metrics  
- Volatility Metrics by Sentiment  

(All outputs are generated within the Jupyter notebook.)

---

## 4️⃣ Short Write-Up Summary

### Methodology
Daily Bitcoin market sentiment data was aligned with trade-level historical data. Feature engineering was performed to define trade outcomes, risk exposure, and simplified sentiment categories. The analysis compared profitability, activity, risk, behavior, and stability under Fear and Greed conditions.

---

### Key Insights
- Greed periods show higher average profitability and trading activity.
- Traders take larger risks during Greed, leading to higher volatility.
- Fear periods exhibit lower activity but more stable outcomes.
- The same trader often changes behavior based on market sentiment.
- Higher profits during Greed are frequently accompanied by instability.

---

### Strategy Recommendations
- Limit position size during Greed to avoid overexposure.
- Maintain discipline during Fear to avoid panic-driven decisions.
- Focus on consistency and risk management rather than short-term gains.
- Use market sentiment as contextual guidance, not a direct trading signal.

---

### Limitations & Future Scope
- Sentiment data is available only at a daily level.
- Explicit leverage information was unavailable.
- Future work may include risk-adjusted returns, intraday sentiment, and strategy backtesting.

---

### Conclusion
The analysis confirms that market sentiment significantly influences trader behavior, risk-taking, and performance. Understanding these sentiment-driven patterns can help traders and platforms design smarter, emotion-aware strategies that balance profitability with disciplined risk management.

---

## 🚀 Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  

---

## 📬 Contact
📧 Email: sauvirwodehras3136@gmail.com  
🔗 GitHub: https://github.com/SauvirWodehra  

