# Data Sources

## Official source
NHS England — Referral to Treatment (RTT) Waiting Times:

https://www.england.nhs.uk/statistics/statistical-work-areas/rtt-waiting-times/

## Current 2026/27 data
https://www.england.nhs.uk/statistics/statistical-work-areas/rtt-waiting-times/rtt-data-2026-27/

## Previous 2025/26 data
https://www.england.nhs.uk/statistics/statistical-work-areas/rtt-waiting-times/rtt-data-2025-26/

Teams should follow equivalent annual archive pages to obtain enough historical monthly observations.

## Required data
Use the **full monthly CSV extracts** where available.

The project focuses primarily on:

**Incomplete pathways**

The full extracts also contain dimensions such as:
- provider;
- commissioner;
- treatment function;
- RTT part type;
- waiting-time bands;
- totals.

## Historical requirement
A single month is not a forecasting dataset.

Use at least **24–36 monthly periods where available**, and preferably more when definitions remain sufficiently comparable.

## Target construction
Teams must document exactly how the monthly target is produced.

Recommended grain:

`month + selected provider/treatment function + incomplete pathways`

## Data handling
Do not commit large raw extracts.

Store locally:

```
data/raw/
data/processed/
data/metadata/
```

## Metadata
Record:
- source URL;
- publication month;
- reporting period;
- downloaded_at;
- original filename;
- row count;
- selected schema/version notes;
- processing status.

## Important interpretation note
RTT statistics are operational administrative data. Teams must preserve NHS definitions and document known breaks, revisions or limitations relevant to their selected series.
