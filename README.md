# Secure Data Orchestration Framework for Continuous ICU Monitoring

## Overview

This repository implements a scalable Big Data orchestration framework
for ICU patient monitoring using distributed-style processing and machine learning.

The evaluation is based on a structured simulation of the
MIMIC-III Clinical Database Demo (v1.4).

## Objectives

- Implement ETL-style structured preprocessing
- Perform threshold-based risk labeling
- Train Logistic Regression for risk prediction
- Evaluate Accuracy, Precision, Recall
- Generate Confusion Matrix and ROC Curve
- Perform K-Means clustering
- Measure execution latency
- Demonstrate computational feasibility for near real-time monitoring

---

## Dataset

The dataset simulates ICU physiological monitoring attributes:

- Heart Rate
- Systolic Blood Pressure
- Diastolic Blood Pressure
- Oxygen Saturation (SpO2)

Risk Label Definition:

Risk = 1 if:
- Heart Rate > 100
OR
- SpO2 < 92

Otherwise Risk = 0

---

## Repository Structure

```
Secure-Data-Orchestration-ICU/
│
├── notebooks/
│   └── ICU_Secure_Data_Orchestration.ipynb
│
├── data/
│   └── processed_monitoring_demo.csv
│
├── requirements.txt
│
└── README.md
```

---

## Installation

1. Clone repository:

```
git clone https://github.com/your-username/Secure-Data-Orchestration-ICU.git
cd Secure-Data-Orchestration-ICU
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Launch notebook:

```
jupyter notebook notebooks/ICU_Secure_Data_Orchestration.ipynb
```
