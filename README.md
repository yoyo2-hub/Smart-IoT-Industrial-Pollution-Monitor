# Smart-IoT-Industrial-Pollution-Monitor

**Smart-Indus-Air-Predict**  
*A Proactive IoT Ecosystem for Industrial Air Quality Monitoring & Prediction*

## 📖 Project Overview

This project is an end-to-end Industrial IoT (IIoT) solution designed to move from reactive to proactive safety management.

Unlike traditional systems that alert only after a danger threshold is reached, this system uses **Edge Intelligence** and **Trend Analysis** to predict pollution peaks **15 minutes before they occur**.

By integrating a local **Edge Layer**, the system ensures worker safety through ultra-low latency and guarantees operational continuity even without an internet connection.

## 🛠️ Key Features

- **Real-Time Metrology**: Continuous monitoring of `CO2`, toxic gases, temperature, and humidity.
- **Predictive Analytics**: Edge-based machine learning (`Linear Regression` / `Trend Analysis`) to anticipate pollution peaks.
- **Automated Retroaction**: Local control loop for automated ventilation (`Servo-actuated`) and emergency evacuation signals (`LED` / `Buzzer`).
- **Industrial Dashboard**: Interactive web-based interface for real-time supervision and maintenance diagnostics.
- **Edge Computing Architecture**: Local processing via `Node-RED` to ensure 24/7 reliability and low-latency safety actions.

## 📐 System Architecture

The system follows a three-tier architecture:

- **Perception Layer (IoT Device)**: `ESP32`-based nodes (simulated via `Wokwi`) collect environmental data and execute local physical actions.
- **Connectivity Layer**: Lightweight `MQTT` protocol for seamless, real-time data exchange between the field and the gateway.
- **Edge Intelligence Layer**: A local gateway (`Node-RED`) acting as the *brain*. It handles data filtering, trend prediction, and decision-making logic.

## 💻 Tech Stack

### Hardware (Simulated)

- **Microcontroller**: `ESP32`
- **Sensors**: `MQ-135` (Gas), `DHT22` (Temperature/Humidity), `MPU6050` (Vibrations)
- **Actuators**: `SG90 Servo` (Ventilation), `I2C LCD` (Diagnostics), `LED` (Emergency)

### Software & Protocols

- **Firmware**: `C++` / `Arduino`
- **Communication**: `MQTT` (`HiveMQ` / `Mosquitto`)
- **Edge/Gateway**: `Node-RED`
- **Analytics**: `Python` / `JavaScript`

## 🚦 Operational Scenarios

- **Normal Monitoring**: Continuous data visualization and energy optimization for ventilation systems.
- **Critical Incident**: Immediate detection of gas leaks triggers hardware interrupts and local alarms.
- **Proactive Prevention**: Prediction of future air saturation triggers automated air renewal before hazardous levels are reached.

## 🚀 Installation & Setup

### 1. Node-RED Setup

- Install `Node-RED` on your local machine.
- Import the provided `flows.json`.

### 2. Wokwi Simulation

- Open the `Wokwi` link provided in the source code.
- Connect the `ESP32` to the MQTT broker: `broker.hivemq.com`.


## 👥 Contributors

- **Chayma Dallel**
- **Oumayma Kammoun**
- **Abderrahmen Ayedi** 
