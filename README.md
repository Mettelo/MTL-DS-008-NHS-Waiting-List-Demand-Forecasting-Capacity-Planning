# MTL-DS-008 — NHS Waiting List Demand Forecasting & Capacity Planning

## Project title
**NHS Waiting List Demand Forecasting & Capacity Planning**

## Project type
Data Science · Team project · Production-style portfolio project

## Challenge
NHS England publishes monthly Referral to Treatment (RTT) waiting-times data covering incomplete, admitted and non-admitted pathways across providers and treatment functions.

A planning team needs more than historical reporting. It needs a reproducible forecasting workflow that can estimate how waiting-list pressure may develop over the next few months and translate that forecast into operational planning insight.

Your team will build that forecasting system.

## Official data sources

NHS England RTT waiting-times data:

https://www.england.nhs.uk/statistics/statistical-work-areas/rtt-waiting-times/

Current 2026/27 RTT releases:

https://www.england.nhs.uk/statistics/statistical-work-areas/rtt-waiting-times/rtt-data-2026-27/

Previous 2025/26 releases:

https://www.england.nhs.uk/statistics/statistical-work-areas/rtt-waiting-times/rtt-data-2025-26/

Use the **full monthly CSV extracts** rather than summary tables where available.

## Required modelling scope
The core target is:

**Monthly incomplete RTT pathways**

Teams must choose and document a manageable forecasting grain, for example:

- one provider over time;
- selected providers;
- one treatment function;
- selected treatment functions;
- provider × treatment-function series where sufficient history exists.

Do not attempt to model every provider and specialty at once.

## Historical period
Use enough monthly history for time-series modelling.

Recommended minimum:
- **24–36 monthly observations** where available.

Preferred:
- extend further back where the schema and definitions remain sufficiently comparable.

A single monthly file is not enough for forecasting.

## Cost requirement
**The complete project must be achievable at £0.**

Recommended free stack:
- Python
- pandas
- NumPy
- statsmodels
- scikit-learn
- matplotlib
- XGBoost or equivalent if desired
- Prophet if desired
- Jupyter
- Git
- GitHub

No paid cloud platform or deployment service is required.

## Core objective
Build a reproducible forecasting workflow that:

1. acquires and combines monthly RTT extracts;
2. validates and standardises the historical series;
3. defines a clear target and modelling grain;
4. explores trend, seasonality, structural breaks and anomalies;
5. establishes a baseline forecast;
6. compares at least two credible forecasting approaches;
7. uses time-based validation rather than random train/test splitting;
8. reports suitable forecast-error metrics;
9. produces uncertainty / prediction intervals where supported;
10. generates a 3–6 month planning forecast;
11. translates the forecast into operational capacity insight;
12. documents limitations and monitoring requirements.

## Required analytical flow

```
Monthly NHS RTT extracts
        ↓
Data validation & standardisation
        ↓
Time-series construction
        ↓
Exploratory analysis
        ↓
Baseline forecast
        ↓
Candidate models
        ↓
Rolling / time-based validation
        ↓
Model comparison
        ↓
Final forecast + uncertainty
        ↓
Capacity-planning interpretation
```

## Business questions
The solution should help answer:

- Is the selected waiting list trending upward, downward or remaining stable?
- Is there recurring seasonality?
- How accurate is a simple baseline compared with more advanced models?
- What volume is expected over the next 3–6 months?
- How uncertain is that forecast?
- Under what forecast conditions would planning teams need additional capacity?
- Which assumptions or data limitations could materially affect the forecast?

## Important modelling rule
This is not a competition to use the most complex algorithm.

A simpler model that performs better under time-based validation is preferred to a more sophisticated model with weaker evidence.

## Team submission model
Each team creates **its own GitHub repository**.

Recommended naming:

`MTL-DS-008-<team-name>`

The Mettelo repository is the challenge specification.

Each team must:
1. create its own repository;
2. invite the designated Mettelo reviewer/collaborator;
3. follow `project/REPOSITORY_STRUCTURE.md`;
4. use issues/branches/commits/pull requests as evidence of collaboration;
5. complete `submission/FINAL_SUBMISSION.md`;
6. complete final QA;
7. tag the accepted version `v1.0-mettelo-submission`;
8. submit the repository URL.

## Project documents
- [Project brief](project/PROJECT_BRIEF.md)
- [Data guidance](data/README.md)
- [Mandatory repository structure](project/REPOSITORY_STRUCTURE.md)
- [Deliverables](project/DELIVERABLES.md)
- [Acceptance criteria](project/ACCEPTANCE_CRITERIA.md)
- [Team roles](project/TEAM_ROLES.md)
- [Contribution rules](CONTRIBUTIONS.md)
- [Final submission template](submission/FINAL_SUBMISSION.md)

---
**Mettelo — Built for What’s Next**
