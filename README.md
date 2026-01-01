# 📊 Trader Sentiment Analysis  
### Understanding Trader Behavior Under Fear & Greed Market Conditions

![Bitcoin](https://img.shields.io/badge/Market-Bitcoin-orange)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Status](https://img.shields.io/badge/Status-Completed-success)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Project Overview

Financial markets are strongly influenced by **human emotions**, especially **Fear** and **Greed**.  
This project explores how market sentiment impacts **trader performance, risk-taking behavior, and trading outcomes** using real historical trading data combined with Bitcoin market sentiment indicators.

The goal is to **uncover hidden behavioral patterns** and deliver **data-driven insights** that can help design **smarter and more disciplined trading strategies**.

---

## 🧠 Problem Statement

> How does market sentiment (Fear vs Greed) influence trader behavior and performance?

Specifically, this project aims to:
- Analyze trader profitability under different sentiments
- Identify risk-taking and activity patterns
- Study win/loss behavior and performance stability
- Extract actionable insights for smarter trading decisions

---

## 📂 Datasets Used

### 1️⃣ Bitcoin Market Sentiment Dataset  
- **Source:** Fear & Greed Index  
- **Key Columns:**
  - `timestamp` – Unix timestamp of sentiment
  - `value` – Sentiment score (0–100)
  - `classification` – Fear / Greed label
  - `date` – Calendar date

### 2️⃣ Historical Trader Data (Hyperliquid)
- **Key Columns:**
  - `Account` – Trader identifier
  - `Execution Price` – Trade execution price
  - `Size USD` – Trade size (used as risk proxy)
  - `closedPnL` – Realized profit or loss
  - `Timestamp` – Trade execution time

---

## ⚙️ Methodology

### 🔹 Data Preparation
- Converted timestamps to a common **daily format**
- Merged sentiment and trade data using a **left join**
- Created a sentiment-aligned analysis dataset

### 🔹 Feature Engineering
- **Trade Outcome:** Win / Loss / Breakeven (based on `closedPnL`)
- **Risk Proxy:** Trade size in USD (`Size USD`)
- **Sentiment Simplification:** Extreme Fear → Fear, Extreme Greed → Greed

---

## 📈 Analysis Framework

The analysis was conducted in structured steps:

1. **Average PnL by Sentiment** – Profitability comparison  
2. **Trade Frequency Analysis** – Market activity patterns  
3. **Risk-Taking Behavior** – Position size comparison  
4. **Win vs Loss Distribution** – Trade success rates  
5. **Trader-Level Behavior** – Same trader under Fear vs Greed  
6. **Volatility Analysis** – Stability vs fluctuation of outcomes  

---

## 🔍 Key Insights

- 📈 **Greed** periods show higher average profitability but increased volatility
- ⚠️ Traders take **larger risks** during Greed
- 🛑 **Fear** leads to lower activity but more stable outcomes
- 🔄 The same trader behaves differently under different sentiments
- 🎯 Emotional trading often leads to inconsistent performance

---

## 💡 Practical Strategy Takeaways

- Control position sizing during Greed to avoid overexposure
- Maintain discipline during Fear to avoid panic-driven decisions
- Focus on consistency and risk management over short-term gains
- Use sentiment as a **contextual signal**, not a trading trigger

---

## 📊 Visualizations

The project includes multiple visualizations such as:
- Bar charts for profitability and trade frequency
- Boxplots for risk and PnL volatility
- Stacked bar charts for win/loss distribution
- Scatter plots for behavioral analysis

(All plots are generated using Matplotlib and Seaborn.)

---

## 🚀 Tech Stack

- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  

---

## ⚠️ Limitations & Future Scope

- Sentiment data is daily (no intraday sentiment)
- Explicit leverage data was unavailable
- Future improvements could include:
  - Risk-adjusted returns
  - Intraday sentiment analysis
  - Strategy backtesting

---

## 🏁 Conclusion

This project demonstrates that **market sentiment significantly influences trader behavior, risk-taking, and performance**.  
By converting emotional signals into data-driven insights, traders and platforms can design **smarter, emotion-aware strategies** that balance profitability with disciplined risk management.

---

## 📬 Contact

If you have questions or feedback, feel free to reach out.

📧 **Email:** sauvirwodehras3136@gmail.com  
🔗 **GitHub:** https://github.com/SauvirWodehra  

---

⭐ If you found this project insightful, feel free to star the repository!
