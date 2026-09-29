# Mandatory Team Repository Standard

## Repository Ownership

Each team should use one delivery repository for the project.

Recommended naming:

```text
MTL-DS-008-<team-name>
```

Example:

```text
MTL-DS-008-waiting-list-forecasting-team
```

## Mandatory Mettelo Organisation Access

Every project delivery repository must be accessible to the **Mettelo GitHub organisation**.

### Preferred setup

Where available, create the delivery repository **inside the Mettelo GitHub organisation**.

This is the preferred delivery model because Mettelo can manage repository access, project teams and review permissions centrally.

### If your repository is outside Mettelo

GitHub does not normally allow a personal repository to invite an entire organisation directly.

If your repository is under a personal GitHub account or another organisation, follow the Mettelo access route provided for your cohort before submission. This may require:

- transferring the repository into the Mettelo GitHub organisation; or
- granting access to the specific Mettelo reviewer account/team designated for that cohort.

## Required Review Access

Before submission, Mettelo must be able to inspect:

- repository files and folders;
- commit history;
- branches;
- issues;
- pull requests;
- reviews;
- tests;
- documentation;
- contribution evidence;
- final deliverables.

## Submission Rule

A repository is **not a complete Mettelo submission until Mettelo organisation access has been granted and verified**.

The Team Lead is responsible for confirming this access.

Do not remove Mettelo access until review, verification and project sign-off are complete.

## Git Workflow Expectations

Teams should demonstrate normal collaborative delivery practices:

- meaningful commits;
- issues for material work items;
- branches for substantial changes;
- pull requests for material merges;
- peer review where practical;
- visible individual contributions.

Do not upload the whole project in one final commit.

## Reproducibility

The repository must contain enough documentation for a technically competent Mettelo reviewer to understand and reproduce the delivery.

Where relevant include:

- environment/setup instructions;
- dependency requirements;
- execution order;
- configuration guidance;
- data acquisition instructions;
- pipeline/run instructions;
- test instructions;
- known limitations.

## Security

Never commit:

- passwords;
- API keys;
- access tokens;
- private credentials;
- secrets;
- personal information not intended for publication.
