# Required Deliverables

## D1 — Problem framing
Define:
- business problem;
- user;
- target;
- modelling grain;
- forecast horizon;
- intended decision;
- success criteria;
- limitations.

Output:
`docs/01-problem-framing/`

## D2 — Data acquisition & understanding
Document:
- NHS source pages;
- monthly files used;
- historical period;
- relevant fields;
- aggregation logic;
- schema changes;
- data-quality risks.

Output:
`docs/02-data-understanding/`

## D3 — Reproducible preparation pipeline
Build code that:
- loads monthly extracts;
- standardises schemas;
- filters selected scope;
- aggregates the target;
- validates dates/records;
- produces the modelling series.

Output:
`src/data/`

## D4 — Exploratory time-series analysis
Analyse:
- trend;
- seasonality;
- variation;
- autocorrelation;
- anomalies;
- structural breaks;
- missing periods.

Output:
`docs/03-eda/` and `outputs/figures/`

## D5 — Baseline
Implement and evaluate at least one simple forecasting benchmark.

Output:
`src/models/` and `docs/04-modelling/`

## D6 — Candidate models
Train and compare at least two credible forecasting approaches.

Document:
- assumptions;
- features/parameters;
- training process;
- limitations.

## D7 — Time-based evaluation
Use rolling/expanding or equivalent chronological validation.

Report:
- MAE;
- RMSE;
- at least one additional justified measure where useful;
- performance by forecast horizon where feasible.

Output:
`docs/05-evaluation/`

## D8 — Final 3–6 month forecast
Produce:
- point forecasts;
- uncertainty ranges where supported;
- chart/table;
- clear forecast dates.

Output:
`outputs/forecasts/`

## D9 — Capacity-planning interpretation
Translate the forecast into a documented operational planning view without presenting assumptions as observed fact.

Output:
`docs/06-capacity-planning/`

## D10 — Monitoring & handover
Document:
- setup;
- run process;
- adding a new month;
- retraining;
- model-performance monitoring;
- known limitations;
- troubleshooting.

Output:
`docs/07-technical-handover/`

## D11 — Collaboration & submission
Complete:
- `CONTRIBUTIONS.md`;
- GitHub collaboration evidence;
- `submission/FINAL_SUBMISSION.md`;
- final tag.
