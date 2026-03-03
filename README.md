# Secure Data Orchestration for Patient Monitoring: Reliability and Privacy in Big Data Streams

This repository contains the case study implementation of a Secure Data Orchestration framework for continuous patient monitoring in Big Data stream environments.

The framework integrates structured data processing, reliability-aware architectural principles, and privacy-conscious analytical design to support resilient and secure ICU monitoring workflows. The implementation evaluates predictive performance and computational feasibility using structured physiological data derived from the MIMIC-III Clinical Database Demo (v1.4).

---

## Dataset and Feature Extraction

The analysis utilizes the `CHARTEVENTS` table to extract continuous monitoring attributes:

- Heart Rate (ITEMID 211, 220045)  
- Systolic Blood Pressure (ITEMID 220179)  
- Diastolic Blood Pressure (ITEMID 220180)  
- Oxygen Saturation (ITEMID 220277)  

Preprocessing involves:

- Filtering relevant physiological measurements  
- Aggregating repeated observations per patient using mean values  
- Handling missing values through mean imputation  

After preprocessing, 98 unique patient records are retained for downstream analysis.

---

## Reliability and Privacy Perspective

The implementation aligns with a reliability-aware and privacy-conscious orchestration model for distributed healthcare systems.

Reliability considerations are reflected in structured data transformation, fault-tolerant architectural layering, and execution latency evaluation. Privacy-aware principles are incorporated through the use of de-identified clinical data and decentralized analytical concepts embedded within the overall framework.

---

## Risk Modeling and Patient Stratification

A binary monitoring risk indicator is defined using physiological thresholds to simulate anomaly detection in ICU environments.

Logistic Regression is applied for binary risk prediction, while K-Means clustering (k = 3) supports physiological stratification of patient states.

---

## Experimental Design

The dataset is partitioned using a 70–30 train-test split. Execution time is measured during model training to assess computational feasibility for near real-time monitoring scenarios.

---

## Analytical Environment

The workflow reflects a distributed Big Data configuration integrating Spark-based architectural concepts with Python-based machine learning libraries.
