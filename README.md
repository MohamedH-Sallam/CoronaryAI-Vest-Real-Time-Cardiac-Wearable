# CoronaryAI Vest — Real-Time Cardiac Wearable
**Biomedical Engineering | Edge AI & Signal Processing | Embedded Firmware | Wearable Technology**

Welcome to the engineering documentation hub for the CoronaryAI Vest. This repository showcases the end-to-end development of an intelligent, wearable medical device—spanning analog front-end (AFE) biomedical hardware design, real-time digital signal processing (DSP), edge machine learning for arrhythmia classification, and low-power wireless firmware deployment.

## 🎥 System Operation Demo
![Wearable Vest Operation](./hardware_demo.gif)

*Real-time ECG acquisition, localized QRS detection, and AI-driven anomaly classification during active patient mobility.*

---

## 📄 Core Project Assets
* 🚀 **[Click Here to View the Full Technical Report](./Real-Time_Wearable_T-Shirt_for_Cardiac_Monitoring_Formal_Report.pdf)**
* 💻 **[View Edge AI Inference Code Snippet](#embedded-machine-learning-implementation)**
* 📊 **[View Signal Processing & ML Pipeline Architecture](./ml_pipeline_architecture.png)**

---

## ⚙️ Core Engineering Achievements

### 1. Biomedical Hardware & Sensor Integration
* **Wearable Architecture:** Designed a lightweight, ergonomic textile vest integrating dry-electrode arrays optimized for continuous multi-lead ECG acquisition with minimal motion artifacts.
* **Analog Front-End (AFE):** Configured low-noise instrumentation amplifiers and hardware shielding to maximize Common Mode Rejection Ratio (CMRR), isolating clean cardiac biopotentials from environmental electromagnetic interference.

### 2. Real-Time Signal Processing & Machine Learning
* **DSP Pipeline:** Engineered digital bandpass and notch filters to eliminate baseline wander and 50/60 Hz power-line hum, paired with a robust Pan-Tompkins style algorithm for real-time R-peak and QRS complex detection.
* **Edge AI Classification:** Developed and trained a lightweight Convolutional Neural Network (CNN) optimized for microcontroller deployment, achieving high-accuracy, low-latency classification of cardiac anomalies (e.g., AFib, PVCs).
* **Pipeline Verification:** ![Signal Processing Pipeline](./ml_pipeline_architecture.png)
  *Visualization of the signal conditioning pipeline converting raw biopotentials into clean data arrays for real-time model inference.*

### 3. Embedded Software & Wireless Telemetry
* **Firmware Architecture:** Developed ultra-low-power microcontroller firmware managing synchronous ADC sampling, algorithmic filtering, and ML inference blocks within a strict real-time execution window.
* **Control Loop & Telemetry Execution:**
  ![Embedded C++ Code](./firmware_snippet.png)
  *Embedded implementation of the core execution loop processing raw telemetry, running edge inference, and packaging anomaly alerts via Bluetooth Low Energy (BLE).*

---

## 📂 Repository Contents
* `Real-Time Wearable T-Shirt for Cardiac Monitoring - Formal Report.pdf` — Comprehensive engineering blueprint containing schematics, PCB layouts, and clinical validation metrics.
* `hardware_demo.gif` — Visual proof of the wearable vest acquiring and analyzing data in real time.
* `edge_inference_model.h` — Exported C++ array of the trained neural network optimized for edge microcontroller deployment.
* `ml_pipeline_architecture.png` — Visual schematic of the DSP filter stages and neural network architecture.
* `firmware_snippet.png` — High-resolution layout of the core embedded C/C++ firmware loop.
