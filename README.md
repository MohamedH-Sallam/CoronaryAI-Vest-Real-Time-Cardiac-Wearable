# CoronaryAI Vest

<p align="center">
  <strong>Real-Time Wearable Cardiac Monitoring</strong><br>
  Biomedical Engineering · Embedded Systems · Signal Processing · Edge AI · Flutter
</p>

<p align="center">
  <a href="./docs/technical/Real-Time_Wearable_T-Shirt_for_Cardiac_Monitoring_Formal_Report.pdf">Technical Report</a> ·
  <a href="./media/app/coronary_app_dashboard.png">Mobile App</a> ·
  <a href="./docs/awards/1st_place_certificate.jpeg">IEEE YESIST12 2025</a>
</p>

---

## Overview

**CoronaryAI Vest** is a wearable cardiac monitoring prototype that combines ECG sensing, embedded processing, AI-based rhythm classification, and a Flutter mobile application in one system.

The project was built to explore how real-time physiological data can be collected, processed, and presented through a portable wearable platform.

> 🏆 **1st Place — IEEE YESIST12 2025**  
> Regional round winner in the **Heart AI Innov.** topic · Abstract ID: **9996**

---

## At a Glance

| Area | Implementation |
| --- | --- |
| **ECG** | Multi-lead dry-electrode acquisition |
| **Signal Processing** | Band-pass, notch filtering & QRS detection |
| **AI** | Lightweight CNN for selected rhythm abnormalities |
| **Embedded System** | Real-time sensing, processing & BLE communication |
| **Mobile App** | Flutter application |
| **Connectivity** | Bluetooth Low Energy (BLE) |
| **Wearable** | Custom textile vest |

---

## System

<p align="center">
  <img src="./media/prototype/ieee_coronary_vest_prototype.png" alt="CoronaryAI Vest prototype" width="520">
</p>

<p align="center">
  <img src="./media/prototype/execution_1.png" alt="CoronaryAI Vest prototype" width="280">
  &nbsp;&nbsp;
  <img src="./media/prototype/execution_2.png" alt="CoronaryAI Vest prototype" width="280">
</p>

The prototype brings the sensing electrodes, electronics, and wearable structure together into a single vest designed for on-body data collection.

---

## How It Works

```text
┌──────────────────┐
│  Wearable Vest   │
│ ECG + Sensors    │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│ Embedded System  │
│ Filtering + AI   │
└────────┬─────────┘
         │ BLE
         ▼
┌──────────────────┐
│   Flutter App    │
│ Live Data + UI   │
└──────────────────┘
```

### 01 · Wearable Hardware

- Custom vest designed around electrode placement
- Multi-lead dry electrodes for ECG acquisition
- Sensors for heart rate and SpO₂
- Experimental NIR-based glucose and cholesterol estimation
- Custom micro-pump mechanism for the project's emergency-response concept

### 02 · Signal Processing

- Digital band-pass and notch filtering
- Baseline-drift and power-line interference reduction
- Pan-Tompkins-based QRS detection
- R-peak and heart-rate calculation

### 03 · Edge AI

A lightweight CNN is used to classify selected cardiac rhythm abnormalities, including **AFib** and **PVCs**. The processing pipeline is designed with embedded hardware constraints in mind.

### 04 · Mobile Application

The Flutter application receives data from the wearable over BLE and provides:

- Live cardiac data and waveform display
- Actual vs. estimated measurements
- Trend and activity tracking
- Medication reminders
- AI-assisted user guidance
- Telemedicine and emergency-location features

---

## Experimental Measurements

The system also explores NIR-based estimation of **glucose and cholesterol** using 660 nm and 940 nm light sources.

These values are **experimental estimates only** and are not intended to replace clinical measurements or diagnostic equipment.

---

## Project Structure

```text
CoronaryAI-Vest-Real-Time-Cardiac-Wearable/
│
├── README.md
│
├── docs/
│   ├── technical/
│   │   └── Real-Time_Wearable_T-Shirt_for_Cardiac_Monitoring_Formal_Report.pdf
│   ├── analysis/
│   │   └── analysis_overview_report_summary.png
│   ├── brochure/
│   │   └── project_brochure.jpeg
│   └── awards/
│       └── 1st_place_certificate.jpeg
│
└── media/
    ├── prototype/
    │   ├── ieee_coronary_vest_prototype.png
    │   ├── execution_1.png
    │   └── execution_2.png
    └── app/
        └── coronary_app_dashboard.png
```

The repository is kept simple and organized by purpose: **documentation** goes under `docs/`, while project images and visual assets are grouped under `media/`.

---

## Project Files

| Resource | Description |
| --- | --- |
| 📄 [Technical Report](./docs/technical/Real-Time_Wearable_T-Shirt_for_Cardiac_Monitoring_Formal_Report.pdf) | Full technical report |
| 📱 [Mobile App Dashboard](./media/app/coronary_app_dashboard.png) | Application interface |
| 📊 [System Analysis](./docs/analysis/analysis_overview_report_summary.png) | Requirements and system analysis |
| 📘 [Project Brochure](./docs/brochure/project_brochure.jpeg) | Project overview and specifications |
| 🏆 [Award Certificate](./docs/awards/1st_place_certificate.jpeg) | IEEE YESIST12 2025 first-place certificate |

---

## Mobile Application

<p align="center">
  <img src="./media/app/coronary_app_dashboard.png" alt="CoronaryAI mobile application dashboard" width="560">
</p>

The companion Flutter application is used to view incoming wearable data and interact with the system through a simple patient-facing interface.

---

## Team

**Ahmed Khaled · Mohamed Hatem · Mostafa Ibrahim**

📍 Hadayek October, Giza, Egypt  
✉️ cucs.cad@gmail.com

---

## Disclaimer

CoronaryAI Vest is an **engineering research and prototyping project**. It is not a certified medical device and should not be used for clinical diagnosis or treatment.

---

<p align="center">
  <sub>Built as an interdisciplinary project combining biomedical engineering, embedded systems, signal processing, AI, and mobile development.</sub>
</p>
