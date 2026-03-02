# Secure Data Orchestration for Patient Monitoring

This repository presents the case study implementation of a Secure Data Orchestration framework for continuous ICU monitoring within a Big Data analytics environment.

The implementation evaluates predictive performance and computational feasibility using structured physiological data derived from the MIMIC-III Clinical Database Demo (v1.4).

---

## Data Processing

The analysis utilizes the `CHARTEVENTS` table to extract the following monitoring attributes:

- Heart Rate (ITEMID 211, 220045)
- Systolic Blood Pressure (ITEMID 220179)
- Diastolic Blood Pressure (ITEMID 220180)
- Oxygen Saturation (ITEMID 220277)

Preprocessing includes:

- Filtering relevant physiological measurements  
- Aggregating repeated observations per patient using mean values  
- Handling missing values through mean imputation  

After preprocessing, 98 unique patient records are retained for analysis.

---

## Risk Modeling

A binary monitoring risk indicator is defined using physiological threshold thresholds to simulate anomaly detection in ICU settings.

Logistic Regression is applied for risk prediction, and clustering analysis using K-Means (k = 3) supports physiological stratification.

---

## Experimental Design

The dataset is partitioned using a 70–30 train-test split. Execution time is measured during model training to assess suitability for near real-time monitoring scenarios.

---

## Environment

The analytical workflow reflects a distributed Big Data configuration, integrating Spark-based architectural concepts with Python-based machine learning libraries.
