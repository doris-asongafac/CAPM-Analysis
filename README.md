Stock Market Risk & Return Analysis
Dow Jones Industrial Average & S&P 500 (CAPM-Based Study)

Author
Doris Mbitazi Asongafac
March 2025

Executive Summary
This project analyzes historical stock data from the Dow Jones Industrial Average (30 major U.S. companies) and the S&P 500 index to evaluate:

Market risk (volatility)
Stock sensitivity to market movements (beta)
Expected returns using the Capital Asset Pricing Model (CAPM)
Key Findings
Financial stocks (e.g., Bank of America, JPMorgan) show high market sensitivity (β > 1)
Defensive stocks (e.g., Walmart, Coca-Cola) exhibit lower volatility and stability
Some utilities and healthcare stocks act as risk stabilizers in portfolios
CAPM reveals that higher risk does not always guarantee higher realized return in short periods

Business Problem
Investors face a key challenge:
How can we measure risk and expected return across different stocks to build a balanced portfolio?

This project answers that question by applying financial data analysis techniques to:
Quantify systematic risk (beta)
Compare stock behavior against the overall market
Estimate expected returns using CAPM

Dataset Overview
Dow Jones Industrial Data
30 large-cap U.S. companies
Weekly OHLC (Open, High, Low, Close) prices
Trading volume and percentage changes

S&P 500 Index Data
Market benchmark used as proxy for overall economic performance
Treasury Data
Used to estimate the risk-free rate (Rf) for CAPM calculations
Data Preparation & Cleaning
Key Steps:
Converted price columns from strings → numeric values
Removed currency symbols ($) and commas
Standardized date formats using lubridate
Handled missing values using na.omit()
Split dataset by stock ticker for individual analysis
Verified structure and consistency of financial time series

Exploratory Data Analysis (EDA)
Market Behavior Insights
Stock returns fluctuate around zero, consistent with efficient market theory
Significant variation exists across sectors
High volatility observed in:
Financials (BAC, JPM)
Technology (CSCO, HPQ)
More stable behavior observed in:
Consumer staples (KO, PG, WMT)

Visual 1: Stock Return Distribution
Boxplot of Weekly Returns Across Stocks
Insight:
Wide dispersion indicates high risk variability across sectors
Several outliers highlight market shock sensitivity

Return Analysis
Weekly returns were computed using:
S&P 500 (market benchmark)
Individual Dow Jones stocks

This allowed comparison of:
Volatility
Directional movement
Correlation with the market

Beta Estimation (Systematic Risk)
Concept
Beta measures how sensitive a stock is to market movements:

β > 1 → More volatile than market
β < 1 → Less volatile than market
β < 0 → Moves opposite to market

Visual 2: Beta Comparison Across Stocks
Conceptual visualization 
Highest beta: BAC (~1.25)
Moderate beta: MCD, JPM, DIS (~0.5–0.8)
Low beta: XOM, INTC, WMT (~0.05–0.2)

Key Insight
Financial stocks amplify market movements, while consumer staples act as defensive assets.

CAPM Analysis (Expected Return Model)
Formula Used:
Expected Return = Rf + β (Market Return − Risk-Free Rate)

Visual 3: CAPM Expected Returns
Key Patterns:
High beta stocks do NOT always deliver highest expected return in short timeframes
Defensive stocks show more stable and predictable returns
Negative beta stocks indicate inverse market sensitivity
Interpretation:
Investors are not just rewarded for return, but for risk exposure
CAPM helps quantify “fair compensation” for risk-taking

Key Insights (Business Value)
Market Behavior
S&P 500 is a reliable benchmark for systemic movement
Individual stocks vary significantly in risk exposure
 Risk Structure
Financial sector = highest risk
Consumer staples = lowest risk
Tech = mixed volatility behavior

Portfolio Strategy
Diversification reduces volatility
Mixing high-beta and low-beta stocks stabilizes returns
 Example Beta Insights Table
Stock	Beta	Interpretation
BAC	1.25	High risk, high sensitivity
AXP	0.80	Moderate-high risk
MCD	0.54	Stable growth stock
KO	0.17	Defensive stock
XOM	0.05	Very low market sensitivity

Conclusion
This analysis demonstrates how financial data can be used to:
Quantify market risk using beta
Compare stock behavior across sectors
Apply CAPM for expected return estimation
Support data-driven investment decisions

 Final Takeaway:
Risk and return are strongly linked, but sector behavior and market conditions significantly influence actual performance outcomes.

 Future Enhancements
Multi-factor models (Fama-French 3-Factor Model)
Predictive modeling for stock returns
Portfolio optimization (Markowitz Efficient Frontier)
Interactive dashboard (Power BI / Shiny App)
Real-time financial data integration

Contact
Doris Mbitazi Asongafac
Data Analyst | Financial Data Enthusiast

LinkedIn: https://www.linkedin.com/in/doris-asongafac
Email: asongafacdoris@gmail.com
