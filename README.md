# Netra.AI – AI-Powered Smart Surveillance System with Anomaly Detection

## Overview

Netra.AI is an intelligent real-time surveillance system designed to detect suspicious activities such as shoplifting and abnormal behavior using Artificial Intelligence, Deep Learning, and Computer Vision techniques.

Traditional CCTV systems only record footage and rely heavily on manual monitoring, which is inefficient, time-consuming, and prone to human error. Netra.AI transforms conventional surveillance into a smart automated security system capable of detecting anomalies in real time and generating instant alerts.

The system integrates object detection, multi-object tracking, pose estimation, temporal behavior analysis, and motion-based anomaly detection into a unified pipeline for intelligent surveillance applications.

---

# Key Features

• Real-time anomaly detection
• AI-powered smart surveillance
• Transformer-based temporal analysis
• Human detection using DETR
• Multi-object tracking using ByteTrack
• Pose estimation using MediaPipe
• ResNet18-based spatial feature extraction
• Motion spike analysis for suspicious activity detection
• Real-time alerts and visualization using Streamlit
• MongoDB integration for anomaly logging and history tracking
• Lightweight and efficient architecture suitable for deployment

---

# Technologies Used

| Technology | Purpose |
| ------------------- | ------------------------------------- |
| Python | Core implementation |
| OpenCV | Video processing and frame extraction |
| PyTorch | Deep learning framework |
| DETR | Human/Object Detection |
| ByteTrack | Multi-object tracking |
| MediaPipe | Pose estimation |
| ResNet18 | Spatial feature extraction |
| Transformer Encoder | Temporal sequence analysis |
| Streamlit | User Interface |
| MongoDB | Database storage |

---

# System Workflow

```text
Video Input
     ↓
Object Detection (DETR)
     ↓
Multi-Object Tracking (ByteTrack)
     ↓
Pose Estimation (MediaPipe)
     ↓
Spatial Feature Extraction (ResNet18)
     ↓
Temporal Analysis (Transformer Encoder)
     ↓
Motion Difference Analysis
     ↓
Anomaly Detection
     ↓
Alert Generation & Database Storage
```

---

# Project Modules

## Object Detection

The system uses DETR (Detection Transformer) to accurately detect humans and objects from surveillance video frames.
<img width="464" height="266" alt="Screenshot 2026-05-16 181041" src="https://github.com/user-attachments/assets/c383c5cf-73b5-41d7-bc2c-b07b10110719" />


## Multi-Object Tracking

ByteTrack assigns unique IDs to detected individuals and tracks their movement consistently across frames.
<img width="525" height="289" alt="Screenshot 2026-05-16 181050" src="https://github.com/user-attachments/assets/ba1dbea8-b8d5-4212-8a5b-a4d6e8f994d6" />


## Pose Estimation

MediaPipe extracts body movement and posture-related information to improve behavioral understanding.
<img width="560" height="287" alt="Screenshot 2026-05-16 181059" src="https://github.com/user-attachments/assets/0ddb0bf0-cbac-47e3-a568-2185f491d676" />


## Feature Extraction

ResNet18 extracts spatial features such as object appearance, edges, textures, and scene information.

## Temporal Behavior Analysis

Transformer Encoder analyzes frame sequences to understand temporal dependencies and detect abnormal patterns.

## Motion Spike Detection

The system computes frame differences to identify sudden abnormal motion patterns that may indicate suspicious activities.


## Alert and Visualization

Streamlit provides an interactive interface displaying processed video, alerts, anomaly status, and tracking information.
<img width="402" height="241" alt="Screenshot 2026-05-16 181109" src="https://github.com/user-attachments/assets/8dc0e672-a269-4704-8a65-6454e74dc4a5" />

## Database Logging

MongoDB stores anomaly history, timestamps, tracking IDs, and incident information for future analysis.
<img width="576" height="280" alt="Screenshot 2026-05-16 181117" src="https://github.com/user-attachments/assets/5abb52d5-c2c5-4d77-b2c0-83df65b03e46" />

---

# Anomaly Detection Strategy

The proposed system uses a hybrid anomaly detection mechanism:

• Transformer-based temporal modeling
• Motion difference analysis
• Threshold-based anomaly classification

This combination improves detection accuracy while reducing false positives and false negatives.

# Installation & Setup

## 1. Clone Repository

```bash
git clone https://github.com/your-github-username/Netra.AI.git
cd Netra.AI
```

## 2. Install Dependencies

```bash
pip install -r requirements.txt
```

## 3. Run Application

```bash
streamlit run app.py
```

# Applications

• Retail Security
• Smart Surveillance Systems
• Public Safety Monitoring
• Campus Security
• Hospital Monitoring
• Industrial Surveillance
