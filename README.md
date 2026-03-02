# Secure Data Orchestration Framework for Patient Monitoring

This repository implements the case study evaluation described in Section 5
of the project report.

## Workflow

1. Extraction of vital signs from CHARTEVENTS
2. Mean aggregation per patient
3. Mean imputation
4. Binary risk classification using Logistic Regression
5. Execution time measurement
6. K-Means clustering (k=3)

The implementation evaluates predictive performance,
computational feasibility, and clustering behavior
on the MIMIC-III Clinical Database Demo dataset.
