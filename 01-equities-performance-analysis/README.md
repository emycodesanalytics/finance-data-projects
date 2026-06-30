# 01. Nigerian Equities Performance Analysis

Comparative performance analysis of three major Nigerian stocks — **DANGCEM**, **GTCO**, and **ZENITHBANK** — over a **5-year period** (June 2021 – June 2026).

## Objective
To evaluate and compare the risk-return profiles of these equities, assess their diversification potential, and identify which stock offered the best risk-adjusted performance during the period.

## Dataset
- Source: Investing.com (daily closing prices)
- Time Period: Approximately 5 years
- Stocks: DANGCEM (Industrial Goods), GTCO & ZENITHBANK (Financial Services)

## Key Analyses Performed
- Data cleaning and preprocessing
- Return calculations (daily and annualized geometric returns)
- Risk metrics (volatility, semi-variance, high-low range)
- Risk-adjusted performance (Sharpe Ratio)
- Distribution analysis (skewness and normality tests)
- Pairwise similarity measures (Euclidean, Manhattan, and Cosine similarity)
- Visualizations (normalized prices, correlation heatmap, return distributions, rolling volatility)

## Key Findings

**Performance Summary**
- **DANGCEM** stood out as the strongest performer on a risk-adjusted basis, delivering competitive returns with the **lowest volatility** and the **highest Sharpe Ratio**.
- **ZENITHBANK** showed similar returns to DANGCEM but with noticeably higher volatility.
- **GTCO** recorded the lowest returns among the three with moderate volatility.

**Similarity & Diversification**
- ZENITHBANK and GTCO (both from the Financial Services sector) exhibited **moderate similarity** in their return patterns (Cosine Similarity ≈ 0.563).
- DANGCEM showed **very low similarity** with both banking stocks (Cosine Similarity < 0.07), indicating strong diversification potential when combined with banking stocks.

**Distribution Characteristics**
- All three stocks displayed **negative skewness**, suggesting a higher likelihood of extreme negative returns.
- Returns are **not normally distributed** (Jarque-Bera p-value = 0.0 for all stocks), which is typical in equity markets.

## Technologies Used
- Python, pandas, NumPy, Matplotlib, Seaborn

## How to Run
1. Open `notebooks/equities_performance_analysis.ipynb`
2. Run the cells sequentially

## Conclusion
DANGCEM demonstrated superior risk-adjusted performance over the 5-year period. The low correlation between DANGCEM and the banking stocks (GTCO & ZENITHBANK) suggests that a diversified portfolio combining Industrial Goods and Financial Services stocks could offer better risk management in the Nigerian market.

---

**Connect with me:**

- GitHub: [@emycodesanalytics](https://github.com/emycodesanalytics)
- LinkedIn: [Olamide Emmanuel Ogundare](https://www.linkedin.com/in/olamide-emmanuel-ogundare/)  
- Twitter/X: [@emycodes](https://x.com/emycodes)

**Last Updated:** June 30, 2026