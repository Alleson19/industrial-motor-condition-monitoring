# Industrial Motor Condition Monitoring System

## 📌 Project Overview

This project presents an industrial motor condition monitoring system developed using PLC concepts, MQTT communication, and Node-RED.

The system continuously monitors important motor operating parameters such as:

- Temperature
- Vibration
- Current
- Motor ON/OFF status
- Alarm status

The collected data is processed and visualized through a Node-RED dashboard. The system also calculates a motor health score and generates alerts when monitored parameters exceed predefined limits.

The project demonstrates how industrial automation data can be integrated with modern IoT-based monitoring and visualization technologies.

---

## 🎯 Objectives

The main objectives of this project are:

1. Monitor important industrial motor parameters.
2. Process motor data using Node-RED.
3. Establish MQTT-based communication.
4. Display real-time motor conditions through a dashboard.
5. Detect abnormal operating conditions.
6. Generate temperature, vibration, and current alerts.
7. Calculate an overall motor health score.
8. Demonstrate the integration of PLC concepts with Industrial IoT technologies.

---

## 🏭 Industrial Context

Industrial motors are critical components in manufacturing plants and process industries. Unexpected motor failures can result in production downtime, maintenance costs, and reduced operational efficiency.

Traditional monitoring methods may depend heavily on periodic inspection and manual observation.

This project demonstrates a condition-monitoring approach in which motor parameters are continuously collected, processed, and displayed on a centralized dashboard.

The architecture can be extended to receive real sensor data from PLC-connected field devices in an industrial environment.

---

## ⚙️ System Architecture

```text
Industrial Motor / Sensors
          │
          ▼
   PLC / Control System
          │
          ▼
   Industrial Network
          │
          ▼
        MQTT
          │
          ▼
       Node-RED
          │
          ▼
   Data Processing
          │
    ┌─────┴─────────┐
    ▼               ▼
Health Score      Alarm Logic
    │               │
    └───────┬───────┘
            ▼
     Node-RED Dashboard
            │
    ┌───────┼────────┐
    ▼       ▼        ▼
 Temperature Vibration Current
    Gauge      Gauge     Gauge
            │
            ▼
       Trend Charts
