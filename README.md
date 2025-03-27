# Machine Learning-Based Predictive Alerts for Proactive System Failure Prevention

## Overview

This project implements a machine learning framework designed to proactively predict system failures using system metrics data. By leveraging Random Forest feature selection and an LSTM recurrent neural network, the system aims to enhance stability, prevent downtime, and support operational continuity.

---

## Motivation

System availability is critical, especially for IT infrastructure in banking and financial services. This project addresses the need for proactive monitoring solutions to minimize unexpected downtime and maintain optimal service delivery.

---

## Project Objectives

- Collect and analyze critical system metrics.
- Perform feature engineering to identify impactful metrics.
- Use Random Forest classification to assess feature importance.
- Train an LSTM recurrent neural network with selected features to predict system behavior.
- Provide proactive alerts based on predictive insights.

---

## Data Collection and Features

System data was collected at 5-second intervals, totaling approximately 1000 records, and stored in CSV format. Features include:

- **CPU Usage**
- **Memory Utilization (MEM)**
- **System Load (LOAD)**
- **TCP Port Status (TCP_PORT_STATUS)**
- **TCP Connection Time Waits (TCP_TIME_WAITS)**
- **Transactions per Second (TPS)**
- **Total TCP Connections (TOTAL_TCP)**
- **Network Latency (NETWORK_LATENCY)**
- **Response Time (RESPONSE_TIME)**
- **Thread Count (THREAD_COUNT)**

**Target variable:**
- **RESTART:** System health states categorized as:
  - `Healthy` (optimal)
  - `Amber` (early abnormality signs)
  - `Red` (critical resource exhaustion)

---

## Methodology

- **Feature Selection**:
  - Applied Random Forest ensemble (`RandomForestClassifier`) with specific hyperparameters.
  - Evaluated using `feature_importances_`.

- **Predictive Modeling**:
  - Utilized an LSTM recurrent neural network for predicting system states from time-series data.
  - Currently gathering and preprocessing additional data to meet deep learning model requirements.

---

## Visualization and Analysis Tools

- Python libraries:
  - **Pandas**
  - **NumPy**
  - **Matplotlib**
  - **Seaborn**
  - **Scikit-learn**
  - **TensorFlow/Keras** (for LSTM implementation)

---

## Results

- Identified key predictive features (CPU, TOTAL_TCP, RESPONSE_TIME).
- Provided visualization of feature importance and model performance.

---

## Next Steps

- Expand dataset size for improved LSTM model training.
- Perform extensive data cleaning and preprocessing.
- Develop and validate LSTM predictive models.

---


# systemHealthCheck
