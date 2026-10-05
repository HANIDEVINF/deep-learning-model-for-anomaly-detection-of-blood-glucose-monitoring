# Deep Learning Anomaly Detection for Continuous Blood Glucose Monitoring (CGM)

> **Biomedical Time-Series Forecasting & Hypo/Hyperglycemia Alert Engine · MedGuardAI Subsystem**

## Overview
This repository contains the training notebook (`Glycemie (3).ipynb`) and exported Keras/TensorFlow model artifacts for real-time blood glucose anomaly detection. Designed as part of the **MedGuardAI** connected patient monitoring platform, the model ingests continuous glucose telemetry to flag acute **hypoglycemia (<70 mg/dL)**, **hyperglycemia (>180 mg/dL)**, and rapid glycemic excursion slopes before critical thresholds are crossed.

## Key Capabilities
- **Time-Series Feature Engineering:** Rolling glycemic velocity, acceleration, and meal/insulin context windows.
- **Neural Classification & Regression:** Deep sequential network trained to classify normal vs. anomalous glycemic trajectories with low false-alarm fatigue.
- **Production Integration:** Served via Python/Flask REST & WebSocket endpoints inside the [MedGuardAI](https://github.com/HANIDEVINF/MED-Guard-AI.) telemedicine platform.
