# 01. Equities Performance Analysis

Comparative performance analysis of three major Nigerian stocks, namely, **DANGCEM** (Dangote Cement Plc), **GTCO** (Guaranty Trust Holding Company Plc), and **ZENITHBANK** (Zenith Bank Plc), over a 5-year period (approximately June 2021 to June 2026).

## Objective
To evaluate and compare the risk-return profiles of these equities using various financial metrics, assess their diversification potential through similarity measures, and determine which stock offered the best risk-adjusted performance.

## Dataset
- Source: Investing.com (daily closing prices)
- Time Period: June 2021 – June 2026
- Stocks: **DANGCEM** (Dangote Cement Plc - Industrial Goods sector), **GTCO** (Guaranty Trust Holding Company Plc) and **ZENITHBANK** (Zenith Bank Plc - Financial Services sector)

## Key Analyses Performed
- Data loading, cleaning and preprocessing
- Calculation of daily returns and annualized geometric returns
- Risk metrics including standard deviation, moving average volatility, semi-variance, and high-low range
- Risk-adjusted performance using Sharpe Ratio
- Distribution analysis (skewness and normality testing)
- Pairwise similarity measures (Euclidean Distance, Manhattan Distance, and Cosine Similarity)
- Visualizations including normalized price trends, correlation heatmap, return distributions with pairplots and regression lines, and rolling volatility charts

## Summary Statistics

| Stock       | Annualized Return | Daily Return | Std Deviation | Sharpe Ratio | SemiVariance |
|-------------|-------------------|--------------|---------------|--------------|--------------|
| DANGCEM     | 0.0850            | 0.001248     | 0.02106       | 0.0593       | 0.000236     |
| GTCO        | 0.0844            | 0.001135     | 0.02203       | 0.0515       | 0.000414     |
| ZENITHBANK  | 0.0848            | 0.001243     | 0.02277       | 0.0546       | 0.000474     |

[Download Summary Statistics](./outputs/summary_statistics.xlsx)

**Explanation**:
- **Annualized Return** shows the compounded yearly return.
- **Sharpe Ratio** measures return per unit of risk (higher is better).
- **Std Deviation** measures volatility (lower is better for same return).

## Pairwise Similarity Measures

| Pair                  | Euclidean Distance | Manhattan Distance | Cosine Similarity |
|-----------------------|--------------------|--------------------|-------------------|
| DANGCEM - ZENITHBANK  | 1.0532             | 22.2155            | 0.0664            |
| DANGCEM - GTCO        | 1.0527             | 21.7883            | 0.0336            |
| ZENITHBANK - GTCO     | 0.7362             | 17.3105            | 0.5630            |

[Download Similarity Measures](./outputs/similarity_measures.xlsx)

**Explanation**:
- Lower Euclidean and Manhattan distances indicate more similar return behavior.
- Higher Cosine Similarity (closer to 1) means the stocks move more in the same direction.
- ZENITHBANK and GTCO are more similar to each other, while DANGCEM behaves quite differently.

## Key Findings
**Performance Summary**
- **DANGCEM** demonstrated the strongest risk-adjusted performance with competitive returns and the **lowest volatility** among the three stocks, resulting in the **highest Sharpe Ratio**.
- **ZENITHBANK** delivered similar returns to **DANGCEM** but carried higher volatility, while
- **GTCO** recorded the lowest returns among the three with moderate volatility.

**Similarity and Diversification**
- **ZENITHBANK** and **GTCO** (both from the Financial Services sector) exhibited **moderate similarity** in their return patterns (Cosine Similarity ≈ 0.563).
- **DANGCEM** showed **very low similarity** with both banking stocks (Cosine Similarity < 0.07), indicating strong diversification potential when combined with banking stocks.

**Distribution Characteristics**
- All three stocks displayed **negative skewness**, suggesting a higher likelihood of extreme negative returns.
- Returns are **not normally distributed** (Jarque-Bera p-value = 0.0 for all stocks), which is typical in equity markets.

## Technologies Used
- Python, pandas, NumPy, Matplotlib, Seaborn

## Full Analysis
For the complete breakdown, code, detailed analysis, visualizations, and findings, please see the full Jupyter Notebook:
[`equities_performance_analysis.ipynb`](./notebooks/equities_performance_analysis.ipynb)

All generated charts have been exported as PNG files into the [`outputs/`](./outputs/) folder.

## Conclusion
**DANGCEM** demonstrated superior risk-adjusted performance over the 5-year period. The low correlation between DANGCEM and the banking stocks (**GTCO** & **ZENITHBANK**) suggests that a diversified portfolio combining Industrial Goods and Financial Services stocks could offer better risk management in the Nigerian market. This kind of analysis helps investors and portfolio managers make more informed decisions when constructing portfolios, balancing return potential with risk exposure in emerging markets like Nigeria.

---

**Connect with me:**

- GitHub: [@emycodesanalytics](https://github.com/emycodesanalytics)
- LinkedIn: [Olamide Emmanuel Ogundare](https://www.linkedin.com/in/emycodesanalytics)
- Twitter/X: [@emycodes](https://x.com/emycodes)

---

**Last Updated:** 04 July 2026