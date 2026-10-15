international-airpassengers-project

Submitted by: Baylsan Hassan Almehdawi — academy: @SDAIAAcademy

Capstone project for the SDAIA Time Series course, using the Box & Jenkins AirPassengers dataset (1949–1960).

Project Overview

This project explores monthly airline passenger data, identifies trend and seasonality, evaluates a Seasonal Naive baseline, and compares forecasting models using time-series cross-validation.

Methods and Tools

* Python
* Pandas and NumPy
* STL decomposition
* Autocorrelation (ACF)
* AutoGluon TimeSeries
* StatsForecast
* Forecast evaluation: MASE, RMSSE, CRPS, and 80% prediction interval coverage

Results

AutoARIMA performed better than the Seasonal Naive baseline on the cross-validation results, with lower MASE, RMSSE, and CRPS. Prediction interval coverage remained below the target 80%, indicating that interval calibration may need improvement.

Dataset

Monthly international airline passenger totals from 1949 to 1960.

Files

* project.ipynb — analysis, forecasting, and evaluation
* report.md — project findings and recommendations
* brief.md — project instructions
* rubric.md — evaluation criteria

## Files

- `project.ipynb` — the starter notebook; the graded deliverable
- `brief.md` — the project brief
- `rubric.md` — how it is graded (100 + extra credit)
- `coursekit/` — shared plotting + scoring helpers (the course's harness)
