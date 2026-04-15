# RehabLink – Arm Rehabilitation System

A wearable, real-time biomedical monitoring system designed to support upper limb rehabilitation. Developed as part of the Biomedical Systems and Prototyping course at Universidad de Deusto (2024–2025).

**Authors:** Cristina Borbolla and Lucía García

---

## Overview

RehabLink continuously monitors key physiological signals during rehabilitation exercises and visualizes them through an interactive dashboard, enabling clinicians and patients to track recovery in real time.

## Features

- Real-time monitoring of EMG, joint flexion, heart rate, and ambient temperature
- Interactive Node-RED dashboard with charts, gauges, and color-coded alerts
- Automatic alert system when sensor values exceed safety thresholds
- Per-patient data storage and CSV export for retrospective analysis
- Admin authentication to protect sensitive patient information
- Multi-tab interface: Home, Device Info, Sensors, Alerts, Patient History, Admin

## System Architecture

**Hardware:** Arduino UNO (data acquisition) → Raspberry Pi (processing and visualization)

**Sensors:** Grove EMG sensor, Flex sensor, Finger-clip Heart Rate sensor (PAH8001EI-2G), DHT20 temperature sensor

**Communication:** Serial (Arduino → Raspberry Pi) → MQTT → Node-RED dashboard

## Repository Contents

- `rehablink_flow.json` — Complete Node-RED flow
- `RehabLink_report.pdf` — Full project documentation

## Technologies

Arduino · Raspberry Pi · Python · Node-RED · MQTT · JavaScript
