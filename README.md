# 🚦 Machine Learning-Driven Adaptive Traffic Control System

## Overview

This project presents an intelligent traffic management system that dynamically optimizes traffic signal timings using Machine Learning-based congestion prediction, Priority Queue Scheduling, and Emergency Vehicle Preemption.

The system replaces conventional fixed-time traffic controllers with an adaptive framework capable of responding to real-time traffic conditions, reducing congestion, improving traffic throughput, and prioritizing emergency vehicles.

A real-time monitoring dashboard built using Flask and Chart.js provides live traffic analytics, congestion monitoring, signal status tracking, and emergency event visualization.

---

## Features

### 🧠 Machine Learning-Based Congestion Prediction

* Random Forest Classifier for congestion classification
* Low, Medium, and High congestion prediction
* Real-time traffic state analysis
* Dataset-driven traffic pattern simulation

### 🚦 Adaptive Signal Optimization

* Dynamic traffic signal timing allocation
* Priority Queue-based lane scheduling
* Starvation prevention mechanism
* Fair traffic distribution across lanes

### 🚑 Emergency Vehicle Preemption

* Automatic ambulance detection
* Instant traffic signal override
* Priority lane clearance
* Automatic recovery after emergency passage

### 📊 Real-Time Analytics Dashboard

* Live signal status monitoring
* Throughput tracking
* Congestion visualization
* Lane priority analysis
* Event logging
* Emergency alerts

### 🎮 Traffic Simulation Environment

* Pygame-based traffic simulation
* Multi-lane intersection model
* Realistic traffic generation
* Vehicle movement visualization

---

## System Architecture

```text
Traffic Generation
        │
        ▼
Feature Engineering
        │
        ▼
Random Forest Model
        │
        ▼
Priority Queue Scheduler
        │
        ▼
Traffic Signal Controller
        │
        ▼
Emergency Preemption Module
        │
        ▼
Flask Dashboard
```

---

## Technologies Used

* Python
* Flask
* Pygame
* Scikit-Learn
* Random Forest Classifier
* Pandas
* NumPy
* Joblib
* HTML
* CSS
* JavaScript
* Chart.js

---
## Dataset and Models

### Dataset

The project uses traffic datasets representing a four-way intersection with features such as:

- Vehicle counts
- Queue lengths
- Traffic density
- Congestion levels
- Vehicle movement patterns
- Lane-wise traffic statistics

The datasets are stored in the `data/` directory and are used for training, prediction, and simulation.

### Machine Learning Models

The repository includes pre-trained machine learning models for:

- Traffic congestion prediction
- Queue length estimation
- Waiting time prediction
- Traffic anomaly detection

Models are stored in the `model/` and `data/models/` directories and are loaded dynamically during simulation execution.

---

## Project Structure

```text
ML-Adaptive-Traffic-Control-System
│
├── dashboard_server.py
├── launcher.py
├── traffic_sim.py
├── requirements.txt
├── README.md
├── .gitignore
│
├── templates
│   └── dashboard.html
│
├── data
│   ├── live_feedback_log.csv
│   ├── predictions_4way_by_lane.csv
│   ├── predictions_4way_full.csv
│   ├── traffic_dataset_4way.csv
│   └── models/
│       ├── ml_congestion_classifier.pkl
│       ├── ml_feature_names.pkl
│       ├── ml_label_encoders.pkl
│       ├── ml_queue_regressor.pkl
│       └── ml_wait_regressor.pkl
│
├── model
│   ├── anomaly_detector_4way.pkl
│   ├── label_encoder_congestion.pkl
│   ├── label_encoder_destination.pkl
│   ├── label_encoder_origin.pkl
│   ├── label_encoder_turn.pkl
│   └── traffic_model_4way.pkl
│
└── images
    ├── car1.png
    ├── car2.jpg
    ├── intersection.jpg
    ├── mod_int.png
    ├── down/
    ├── left/
    ├── right/
    ├── up/
    └── signals/
```
---

## Installation

### Clone the Repository

```bash
git clone https://github.com/AnanyaGaikwad/ML-Adaptive-Traffic-Control-System.git

cd ML-Adaptive-Traffic-Control-System
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Project

Launch the complete system:

```bash
python launcher.py
```

This starts:

* Traffic Simulation (Pygame)
* Flask Backend
* Real-Time Dashboard

Dashboard URL:

```text
http://127.0.0.1:5000
```

---

## Performance Results

| Metric                         | Fixed-Time System | Proposed System |
| ------------------------------ | ----------------- | --------------- |
| Average Wait Time              | 45.2 s            | 27.1 s          |
| Average Queue Length           | 8.5               | 5.2             |
| Throughput                     | 18.3 veh/min      | 24.7 veh/min    |
| Emergency Clearance Time       | 12.8 s            | 0.5 s           |
| Congestion Prediction Accuracy | N/A               | 95%             |

### Improvements Achieved

* 40% reduction in average waiting time
* 39% reduction in queue length
* 35% increase in throughput
* 96% faster emergency vehicle clearance

---

## Research Publication

This project is associated with the research paper:

**Machine Learning-Driven Adaptive Traffic Control System with Priority-Based Signal Optimization**

Published at:

**International Conference on Emerging Smart Computing and Informatics (ESCI 2026)**
Pune, India

---

## Contributors

* Sheela V. Chinchmalatpure
* Shourya S. Desai
* Vardhan M. Dhavale
* Saumya S. Dhorje
* Ananya A. Gaikwad
* Payal S. Dhaygude

---

## My Contribution

Contributed to dataset preparation, feature engineering, Random Forest model development, performance evaluation, and adaptive traffic signal optimization. Participated in congestion prediction analysis, system validation, and comparative performance assessment against fixed-time traffic control baselines.

---

## Future Scope

* Multi-intersection traffic coordination
* Reinforcement Learning-based optimization
* IoT sensor integration
* Weather-aware traffic prediction
* Smart city deployment
* Multi-emergency vehicle prioritization

---

## License

This repository is intended for academic, educational, and research purposes.
