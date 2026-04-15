# Redeem — Cybernetic Plant with AI-Driven Health Optimisation

## Overview

**Redeem** is a BT3086 major project that integrates cybernetic systems with living plants to monitor, diagnose, and optimise plant health using artificial intelligence. The system bridges biotechnology and computational intelligence, creating a closed-loop feedback mechanism that continuously assesses a plant's physiological state and takes corrective action to improve its well-being.

## Problem Statement

Traditional plant care relies on manual observation and fixed watering/fertilising schedules, which often leads to:

- **Late detection** of diseases, nutrient deficiencies, or environmental stress.
- **Resource waste** from over-watering or excessive fertiliser use.
- **Crop loss** due to delayed or incorrect interventions.

Redeem addresses these challenges by embedding sensors and AI directly into the plant management workflow, enabling real-time, data-driven health optimisation.

## How It Works

### 1. Sensing Layer

Sensors continuously collect data on key plant health indicators:

| Parameter           | Sensor Type                  |
|---------------------|------------------------------|
| Soil moisture       | Capacitive moisture sensor   |
| Light intensity     | LDR / Lux sensor             |
| Temperature         | DHT11 / DHT22               |
| Humidity            | DHT11 / DHT22               |
| Soil pH             | pH probe                    |
| Nutrient levels     | EC (electrical conductivity) |

### 2. Data Processing

Raw sensor readings are transmitted to a microcontroller (e.g. Arduino / Raspberry Pi) and pre-processed:

- Noise filtering and calibration
- Time-series aggregation
- Feature extraction for the AI model

### 3. AI-Driven Health Analysis

A machine-learning model analyses the processed data to:

- **Classify** the current health status (healthy, stressed, diseased, nutrient-deficient).
- **Predict** future health trends based on historical patterns.
- **Recommend** optimal environmental adjustments (watering volume, light duration, nutrient dosage).

### 4. Actuation & Feedback Loop

Based on AI recommendations, actuators execute corrective actions automatically:

- Water pump adjustment
- Grow-light scheduling
- Nutrient dosing

The system continuously monitors the effect of each intervention, creating a closed feedback loop that refines its predictions over time.

## Project Objectives

1. Design and build a sensor-equipped cybernetic interface for a living plant.
2. Develop an AI model capable of classifying plant health states from sensor data.
3. Implement a closed-loop control system that autonomously optimises plant growing conditions.
4. Evaluate the system's effectiveness by comparing AI-managed plants against manually managed controls.

## Technology Stack

| Component       | Technology                          |
|-----------------|-------------------------------------|
| Microcontroller | Arduino / Raspberry Pi              |
| Sensors         | DHT22, soil moisture, pH, EC, LDR   |
| AI / ML         | Python, scikit-learn / TensorFlow   |
| Data Storage    | SQLite / CSV logging                |
| Communication   | Serial / MQTT                       |
| Visualisation   | Matplotlib / Grafana                |

## Expected Outcomes

- A working prototype of a cybernetic plant system with real-time health monitoring.
- An AI model that accurately classifies plant health and predicts stress conditions.
- Demonstrated improvement in plant health metrics compared to a manually managed baseline.
- A reusable framework that can be extended to different plant species and environments.

## Course Context

This project is submitted as part of the **BT3086 — Major Project** curriculum. It demonstrates the application of biotechnology principles combined with computational tools to solve a real-world agricultural and environmental challenge.

## License

This project is for academic purposes. Please refer to the repository's licence file for usage terms.
