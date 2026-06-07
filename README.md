# CoronaryAI Vest — Real-Time Cardiac Wearable
**Biomedical Engineering | Edge AI & Signal Processing | Embedded Firmware | Mobile UI**

Welcome to the engineering documentation hub for the CoronaryAI Vest. This repository showcases the end-to-end development of an intelligent, wearable medical device—spanning analog front-end (AFE) biomedical hardware design, real-time digital signal processing (DSP), edge machine learning for arrhythmia classification, low-power wireless firmware deployment, and mobile application integration.

🏆 **1st Place Project Award:** Recognized for excellence in biomedical engineering and edge AI implementation. Proud to receive this Certificate of Appreciation for contributing as an IC Winner (1st Place) in the regional round of YESIST12 2025.
Abstract ID: 9996
Project/Topic: Heart AI Innov. (Based on handwritten entry)
Event Dates: 8th - 9th May 2025
Organized by: IEEE-HKN Mu Beta (Egypt-Section)
Venue: Arab Academy for Science, Technology & Maritime Transport, Alexandria, Egypt.
A huge thank you to the organizers! [View Certificate](./1st_place_certificate.jpeg)

## 🎥 System Operation & Prototype
![Full Prototype](./ieee_coronary_vest_prototype.png)

*Fully integrated CoronaryAI Vest worn on-body, demonstrating the ergonomic fit and active dry-electrode sensor placement.*

---

## 📄 Core Project Assets
* 🚀 **[Click Here to View the Full Technical Report](./Real-Time_Wearable_T-Shirt_for_Cardiac_Monitoring_-_Formal_Report.pdf)**
* 📱 **[View Mobile App Dashboard](./coronary_app_dashboard.png)**
* 💻 **[View Edge AI Inference Code Snippet](#embedded-software--wireless-telemetry)**

---

## ⚙️ Core Engineering Achievements

### 1. Biomedical Hardware & Sensor Integration
* **Wearable Architecture:** Designed a lightweight, ergonomic textile vest integrating dry-electrode arrays optimized for continuous multi-lead ECG acquisition with minimal motion artifacts.
* **Analog Front-End (AFE):** Configured low-noise instrumentation amplifiers and hardware shielding to maximize Common Mode Rejection Ratio (CMRR), isolating clean cardiac biopotentials from environmental electromagnetic interference.

### 2. Real-Time Signal Processing & Machine Learning
* **DSP Pipeline:** Engineered digital bandpass and notch filters to eliminate baseline wander and 50/60 Hz power-line hum, paired with a robust Pan-Tompkins style algorithm for real-time R-peak and QRS complex detection.
* **Edge AI Classification:** Developed and trained a lightweight Convolutional Neural Network (CNN) optimized for microcontroller deployment, achieving high-accuracy, low-latency classification of cardiac anomalies (e.g., AFib, PVCs).

### 3. Embedded Software & Wireless Telemetry
* **Firmware Architecture:** Developed ultra-low-power microcontroller firmware managing synchronous ADC sampling, algorithmic filtering, and ML inference blocks within a strict real-time execution window.
* **Control Loop & Telemetry Execution:**
  ![Embedded C++ Code](./firmware_snippet.png)
  *Embedded implementation of the core execution loop processing raw telemetry, running edge inference, and packaging anomaly alerts via Bluetooth Low Energy (BLE).*

### 4. Mobile Application & User Interface
* **Real-Time Visualization:** Developed a cross-platform mobile application to receive BLE packets, rendering live ECG waveforms and instantaneous heart rate (BPM) metrics directly to the user's smartphone.
* **Alert Management:** Integrated a dynamic UI/UX that visualizes AI-flagged cardiac anomalies in real-time, providing an accessible and immediate health monitoring dashboard for the end-user.

---

## 📂 Repository Contents
* `Real-Time Wearable T-Shirt for Cardiac Monitoring - Formal Report.pdf` — Comprehensive engineering blueprint containing schematics, PCB layouts, and clinical validation metrics.
* `prototype_full.png` — High-resolution image of the fully integrated CoronaryAI Vest worn on-body.
* `mobile_app_interface.png` — UI/UX screenshots of the mobile application displaying live cardiac telemetrics and AI classifications.
* `1st_place_certificate.png` — Official documentation of the 1st Place award recognition for this project.
* `firmware_snippet.png` — High-resolution layout of the core embedded C/C++ firmware loop.
