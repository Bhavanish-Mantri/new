# Trader Behavior vs Market Sentiment Analysis

## Objective
This project explores the relationship between trader performance and Bitcoin market sentiment using the Fear & Greed Index and historical trader data from Hyperliquid.

The goal is to understand how profitability, risk-taking behavior, and risk-adjusted performance vary across different market sentiment regimes.

---

## Datasets
- **Historical Trader Data (Hyperliquid)**  
  https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view

- **Bitcoin Fear & Greed Index**  
  https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view

> Datasets are not included in this repository due to size constraints.

---

## Methodology
1. Parsed and cleaned historical trade timestamps.
2. Standardized trade and sentiment data.
3. Aligned trades with the most recent available sentiment using a time-aware (`merge_asof`) join.
4. Engineered performance and risk metrics.
5. Analyzed profitability, win rate, and risk-adjusted efficiency across sentiment regimes.

---

## Key Findings
- Extreme Greed periods show the highest absolute returns but also the largest losses.
- Risk-adjusted efficiency is highest during Fear and Neutral regimes.
- Greed regimes exhibit signs of overconfidence and poor risk efficiency.
- Extreme Fear reflects capital preservation rather than opportunity-seeking behavior.

---

## Trading Implications
- Market sentiment should be treated as a **risk management signal**, not a directional predictor.
- Position sizing should be reduced during Greed and Extreme Greed regimes.
- More stable opportunities exist during Neutral and Fear periods.

---

## How to Run
1. Download both datasets from the links above.
2. Place them in a local directory or Colab `/content/` folder.
3. Run `analysis.ipynb` top to bottom.

---

## Tools Used
- Python
- Pandas
- Google Colab
