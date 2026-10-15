##international-airpassengers-project

Submitted by: Baylsan Hassan Almehdawi — academy: @SDAIAAcademy

⸻

Project Overview

Capstone project for the SDAIA Time Series course, using the Box & Jenkins AirPassengers dataset (1949–1960).

Project Objectives

* Explore monthly airline passenger data.
* Analyze trend and seasonality using STL decomposition.
* Evaluate a Seasonal Naive baseline.
* Compare forecasting models using cross-validation.
* Assess forecast accuracy and prediction interval coverage.

Methods and Tools

* Python, Pandas, and NumPy
* STL Decomposition and ACF
* AutoGluon TimeSeries
* StatsForecast
* MASE, RMSSE, CRPS, and 80% prediction interval coverage

Results

AutoARIMA outperformed the Seasonal Naive baseline in cross-validation, achieving lower MASE, RMSSE, and CRPS. However, the 80% prediction interval coverage remained below the target, indicating that interval calibration needs improvement.

Dataset

Monthly international airline passenger totals from 1949 to 1960.

Repository Files

* project.ipynb — analysis, forecasting, and evaluation.
* report.md — project findings and recommendations.
* brief.md — project instructions.
* rubric.md — evaluation criteria.

⸻
