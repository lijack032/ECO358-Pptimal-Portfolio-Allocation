# ECO358 — Optimal Portfolio Allocation

This repository contains my solution to the **ECO358 Financial Economics I assignment on Optimal Portfolio Allocation** at the **University of Toronto**.

The project applies **mean–variance portfolio theory (Markowitz framework)** to construct optimal portfolios using six Canadian equities and a risk-free asset.

---

# Project Overview

The objective of this assignment is to apply modern portfolio theory to determine:

- The **optimal risky portfolio**
- The **global minimum variance portfolio**
- The effect of **short-selling constraints**
- The **optimal capital allocation** between risky assets and the risk-free asset

Using historical return data, the project computes portfolio statistics and analyzes the **risk–return tradeoff**.

---

# Assets Used

The portfolio consists of six equities traded on the Toronto Stock Exchange.

| Company | Ticker |
|-------|------|
| Royal Bank of Canada | RY.TO |
| Suncor Energy | SU.TO |
| Canadian National Railway | CNR.TO |
| Thomson Reuters | TRI.TO |
| Telus | T.TO |
| Fortis | FTS.TO |

A **3-month Canadian Treasury Bill** is used as the **risk-free asset**.

---

# Data

Daily stock returns were collected for the period

2012-01-01 to 2016-12-31

Daily returns were aggregated into **weekly returns using compounding**.

From these weekly returns we computed:

- expected return
- standard deviation
- covariance matrix

---

# Methodology

## Mean–Variance Optimization

The optimal risky portfolio is obtained by **maximizing the Sharpe ratio**

Sharpe Ratio = (Expected Portfolio Return − Risk Free Rate) / Portfolio Standard Deviation

The optimization was performed numerically using **Excel Solver**.

---

## Efficient Frontier Analysis

Three portfolios are analyzed and plotted on an **E(r) − σ graph**:

- individual equities
- optimal risky portfolio
- global minimum variance portfolio

This allows us to visually examine diversification and the efficient frontier.

---

## Short-Selling Constraints

Two portfolio optimization scenarios were considered:

1. Short selling allowed
2. Short selling not allowed

We compare how the constraint affects:

- portfolio weights
- expected return
- portfolio risk
- Sharpe ratio

---

## Capital Allocation

Investor preferences are represented using a **mean-variance utility function**

U = E(r) − (A / 2) σ²

where the risk aversion coefficient is

A = 15

Using this framework we determine how a **$1,000,000 portfolio** should be allocated between:

- the optimal risky portfolio
- the risk-free Treasury bill

---

# Key Results

## Optimal Risky Portfolio (Short Selling Allowed)

| Metric | Value |
|------|------|
Expected weekly return | 0.38557%
Standard deviation | 1.63567%
Sharpe ratio | 0.22318

---

## Optimal Risky Portfolio (No Short Selling)

| Metric | Value |
|------|------|
Expected weekly return | 0.37240%
Standard deviation | 1.59259%
Sharpe ratio | 0.22094

The short-selling constraint has **only a small effect** on the portfolio.

---

## Global Minimum Variance Portfolio

| Metric | Value |
|------|------|
Expected weekly return | 0.29469%
Standard deviation | 1.41752%
Sharpe ratio | 0.19341

---

# Optimal Capital Allocation

Given:

- risk aversion coefficient A = 15
- total wealth = $1,000,000

The optimal allocation is approximately:

- **92.5% invested in the risky portfolio**
- **7.5% invested in Treasury Bills**

---

# Value of Short Selling

The analysis shows that the investor would be willing to sacrifice approximately

0.00332% of expected return

to gain access to **short-selling capability**.

---

# Tools Used

- Excel Solver
- Mean-Variance Portfolio Theory
- Sharpe Ratio Optimization
- Efficient Frontier Analysis

---

# Course

ECO358 — Financial Economics I  
University of Toronto

---

# Disclaimer

This project was completed for academic purposes as part of a university assignment.
