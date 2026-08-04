# Alternative Data Sentiment Analysis: Search Volume Index (SVI) of Nigerian Equities

**Status: In Progress**

## Planned Scope
- Google Trends data collection and analysis
- Sentiment analysis using TF-IDF and other techniques
- Correlation between sentiment and equity performance

## Overview

This project applies **Search Volume Index (SVI)** from Google Trends as an alternative data source to analyze public interest in three major Nigerian equities and their relationship with stock price movements in the Nigerian market:

- Dangote Cement
- Guaranty Trust Bank (GTCO)
- Zenith Bank

The goal is to explore how search behavior reflects public attention, digital engagement, and potential sentiment signals around these companies over a 5-year period (Nigeria-focused).

---

## Key Insights

- **Zenith Bank** consistently dominates search interest both nationally and regionally.
- Search activity for Zenith Bank is heavily driven by **customer service** and **digital banking** related queries (e.g., USSD codes, internet banking, customer care).
- **Dangote Cement** and **Guaranty Trust Bank** attract significantly lower search volume, with interest more localized.
- Rising queries around Zenith Bank highlight increasing attention to digital access issues and banking tools.

These patterns suggest that search data can serve as a useful proxy for public engagement and service-related sentiment, particularly for retail-focused banks.

---

## Data Source

- **Google Trends** via the `pytrends` library
- Geographical focus: Nigeria (`geo="NG"`)
- Timeframe: Last 5 years
- Keywords used:
  - DANGOTE CEMENT
  - GUARANTY TRUST BANK
  - ZENITH BANK

---

## Project Structure

03-alternative-data-sentiment-analysis/
├── data/
│   ├── raw/                 # Raw data pulled from Google Trends
│   └── processed/           # Cleaned and transformed datasets
├── notebooks/
│   └── equities_svi_analysis.ipynb
├── outputs/                 # CSV exports of top & rising queries, charts
└── README.md


---

## Methodology

1. Collected interest-over-time data for the three equities using Google Trends.
2. Filtered out partial data points.
3. Analyzed related queries (Top and Rising) for each keyword.
4. Compared relative search interest across the three companies.
5. Interpreted patterns with focus on digital banking and customer service themes.

---

## Technologies Used

- Python
- pytrends
- pandas
- matplotlib
- seaborn

---

## Future Improvements

- Integrate Nigerian news sentiment (headlines from local sources)
- Combine SVI with price data to test predictive or correlative relationships
- Expand to more Nigerian equities and sectors
- Build a simple dashboard for monitoring search interest over time

---

## Author

**Olamide Emmanuel Ogundare**  
Aspiring Quantitative Analyst | MScFE Candidate (WorldQuant University)

[GitHub](https://github.com/emycodesanalytics) · [LinkedIn](https://linkedin.com/in/emycodesanalytics)

---

**Last Updated:** 01 July 2026