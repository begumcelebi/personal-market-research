# FTSE 100 vs BIST 100 Portfolio Analysis

## Overview
This project analyses the relationship between the FTSE 100 (UK) and BIST 100 (Turkey) indices using historical daily returns and risk-free yields. The analysis focuses on risk-adjusted performance, correlation dynamics, and diversification insights.  

The purpose is to explore how these two equity markets behave individually and in relation to each other, providing the foundation for a simple two-asset portfolio.

---

## Data
- **Equities:** Daily percentage change data for FTSE 100 and BIST 100.  
- **Risk-Free Rates:** 3-month government yields for the UK and Turkey (annualized, decimal form).  
- **Time Frame:** Last 5 years (adjustable).

**Note:** All calculations are performed in local currency. FX risk is not included.

---

## Methodology
1. **Daily Returns Comparison:** Visualizes short-term performance and volatility.  
2. **30-Day Rolling Correlation:** Shows how the relationship between FTSE 100 and BIST 100 changes over time.  
3. **Monthly Risk–Return Scatter:** Each point represents one month's volatility vs return, showing clusters and diversification potential.  
4. **Risk Metrics:**  
   - Annualized return and volatility  
   - Sharpe ratios using yield-based daily excess returns  
   - Average correlation between indices

---

## Insights
- Correlation between FTSE 100 and BIST 100 is generally low (~0.2), suggesting diversification benefits.  
- Sharpe ratios are calculated relative to local risk-free rates. Negative Sharpe ratios indicate periods where equities underperformed short-term sovereign yields.  
- The monthly risk–return scatter highlights months with higher risk and potential return, providing intuitive visualization for portfolio construction.

---

## Usage
1. Place all CSV files (`ftse_100 .csv`, `bist_100 .csv`, `uk_three_month_gov_bond .csv`, `turkey_three_month_gov_bill .csv`) in the same folder as the Python script.  
2. Run `ftse_bist_portfolio_analysis.py` in Python 3 (with `pandas`, `numpy`, `matplotlib` installed).  
3. The script prints a summary of key metrics and generates the following visuals:  
   - Daily returns comparison  
   - 30-day rolling correlation  
   - Monthly risk–return scatter  

---

## Next Steps / Extensions
- Add a **cumulative investment growth chart** to simulate portfolio performance.  
- Construct **a simple two-asset portfolio** using FTSE 100 and BIST 100 to explore diversification benefits.  
- Incorporate FX-adjusted returns to analyze performance in a single currency.  

---

## Author
Begum Celebi – Portfolio-focused student project
