# 📊 Market Sentiment vs Trader Behavior Analysis

## 🎯 Objective
This project analyzes how market sentiment (Fear vs Greed) influences trader behavior and performance in cryptocurrency markets. The goal is to determine whether sentiment impacts profitability directly or indirectly through changes in trading behavior.

---

## 💡 Motivation
Financial markets are strongly influenced by human psychology. In highly volatile crypto markets, sentiment (fear or greed) can drive trading decisions. This project aims to quantify how sentiment affects trader actions such as leverage, trade frequency, and positioning.

---

## 📁 Datasets

1. **Bitcoin Market Sentiment (Fear/Greed Index)**  
   https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing  

2. **Historical Trader Data (Hyperliquid)**  
   https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing  

---

## ⚙️ Methodology

### 1. Data Preparation
- Loaded and inspected both datasets
- Checked for missing values and duplicates
- Converted timestamps to a common daily format

### 2. Feature Engineering
- **Performance Metrics**: Daily PnL, win rate  
- **Behavioral Metrics**: Trade frequency, leverage, position size, long/short ratio  

### 3. Data Alignment
- Aggregated trading data at daily level
- Merged with sentiment data using date

### 4. Exploratory Analysis
- Compared trader performance and behavior across Fear vs Greed conditions
- Visualized distributions and trends

### 5. Statistical Analysis
- Conducted a t-test to evaluate differences in PnL  
- **Result:** p-value = 0.248 → Not statistically significant

### 6. Trader Segmentation
- Segmented traders based on leverage and activity
- Applied clustering (KMeans) to identify behavioral groups

---

## 📊 Key Insights

- No statistically significant difference in PnL between Fear and Greed days  
- Trader behavior varies significantly with market sentiment  
- Sentiment influences **risk-taking patterns** (leverage, frequency) more than direct profitability  
- High-leverage and frequent traders exhibit more volatile outcomes  

---

## 💡 Strategy Recommendations

### 🔹 Risk Management in Fear Markets
- Reduce leverage and control position sizes  
- Focus on selective, high-confidence trades  

### 🔹 Avoid Overtrading in Greed Markets
- Limit excessive trading activity  
- Manage overconfidence and apply stricter risk controls  

---

## 🧠 Key Takeaway
Market sentiment does not directly determine profitability but significantly influences trader behavior. Effective trading strategies should adapt to behavioral shifts rather than rely solely on sentiment-driven expectations.

---

## 🚀 Bonus Work
- Trader clustering using KMeans  
- Basic predictive modeling for trader performance trends  

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- SciPy  

---

## ▶️ How to Run

1. Clone the repository  
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
