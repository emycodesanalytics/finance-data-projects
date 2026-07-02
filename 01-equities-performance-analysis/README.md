# 01. Equities Performance Analysis

Comparative performance analysis of three major Nigerian stocks — DANGCEM, GTCO, and ZENITHBANK — over a 5-year period (approximately June 2021 to June 2026).

## Objective
To evaluate and compare the risk-return profiles of these equities using various financial metrics, assess their diversification potential through similarity measures, and determine which stock offered the best risk-adjusted performance.

## Dataset
- Source: Investing.com (daily closing prices)
- Time Period: June 2021 – June 2026
- Stocks: DANGCEM (Industrial Goods sector), GTCO and ZENITHBANK (Financial Services sector)

## Key Analyses Performed
- Data loading, cleaning and preprocessing
- Calculation of daily returns and annualized geometric returns
- Risk metrics including standard deviation, moving average volatility, semi-variance, and high-low range
- Risk-adjusted performance using Sharpe Ratio
- Distribution analysis (skewness and normality testing)
- Pairwise similarity measures (Euclidean Distance, Manhattan Distance, and Cosine Similarity)
- Visualizations including normalized price trends, correlation heatmap, return distributions with pairplots and regression lines, and rolling volatility charts

## Key Findings

**Performance Summary**  
DANGCEM demonstrated the strongest risk-adjusted performance with competitive returns and the lowest volatility among the three stocks, resulting in the highest Sharpe Ratio. ZENITHBANK delivered similar returns to DANGCEM but carried higher volatility, while GTCO recorded the lowest returns with moderate volatility.

**Similarity and Diversification**  
ZENITHBANK and GTCO showed moderate similarity in their return patterns (highest Cosine Similarity of 0.563). DANGCEM exhibited very low similarity with both banking stocks. This suggests strong diversification benefits when combining DANGCEM with banking sector stocks.

**Distribution Characteristics**  
All three stocks displayed negative skewness, indicating a higher likelihood of extreme negative returns. Returns were not normally distributed across the stocks.

## Technologies Used
- Python, pandas, NumPy, Matplotlib, Seaborn
- scikit-learn (for similarity calculations)

## How to Run
1. Navigate to the `notebooks/` folder
2. Open `equities_performance_analysis.ipynb`
3. Run the cells sequentially

All generated charts have been exported as PNG files into the `outputs/` folder.

## Conclusion
Over the 5-year period, DANGCEM offered the best balance of return and risk. The low similarity between DANGCEM and the two banking stocks highlights meaningful diversification opportunities in the Nigerian equities market.

---

**Connect with me:**

- GitHub: [@emycodesanalytics](https://github.com/emycodesanalytics)
- LinkedIn: [Olamide Emmanuel Ogundare](https://www.linkedin.com/in/olamide-emmanuel-ogundare/)
- Twitter/X: [@emycodes](https://x.com/emycodes)

**Last Updated:** 01 July 2026