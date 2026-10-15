# AirPassengers Time Series Forecasting Report

## Objective

The goal of this project is to analyze monthly international airline passenger data from 1949 to 1960 and evaluate forecasting models.

## Data Exploration

The series shows a clear upward trend and a repeating yearly seasonal pattern. Seasonal fluctuations increase as passenger numbers grow, suggesting that the seasonal variation changes with the level of the series.

## Decomposition and Baseline

STL decomposition with a seasonal period of 12 identified strong trend and seasonal components. The estimated trend strength was 1.00 and seasonal strength was 0.98.

The Seasonal Naive model uses the passenger count from the same month of the previous year as its forecast. Its cross-validation results were MASE 2.335, RMSSE 2.215, and CRPS 0.103. Its 80% prediction interval coverage was 30.6%.

## Model Evaluation

AutoARIMA achieved better cross-validation results than the Seasonal Naive baseline:

- **MASE:** 1.379
- **RMSSE:** 1.387
- **CRPS:** 0.066
- **80% prediction interval coverage:** 43.1%

Lower MASE, RMSSE, and CRPS indicate better forecasting performance. AutoARIMA improved all three metrics compared with the baseline. However, its prediction intervals covered only 43.1% of actual observations, well below the intended 80% coverage.

## Recommendation

Use AutoARIMA as the preferred model among the two evaluated models, while improving prediction interval calibration before relying on its uncertainty estimates for operational decisions.

A useful next step is to evaluate interval calibration over additional rolling-origin validation windows and investigate whether a multiplicative seasonal model better captures the increasing seasonal variation.
