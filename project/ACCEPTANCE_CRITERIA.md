# Acceptance Criteria

## Problem framing
- Forecast target is explicit.
- Forecast horizon is explicit.
- Provider/treatment-function scope is documented.
- Intended planning decision is clear.

## Data
- Official NHS England RTT data is used.
- Multiple monthly extracts are used.
- Historical period is adequate for the selected modelling approach.
- Aggregation is reproducible.
- Missing/duplicate records are assessed.
- Data limitations are documented.

## Reproducibility
- A reviewer can reproduce the modelling series from documented public data.
- Paid services are not required.
- Local paths are portable/configurable.

## EDA
- Trend assessed.
- Seasonality assessed.
- anomalies/structural changes considered.
- No unsupported causal claims made.

## Baseline
- At least one simple baseline is implemented.
- Baseline performance is reported.

## Modelling
- At least two credible forecasting approaches are compared.
- Model choice is justified by evidence.
- Complexity is not treated as quality by itself.

## Validation
- Random train/test split is not used.
- Time-based validation is implemented.
- Metrics are appropriate and explained.
- Leakage is avoided.

## Final forecast
- Forecast dates are explicit.
- Forecast horizon is 3–6 months.
- Uncertainty is communicated where possible.
- Results are reproducible.

## Capacity interpretation
- Operational interpretation is provided.
- Assumptions are clearly labelled.
- Model outputs are not represented as guaranteed outcomes.

## Engineering quality
- Reusable code exists outside notebooks.
- Functions/modules are readable.
- Dependencies are reproducible.
- Tests cover important preparation/modelling logic.
- Secrets/personal data are absent.

## Documentation
- Setup instructions complete.
- Data acquisition documented.
- Model selection documented.
- Monitoring/retraining approach documented.
- Limitations documented.

## Collaboration
- Contribution evidence is complete.
- Git history demonstrates meaningful team participation.
- PR workflow used where practical.

## Submission
- Final submission complete.
- Reviewer has access.
- QA complete.
- Final tag `v1.0-mettelo-submission` created.
