# Mandatory Team Repository Structure

Each team must create a separate repository named:

`MTL-DS-008-<team-name>`

Minimum structure:

```
MTL-DS-008-<team-name>/
│
├── README.md
├── CONTRIBUTIONS.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── raw/
│   │   └── README.md
│   ├── processed/
│   │   └── README.md
│   └── metadata/
│       └── README.md
│
├── docs/
│   ├── 01-problem-framing/
│   │   └── README.md
│   ├── 02-data-understanding/
│   │   └── README.md
│   ├── 03-eda/
│   │   └── README.md
│   ├── 04-modelling/
│   │   └── README.md
│   ├── 05-evaluation/
│   │   └── README.md
│   ├── 06-capacity-planning/
│   │   └── README.md
│   └── 07-technical-handover/
│       └── README.md
│
├── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   ├── evaluation/
│   └── utils/
│
├── notebooks/
├── tests/
├── models/
├── outputs/
│   ├── forecasts/
│   ├── figures/
│   └── tables/
│
└── submission/
    └── FINAL_SUBMISSION.md
```

## Repository rules

### Raw data
Do not commit large monthly NHS CSV files.

Instead provide:
- source links;
- reproducible download instructions or scripts;
- metadata;
- processing code.

### Notebook rule
Notebooks may be used for exploration, but the final workflow must not exist only inside one large notebook.

Reusable preparation, modelling and evaluation logic should be moved into `src/`.

### Model artifacts
Only commit model artifacts when small and useful.

### Collaboration evidence
Use:
- issues;
- feature branches;
- meaningful commits;
- pull requests;
- peer review.

## Final version
After QA and Mettelo review:

`v1.0-mettelo-submission`
