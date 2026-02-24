# primetrade-data-science-assignment.

# Trader Performance vs. Market Sentiment Analysis

## Objective
An analysis of how Bitcoin market sentiment (Fear/Greed) influences trader behavior and performance on the Hyperliquid platform.

# Methodology

Data Integration: Aligned transaction-level trader data with daily Bitcoin sentiment logs by normalizing timestamps to a daily grain.

Feature Engineering: Developed key performance indicators (KPIs) including win rate, average trade size, and long/short ratios to quantify trader behavior.

Segmentation: Grouped the population into behavioral archetypes—specifically "Frequent vs. Infrequent" and "Consistent Winners vs. Inconsistent Traders"—based on activity percentiles and win-rate stability.

Comparative Analysis: Performed aggregate statistical comparisons across "Fear," "Greed," and "Neutral" regimes to isolate sentiment-driven performance shifts.

# Key Insights

Fear as an Alpha Driver: Total PnL during Fear regimes is nearly 8x higher than in Greed regimes ($6.7M vs $841k), indicating that high volatility during fearful periods is where the most value is extracted.

The Greed Performance Decay: Win rates drop to their lowest point (30.4%) during Greed cycles, which correlates with traders' tendency to aggressively short the market unsuccessfully (lowest Long/Short ratio of 0.853).

High-Frequency Proficiency: "Consistent Winners" are distinguished by a trade count 18x higher than inconsistent traders, proving that success on Hyperliquid is a function of disciplined, high-volume execution rather than large, sporadic bets.

# Strategy Recommendations

Dynamic Liquidity Provision: Increase capital allocation and trade frequency for the "Frequent" trader segment during Fear regimes to maximize capture of high-win-rate opportunities.

Risk Guardrails for Sentiment Shifts: Implement automated leverage warnings or reductions (suggested 25%) for "Inconsistent" traders during Greed regimes to protect them from failing short-bias strategies.

## How to Run
1. Open `assignment.ipynb` in Jupyter Notebook or Google Colab.
2. Ensure the sentiment and trader datasets are in the same directory.
3. Run all cells to reproduce the analysis and charts.
