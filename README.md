# CI/CD Workflow Anomaly Detection - Python Portfolio

## Overview

A Python implementation for analysing CI/CD pipeline execution times, identifying unusual behaviour, and comparing statistical and machine-learning approaches.

This demonstration is based on technical methods developed during a Bachelor of Engineering thesis at Oulu University of Applied Sciences.

## Technologies

Python, Pandas, Scikit-learn, Isolation Forest, IQR, Git, GitHub Actions, data analysis and statistical evaluation.

## Implemented Features

- Five-feature CI/CD execution-time analysis
- Interquartile range (IQR) anomaly detection
- Isolation Forest unsupervised anomaly detection
- Input validation and CSV result generation
- Anomaly ranking and comparison of detection methods

## Demonstration Results

The supplied dataset contains 33 synthetic workflow runs.

| Method | Runs flagged |
|---|---:|
| IQR | 3 |
| Isolation Forest | 9 |

Both methods identified runs 9, 24 and 31, which contain deliberately increased synthetic timing values.

The methods can produce different classifications. These demonstration results are not evidence that either method is more accurate.

## Run Locally

Install dependencies:

    python -m pip install -r requirements.txt

Run the IQR analysis:

    python scripts/baseline_method/run_common_feature_iqr.py

Run Isolation Forest:

    python scripts/isolation_forest/run_isolation_forest.py

Results are written to data/processed/.

## Data and Confidentiality

The included dataset is synthetic and is not actual company execution data.
No company credentials, attendance records, internal meeting notes, or private infrastructure information are included.

## Academic Context

Developed from work on AI-assisted CI/CD pipeline optimization for an attendance management system.
The full academic thesis and supervisor-review materials are maintained separately in private repositories.
