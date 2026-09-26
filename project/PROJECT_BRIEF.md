# Project Brief

## 1. Business context
RTT waiting-list reporting shows where pressure exists today. Operational planning also needs a view of what may happen next.

A forecasting system can help planning teams anticipate likely future waiting-list volumes, understand uncertainty and identify when demand may exceed current capacity.

## 2. Problem statement
Build a reproducible time-series forecasting solution for monthly incomplete RTT pathways using official NHS England data.

The solution must compare simple and advanced models fairly, use time-aware validation, and convert forecasts into practical capacity-planning insight.

## 3. Primary users
Assume the work supports:
- operational planning teams;
- performance analysts;
- service managers;
- capacity planners;
- analytics teams.

## 4. Target definition
Primary target:

**Total monthly incomplete pathways**

Teams must document:
- exact provider(s);
- treatment function(s);
- aggregation logic;
- monthly date definition;
- inclusion/exclusion rules.

## 5. Data preparation requirements
Teams must:
- acquire multiple monthly full extracts;
- standardise schemas across months;
- parse dates consistently;
- identify duplicate records;
- assess missing values;
- confirm aggregation logic;
- reconcile derived monthly totals against source totals where possible;
- document any schema or publication changes.

## 6. Exploratory analysis
At minimum investigate:
- long-term trend;
- month-to-month variation;
- seasonality;
- autocorrelation;
- unusual spikes/drops;
- missing periods;
- potential structural breaks;
- series length and suitability for modelling.

Avoid making causal claims from time-series patterns alone.

## 7. Baseline model
Every team must implement at least one simple benchmark, such as:
- naive last-value forecast;
- seasonal naive forecast;
- moving-average benchmark.

Advanced models must beat or meaningfully complement the baseline under validation.

## 8. Candidate models
Compare at least two credible approaches beyond or including the baseline.

Examples:
- ETS / Holt-Winters;
- ARIMA / SARIMA;
- Prophet;
- regression with lag/time features;
- gradient boosting with engineered lag features.

Do not use a model simply because it is more complex.

## 9. Validation
Random train/test splits are not acceptable.

Use one of:
- expanding-window validation;
- rolling-origin validation;
- fixed chronological holdout plus rolling evaluation.

Evaluation should reflect the intended forecast horizon.

## 10. Evaluation metrics
Use appropriate metrics such as:
- MAE;
- RMSE;
- MAPE only where mathematically sensible;
- sMAPE or WAPE where useful.

Explain why selected metrics are appropriate.

## 11. Forecast uncertainty
Where supported, provide:
- prediction intervals;
- confidence/uncertainty bands;
- scenario ranges.

Do not present point forecasts as certain outcomes.

## 12. Capacity-planning translation
The final output must go beyond a chart.

Define a simple, explicit planning interpretation such as:
- expected backlog volume;
- forecast change from current level;
- high/medium/low pressure threshold;
- illustrative capacity gap under documented assumptions.

Any capacity conversion must clearly distinguish **measured data** from **assumptions/scenarios**.

## 13. Monitoring
Explain:
- when the model should be refreshed;
- what performance metrics should be monitored;
- what would trigger retraining/reselection;
- how new monthly data would be incorporated.

## 14. Out of scope
The core project does **not** require:
- patient-level data;
- personal data;
- causal inference;
- a production web application;
- paid cloud infrastructure;
- forecasting every NHS provider;
- optimisation of actual clinical staffing levels.

## 15. Success definition
A reviewer should be able to clone the repository, obtain the documented public monthly data, reproduce the selected time series, run the model comparison and regenerate the final forecast without undocumented manual steps.
