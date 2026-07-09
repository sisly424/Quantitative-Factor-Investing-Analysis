# Quantitative Factor Investing Analysis

A quantitative finance project that investigates the value premium in the U.S. equity market by constructing Book-to-Market (B/M) portfolios and evaluating their performance using multiple asset pricing models.

The project reproduces and extends classic empirical asset pricing research through portfolio construction, factor model regression, robustness testing, and double-sorting analysis using Python.

---

## Project Overview

Value investing has long been one of the most influential investment strategies in finance.

This project investigates whether firms with higher Book-to-Market (B/M) ratios continue to outperform growth firms in the U.S. stock market.

Using CRSP and Compustat data from 1982–2019, the project constructs B/M portfolios and evaluates their performance under different weighting methods and asset pricing models. Additional analyses include sub-period testing, Fama-French Five-Factor regression, and Size × Book-to-Market double sorting to examine whether the value premium remains robust across market conditions. :contentReference[oaicite:1]{index=1}

---

## Business Problem

A long-standing question in finance is whether value stocks consistently outperform growth stocks after adjusting for risk.

This project aims to answer several key questions:

- Does the value premium still exist?
- Has the value premium weakened after 2000?
- Does portfolio weighting affect investment performance?
- Can the Fama-French Five-Factor Model better explain stock returns than CAPM or the Three-Factor Model?
- Does firm size influence the value premium?

---

## Data

The project integrates multiple financial datasets.

### CRSP

Monthly stock market data including:

- Monthly Returns
- Stock Prices
- Shares Outstanding
- Market Capitalization

### Compustat

Firm accounting information including:

- Book Equity
- Assets
- Financial Statements

### Fama-French Factor Library

Risk factors including:

- Market Risk Premium (MKT-RF)
- SMB (Size)
- HML (Value)
- RMW (Profitability)
- CMA (Investment)

The sample covers U.S. common stocks listed on NYSE, NASDAQ, and AMEX from **1982–2019**. Major financial crisis years were excluded to improve robustness. :contentReference[oaicite:2]{index=2}

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Statsmodels
- Matplotlib
- SciPy
- Jupyter Notebook

Financial Models

- CAPM
- Fama-French Three-Factor Model
- Fama-French Five-Factor Model
- Portfolio Sorting
- Double Sorting
- Long-Short Portfolio Construction

---

## Methodology

The project follows the following workflow:

1. Data cleaning and preprocessing
2. Construct Book-to-Market ratios
3. Sort stocks into five B/M portfolios
4. Build Equal-Weighted and Value-Weighted portfolios
5. Calculate monthly portfolio returns
6. Construct Long-Short portfolios
7. Estimate CAPM regressions
8. Estimate Fama-French Three-Factor regressions
9. Estimate Fama-French Five-Factor regressions
10. Perform robustness analysis (Pre-2000 vs. Post-2000)
11. Conduct Size × Book-to-Market double sorting

---

## Models Implemented

### Capital Asset Pricing Model (CAPM)

Estimated abnormal portfolio returns (Alpha) after controlling for market risk.

---

### Fama-French Three-Factor Model

Extended CAPM by incorporating:

- Market Factor
- Size Factor (SMB)
- Value Factor (HML)

---

### Fama-French Five-Factor Model

Further extends the Three-Factor Model by including:

- Profitability (RMW)
- Investment (CMA)

The project compares model performance across all three specifications to evaluate whether the value premium persists after controlling for additional systematic risk factors. :contentReference[oaicite:3]{index=3}

---

## Key Analysis

### Portfolio Construction

- Book-to-Market Quintile Portfolios
- Equal-Weighted Returns
- Value-Weighted Returns
- Long-Short Portfolio

---

### Performance Evaluation

- Mean Returns
- Standard Deviation
- Skewness
- Kurtosis
- Alpha
- Beta
- R²
- t-statistics

---

### Robustness Analysis

To examine whether the value premium changes over time, the sample was divided into:

- 1982–1999
- 2000–2019

The project compares portfolio performance before and after 2000.

---

### Double Sorting

Stocks were first grouped by firm size and then sorted by Book-to-Market ratio, resulting in ten portfolios.

This analysis evaluates whether the value premium differs between small-cap and large-cap firms.

---

## Key Findings

Major findings include:

- Value-weighted portfolios exhibit a stronger value premium than equal-weighted portfolios.
- The value premium weakened after 2000 but remained statistically significant in several specifications.
- The Fama-French Three-Factor Model substantially improves explanatory power over CAPM.
- The Five-Factor Model explains additional variation through profitability and investment factors.
- Double sorting indicates that the value premium is strongest among small-cap value stocks.
- Portfolio construction methodology significantly influences investment performance. :contentReference[oaicite:4]{index=4}

---

## Repository Structure

```
quant-factor-investing-analysis/

│
├── Code.ipynb
├── Data-driven Investments Proposal.pdf
├── Data-driven Investments Report.pdf
├── Data-driven Investments Presentation.pdf
└── README.md
```

---

## Repository Contents

| File | Description |
|------|-------------|
| Code.ipynb | Complete Python implementation for portfolio construction, factor regressions, and empirical analysis |
| Data-driven Investments Proposal.pdf | Initial project proposal and research design |
| Data-driven Investments Report.pdf | Final report including methodology, empirical findings, and investment insights |
| Data-driven Investments Presentation.pdf | Final project presentation summarizing methodology and results |

---

## Skills Demonstrated

- Quantitative Finance
- Factor Investing
- Asset Pricing
- Portfolio Construction
- Financial Data Analysis
- CAPM
- Fama-French Three-Factor Model
- Fama-French Five-Factor Model
- Long-Short Portfolio
- Cross-sectional Analysis
- Time-Series Analysis
- Statistical Modeling
- Python
- Pandas
- NumPy
- Statsmodels
- Financial Research

---

## Team

Master of Business Analytics

UBC Sauder School of Business

- Sisly Lyu
- Kaylee Xiaojing Zhang
- Xiaoxi Xu
- Romee Sun
- Zhuji Zhang
- Wenqiang Yu
