# Port Authority Bus Terminal Passenger Predictions | 2026–2030

## Project Overview

This project was completed as part of a University of New Haven data analytics project for the Port Authority of New York and New Jersey.

The objective was to analyze historical passenger and bus departure data and forecast passenger demand at the Port Authority Bus Terminal (PABT) from 2026 through 2030. The analysis was designed to support planning for temporary staging facilities by identifying future passenger volumes, major demand drivers, carrier-level trends, peak travel periods, and recovery relative to pre-COVID 2019 levels.

## Business Questions

The project addressed five key questions:

1. How many passengers are expected to use the bus terminal from 2026–2030?
2. What factors are most important in predicting passenger volume?
3. How will passenger demand change by individual carrier?
4. What will be the busiest weeks, months, and years between 2026 and 2030?
5. How does current and projected usage compare with the 2019 pre-COVID baseline?

## Data

The analysis used Port Authority Bus Terminal operational data covering December 2020 through July 2025.

The dataset included:

- 162 operational reporting periods
- 1,699 carrier-level records
- 12 tracked carriers
- Passenger volumes
- Bus departures
- Passengers per bus
- Historical comparisons with the 2019 baseline
- Weekly and bi-weekly reporting periods

The 2019 benchmark used in the project was approximately 125,500 weekly passengers and 3,900 bus departures.

## Analytical Approach

Several analytical methods were used to answer the project questions:

### Exploratory Data Analysis
Historical passenger trends, carrier patterns, correlations, seasonality, and post-COVID recovery were examined before forecasting.

### Time-Series Forecasting
An ARIMA(1,1,1) model was used for terminal-wide passenger forecasting from 2026–2030.

Individual ARIMA(1,1,0) models were used to generate directional forecasts for individual carriers.

### Regression Analysis
An Ordinary Least Squares (OLS) regression model was used to identify factors associated with passenger volume.

The model achieved:

- R² = 0.9224
- Adjusted R² = 0.9219
- N = 1,655 observations

### Recovery Analysis
Historical and forecast passenger volumes were compared with the 2019 pre-COVID benchmark to estimate the terminal's recovery trajectory.

### Data Visualization
Five Power BI dashboard views were developed to communicate forecasts, predictive factors, carrier-level trends, peak demand periods, and recovery relative to 2019.

## Key Findings

- Average weekly passenger volume is forecast to increase from approximately **109,647 in 2026** to **148,057 in 2030**.
- Passenger volume is projected to exceed the 2019 baseline in **2028**.
- The 2030 forecast is approximately **18% above the 2019 benchmark**.
- Bus departure frequency was identified as an important operational predictor of passenger volume.
- The regression model estimated approximately **27 additional passengers per additional bus departure**, holding other modeled factors constant.
- **October** was identified as the highest-demand month, with the 2030 October forecast reaching approximately **162,759 average weekly passengers**.
- **January** was identified as the lowest-volume month.
- NJ Transit represents the dominant share of terminal passenger demand throughout the forecast horizon.

## Power BI Dashboard

The Power BI dashboard was organized around the five project questions:

1. Passenger Forecast: 2026–2030
2. Key Predictive Factors
3. Carrier-Level Passenger Forecast
4. Busiest Travel Periods
5. Recovery vs. 2019 Baseline

The dashboard includes forecast visualizations, confidence intervals, carrier comparisons, monthly and weekly demand patterns, recovery metrics, and interactive filtering.

## My Contribution

**Harpreet Singh — Exploratory Data Analysis & Recovery Analysis**

My responsibilities included:

- Conducting statistical data auditing
- Performing exploratory data analysis
- Examining correlations and historical passenger patterns
- Analyzing post-COVID passenger recovery
- Comparing passenger volumes with the 2019 pre-COVID baseline
- Supporting the analysis of the projected full-recovery timeline
- Contributing analytical findings to the final report and presentation

## Team

This was a five-member group analytics project.

- Nista Sunuwar — Data Integration
- Subhechha Khatri — ARIMA Forecasting
- Nathan Peter — Regression Analysis
- Agrima Bogati — Power BI Dashboard
- Harpreet Singh — EDA & Recovery Analysis

## Tools & Technologies

- Microsoft Excel
- Microsoft Power BI
- ARIMA Time-Series Forecasting
- Ordinary Least Squares (OLS) Regression
- Exploratory Data Analysis
- Statistical & Correlation Analysis
- Data Visualization

## Project Deliverables

This repository contains the key deliverables developed for the project:

- Final Project Report
- Power BI Analytics Dashboard
- Project Resources Document

## Important Modeling Considerations

The forecasts should be interpreted with appropriate uncertainty. Reporting frequency changed from weekly to bi-weekly during the historical period, and carrier-level forecasts are based on fewer observations than the terminal-wide forecast.

The forecasting models also assume that no major structural disruption comparable to COVID-19 occurs during the 2026–2030 forecast horizon. The project's 95% confidence intervals should therefore be considered when using the forecasts for planning decisions.

---

**University of New Haven | BANL 6430-01 | Group 6 | Spring 2026**
