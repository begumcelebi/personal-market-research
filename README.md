# FTSE 100 vs BIST 100 Portfolio Analysis

## Overview
This project analyzes the FTSE 100 (UK) and BIST 100 (Turkey) indices using historical daily returns and risk-free yields. The focus is on risk-adjusted performance, correlation dynamics, and diversification insights. The analysis provides a foundation for building a simple two-asset portfolio.

---

## Data
- **Equities:** Daily percentage change data for FTSE 100 and BIST 100.  
- **Risk-Free Rates:** 3-month government yields for the UK and Turkey (annualized, decimal form).  
- **Time Frame:** Last 5 years (adjustable).  

**Note:** All calculations are performed in local currency; FX risk is not included.

---

## Methodology
1. **Daily Returns Comparison:** Visualizes short-term performance and volatility.  
2. **30-Day Rolling Correlation:** Shows how the relationship between FTSE 100 and BIST 100 changes over time.  
3. **Monthly Risk–Return Scatter:** Each point represents one month's volatility vs return, showing clusters and diversification potential.  
4. **Rolling 12-Month Volatility (Annualised):** Measures long-term risk trends using monthly returns.  
5. **Risk Metrics:**  
   - Annualized return and volatility  
   - Sharpe ratios using yield-based daily excess returns  
   - Average correlation between indices

---

## Insights
- Correlation between FTSE 100 and BIST 100 is generally low (~0.2), suggesting diversification benefits.  
- Sharpe ratios, calculated relative to local risk-free rates, indicate periods where equities underperform short-term government yields.  
- Rolling 12-month volatility highlights periods of heightened market risk.  
- The monthly risk-return scatter provides a visual sense of risk-reward distribution across months.

---

## Usage
1. Place all CSV files in the same folder as the Python script:  
   - `ftse_100 .csv`  
   - `bist_100 .csv`  
   - `uk_three_month_gov_bond .csv`  
   - `turkey_three_month_gov_bill .csv`  
2. Run `ftse_bist_portfolio_analysis.py` in Python 3 (requires `pandas`, `numpy`, `matplotlib`).  
3. The script prints key metrics and generates the following visuals:  
   - Daily returns comparison  
   - 30-day rolling correlation  
   - Monthly risk-return scatter  
   - Rolling 12-month volatility (annualised)

---

## Next Steps / Extensions
- Construct a **simple two-asset portfolio** using FTSE 100 and BIST 100 to explore diversification benefits.  
- Add a **cumulative investment growth chart** to visualize portfolio performance.  
- Incorporate **FX-adjusted returns** to analyze performance in a single currency.  

---

## Author
© Begum Celebi, December 2025 – Portfolio-focused student project
