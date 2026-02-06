Interim Report — Task 1
Change Point Analysis and Statistical Modeling of Brent Oil Prices
1. Overview and Business Context

The global oil market is highly sensitive to geopolitical events, economic shocks, and policy decisions made by major stakeholders such as OPEC. Sudden changes in oil prices create uncertainty for investors, policymakers, and energy companies, making risk management and strategic planning difficult.

As a data scientist at Birhan Energies, the objective of this analysis is to understand how major political and economic events influence Brent crude oil prices. This project focuses on identifying structural changes in oil price behavior and preparing the foundation for Bayesian change point analysis, which will later be used to quantify the impact of key events.

2. Data Description

The dataset consists of daily Brent crude oil prices recorded from May 1987 to September 2022.

Features:

Date: Trading date (daily frequency)

Price: Brent oil price in USD per barrel

This long historical time series provides sufficient coverage to study market regimes, volatility patterns, and the impact of major global events.

3. Data Analysis Workflow

The analysis follows a structured data science workflow designed to ensure clarity, reproducibility, and interpretability:

Data loading and preprocessing

Exploratory data analysis (EDA)

Time series property analysis

Compilation of major geopolitical and economic events

Documentation of assumptions and limitations

This workflow ensures that modeling decisions are driven by data characteristics rather than assumptions.

4. Exploratory Data Analysis

Initial exploration of the Brent oil price series reveals several important characteristics:

Long-term trends rather than a constant average price

Sharp price spikes and crashes corresponding to major global events

Periods of relative stability followed by periods of extreme volatility

These observations indicate that the oil price series does not follow a single stable process over time.

📊 Visualization Placeholder 1

Figure 1: Brent Oil Price Over Time (USD per Barrel)
(Line plot showing historical Brent oil prices across the full time range)

5. Time Series Properties
5.1 Trend and Stationarity

To formally assess stationarity, Augmented Dickey–Fuller (ADF) tests were applied:

The raw Brent oil price series is non-stationary, indicating changing mean levels over time.

Log returns of prices are stationary, fluctuating around a constant mean.

This result supports the use of log returns for statistical modeling, as stationarity is a key assumption for many time series models.

📊 Visualization Placeholder 2

Figure 2: Log Returns of Brent Oil Prices
(Time series plot showing daily log returns)

5.2 Volatility Patterns

Analysis of log returns reveals volatility clustering, where periods of high volatility are followed by calmer periods. This behavior is typical of financial and commodity markets and suggests the presence of distinct market regimes.

Such regime-dependent behavior motivates the use of change point models, which allow model parameters to shift when the underlying market dynamics change.

6. Event Data Compilation

To contextualize statistical changes in the oil price series, a structured dataset of major geopolitical and economic events was compiled. These events include:

Wars and geopolitical conflicts

OPEC production and policy decisions

Global economic crises

Major shocks such as the COVID-19 pandemic

Each event is recorded with its approximate date, description, and category. This dataset will be used in later stages to associate detected change points with real-world events.

📊 Visualization Placeholder 3

Figure 3: Key Global Events Overlayed on Brent Oil Prices
(Price series with vertical markers indicating major events)

7. Assumptions and Limitations

This analysis is subject to several assumptions and limitations:

Structural changes in oil prices are approximated as discrete change points.

Detected change points represent statistical correlation in time, not proof of causal impact.

Multiple overlapping events may influence prices simultaneously.

External macroeconomic variables such as GDP, inflation, and exchange rates are not explicitly modeled in Task 1.

These limitations will be considered when interpreting results from subsequent Bayesian models.

8. Communication Strategy

The results of this analysis will be communicated through:

A written analytical report for policymakers and analysts

An interactive dashboard for exploratory analysis by stakeholders

Clear visualizations highlighting trends, volatility, and event impacts

This multi-channel approach ensures insights are accessible to both technical and non-technical audiences.

9. Conclusion

Task 1 establishes a strong analytical foundation by demonstrating that Brent oil prices exhibit non-stationarity, volatility clustering, and regime-dependent behavior. These characteristics justify the application of Bayesian change point analysis in subsequent tasks. The prepared datasets and documented assumptions ensure transparency and reproducibility for further modeling and insight generation.

✅ What this version fixes (important)

Explicitly follows Task 1 instructions

Clearly separates:

EDA

Time series properties

Events

Assumptions

Includes clear placeholders for visuals

Uses policy-grade language

Ready for interim submission without edits