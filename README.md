# Sustainable Fashion Consumer Behavior & Analytics

[![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

A quantitative empirical research project examining consumer attitudes, brand skepticism, eco-label trust, perceived barriers, purchase intentions, and willingness to pay premium for sustainable fashion products.

---

## 📌 Project Overview

This repository contains the statistical data analysis codebase, Jupyter Notebook, and quantitative findings for the **BUSI 1783 - Business Analytics Project**. The research evaluates data collected from $N = 200$ respondents across 26 survey items to uncover the psychological and demographic determinants driving consumer adoption and price premium acceptance in the sustainable fashion sector.

---

## 📊 Summary of Statistical Analyses

The project executes **six core statistical techniques**:

1. **Frequency Distribution Analysis**: Profile of respondent demographic attributes (Age, Gender, Income, Education, Employment) and item response frequencies.
2. **Descriptive Statistics**: Central tendency (Mean, Median), dispersion ($SD$, $IQR$, Min, Max), and distribution normality (Skewness, Kurtosis) across 21 Likert items and 7 construct composite scores.
3. **Reliability Analysis**: Internal consistency measurement using **Cronbach's Alpha ($\alpha$)**, item-total correlations, and alpha-if-item-deleted statistics for all theoretical constructs.
4. **Correlation Analysis**: **Pearson Bivariate Correlation ($r$)** and **Spearman Rank Correlation** matrices, two-tailed significance testing ($p$-values), and color-coded heatmap visualizations.
5. **Multiple Linear Regression Analysis**: Predictive Ordinary Least Squares (OLS) modeling for *Purchase Intention* and *Willingness to Pay Premium*, complete with Model Fit ($R^2$, Adj $R^2$, $F$-stat), Beta coefficients ($\beta$), Variance Inflation Factor (VIF) multicollinearity checks, and residual diagnostics (Durbin-Watson, Q-Q plots).
6. **Chi-Square ($\chi^2$) Test of Independence**: Bivariate cross-tabulation testing between demographic segments and sustainable behaviors, assessing Pearson $\chi^2$, degrees of freedom ($df$), $p$-values, and Cramér's V effect sizes.

---

## 📁 Repository Structure

```text
├── sustainable_fashion_analysis.ipynb   # Main interactive Jupyter Notebook (Annotated with Markdown)
├── sustainable_fashion_analysis.py      # Standalone Python script for automated execution
├── Untitled form Coded.xlsx             # Primary survey dataset (Raw response data & coded sheet)
├── README.md                            # Repository documentation & GitHub overview
└── output/                              # Exported high-resolution visualization figures
    ├── demographic_distributions.png    # Demographic distribution bar charts
    ├── correlation_heatmap.png          # Pearson correlation matrix heatmap
    ├── construct_boxplots.png           # Construct composite score boxplots
    └── regression_residuals.png         # Regression residual diagnostic plots
```

---

## 📈 Key Empirical Findings

* **Willingness to Pay Premium ($R^2 = 29.25\%, p < 0.001$)**:
  * **Eco-Label Trust** ($\beta = 0.4763, p = 0.006$) is the strongest positive predictor of willingness to pay higher prices for sustainable fashion.
  * **Brand Skepticism** ($\beta = 0.3314, p = 0.036$) significantly increases willingness to pay, indicating that inquisitive consumers prioritize verified sustainability proof.
  * **Purchase Intention** ($\beta = 0.3019, p = 0.012$) directly drives premium price acceptance.
* **Scale Reliability**:
  * Excellent reliability observed for *Willingness to Pay* ($\alpha = 0.9554$), *Eco-Label Trust* ($\alpha = 0.8768$), *Brand Skepticism* ($\alpha = 0.8373$), and *Perceived Barriers* ($\alpha = 0.8291$).
* **Demographic Segmentation**:
  * Significant chi-square associations found between **Education Level** ($\chi^2 = 32.402, p = 0.0089$) and **Employment Status** ($\chi^2 = 33.055, p = 0.0333$) with willingness to pay a price premium.

---

## 🚀 Getting Started

### Prerequisites

Ensure Python 3.9+ is installed along with the following packages:

```bash
pip install pandas numpy scipy statsmodels matplotlib seaborn openpyxl jupyter nbformat
```

### Running the Analysis

#### Option A: Interactive Jupyter Notebook
Launch Jupyter Notebook and open `sustainable_fashion_analysis.ipynb`:

```bash
jupyter notebook sustainable_fashion_analysis.ipynb
```

#### Option B: Command Line Script
Execute the standalone Python script to run the analysis and save figures:

```bash
python sustainable_fashion_analysis.py
```

---

## 🛠️ Data Codebook Summary

| Construct | Items | Description | Scale |
| :--- | :---: | :--- | :---: |
| **Demographics** | 5 | Age, Gender, Income, Education, Employment | Categorical |
| **Environmental Awareness (EA)** | 3 | Impact awareness, sustainability consideration | 1–5 Likert |
| **Brand Skepticism (SK)** | 3 | Questioning claims, greenwashing awareness | 1–5 Likert |
| **Personal Values (PV)** | 3 | Identity alignment, personal values | 1–5 Likert |
| **Eco-Label Trust (ET)** | 3 | Certification reliability, eco-label trust | 1–5 Likert |
| **Perceived Barriers (PB)** | 3 | Price impact, availability, style constraints | 1–5 Likert |
| **Purchase Intention (PI)** | 3 | Regular purchase, brand choice, intention | 1–5 Likert |
| **Willingness to Pay (WTP)** | 3 | Premium payment, higher price acceptance | 1–5 Likert |

---

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.
