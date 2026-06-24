# Maize Price Trends & Volatility Across Malawian Markets (2003–2026)

An exploratory data analysis of maize retail prices in Malawi, using 20+ years of market price data from the World Food Programme.

## The question

Maize is Malawi's staple food crop. This project asks four practical questions:

1. How has the maize price actually changed over time — and does it look different in local currency (MWK) vs. USD?
2. Is there a predictable seasonal pattern tied to the harvest calendar?
3. Do prices differ meaningfully between Malawi's regions?
4. Which markets have the least predictable (most volatile) prices?

## Key findings

| Finding | Detail |
|---|---|
| **Currency distorts the story** | Nominal MWK price rose ~47x since 2003; USD-adjusted price rose only ~3.9x. Most of the "explosion" in price is currency devaluation, not a real shortage. |
| **Strong seasonality** | Prices are ~60% higher in February (pre-harvest) than May/June (post-harvest), every year. |
| **Regional gap is persistent** | Southern Region pays more for maize than Northern Region in almost every year recorded — a structural gap, not a one-off. |
| **Volatility varies sharply by market** | Markets like Manyamula and Euthini are far less price-stable than markets like Chilumba and Lilongwe. |
| **Data gap (2023–2024)** | No data was reported for these two years — flagged explicitly rather than smoothed over. |

## Charts

- `figures/01_price_trend_mwk_vs_usd.png` — Nominal vs. USD-adjusted price trend
- `figures/02_seasonal_pattern.png` — Average price by calendar month
- `figures/03_regional_comparison.png` — Price by region, by year
- `figures/04_market_volatility.png` — Most volatile markets (coefficient of variation)

## Data source

[WFP Food Prices for Malawi](https://data.humdata.org/dataset/wfp-food-prices-for-malawi) — Humanitarian Data Exchange (HDX), sourced from the World Food Programme Price Database. ~79,000 price records across 63 commodities and 129 markets, 1990–2026 (maize subset: ~14,000 records, 2003–2026).

## Tools

Python, pandas, matplotlib, seaborn — run in Jupyter Notebook.

## How to run

```bash
pip install pandas matplotlib seaborn jupyter
jupyter notebook Malawi_Maize_Price_Analysis.ipynb
```

## Author

Montfort Sayamika — [LinkedIn](https://www.linkedin.com/in/montfort-sayamika-223294358/)
