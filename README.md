# Commercial Property Exposure Data Scrubbing & CAT-Model Preparation

Python-based exposure data quality and pre-modelling review of a synthetic 100-location commercial property portfolio in England.

## Project Overview

This project simulates the pre-modelling review of a commercial property Statement of Values (SOV) for a UK-based AI/data-operations company.

The objective is to take a raw exposure file and assess whether the data is sufficiently complete, internally consistent and well documented for downstream catastrophe-risk modelling.

The analysis focuses on the data-scrubbing work that takes place before the catastrophe model is run.

## Workflow

**Raw SOV → Data QA → Investigation → Remediation → Validation → Exception Management → Pre-Model Readiness**

## What Was Assessed

- Location and identifier integrity
- Duplicate-record investigation and remediation
- Missing-value assessment
- Building, Contents, EDP/IT and Business Interruption TIV reconciliation
- Reported versus calculated TIV validation
- Occupancy and construction classification review
- Year Built, Stories and Floor Area validation
- Flood-risk exposure and accumulation
- Secondary risk modifiers
- Business Interruption share reconciliation
- Internal consistency checks
- Dynamic QA summary and open-exception reporting

## Key Portfolio Findings

- 100 locations
- £2.865bn total portfolio TIV
- Top 10 locations represent 30.17% of total TIV
- Top 5 cities represent 45.99% of total TIV
- Top 5 counties represent 50.73% of total TIV
- High flood-risk locations represent 39.26% of portfolio TIV
- Data Centres represent 24.71% of portfolio TIV

## Pre-Model Readiness

The portfolio passes the majority of structural, numerical and attribute-level validation checks.

Six open issues remain:

- 2 location-level missing-data exceptions
- 2 reported-TIV reconciliation exceptions
- 2 construction-classification issues requiring further validation

These exceptions would need to be resolved or formally accepted before the exposure could be considered fully model-ready.

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Outputs

- `UK Property Exposure Project.ipynb` — source notebook
- `UK Property Exposure Project.html` — rendered analysis and outputs

## Data Disclaimer

All portfolio records, locations and exposure values used in this project are synthetic and created for portfolio/educational purposes.

No confidential, client or proprietary insurance data is included.

This project demonstrates pre-catastrophe-modelling exposure-data QA and does not reproduce proprietary RMS/AIR model codes, mappings or catastrophe-model outputs.
