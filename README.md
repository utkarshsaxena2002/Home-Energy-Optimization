# Home-Energy-Optimization
Home Energy Optimization is a data-driven platform for monitoring, predicting, and optimizing household energy usage.
The system combines real-time streaming, cloud-based storage, and machine-learning models to deliver room-level insights and whole-home energy forecasts. It supports automated workflows for continuous analysis and long-term optimization.

# Features

Real-Time Energy Streaming (Kafka)
Sensor and device data stream into Kafka topics for low-latency processing and immediate analytics.

Cloud Storage (Backblaze B2)
Efficient, scalable storage for raw sensor data, processed datasets, ML features, and historical logs.

Room-Level ML Prediction Models
Individual machine-learning models forecast energy consumption per room, enabling fine-grained optimization.

Whole-Home Neural Network Model
A consolidated neural network provides holistic energy forecasts and anomaly detection across the entire home.

Batch Processing & Workflow Automation (Airflow)
Feature engineering, model training, batch predictions, and archival tasks are orchestrated through Airflow DAGs.

Optimization Engine
Uses predictions and energy patterns to generate actionable recommendations or automated control signals.

Modular Architecture
Designed for plug-and-play components, allowing integration with IoT devices, APIs, or home automation systems.

# System Architecture Overview

Ingestion: Sensors → Kafka → Stream consumers

Storage: Backblaze B2 for raw + processed data

ML: Room-level models + global neural network

Batch Orchestration: Airflow pipelines for training, evaluation, and scheduled prediction

Output: Dashboards, optimizations, alerts, and device automation

# Tech Stack

Streaming: Apache Kafka

Cloud Storage: Backblaze B2

Orchestration: Apache Airflow

ML: Python, scikit-learn, PyTorch

Data Processing: Pandas, NumPy, Pyspark

