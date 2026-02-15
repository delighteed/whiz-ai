# Whiz - AI-Based Real-Time Attention Monitoring System

Whiz is an AI-driven system designed to detect attention drift and cognitive distraction in real time using only a standard webcam.

The project combines computer vision, behavioral signal processing, and lightweight machine learning to estimate user focus levels and provide intelligent feedback. This repository contains the complete Whiz system, including the core MVP engine, the product website, and the monitoring dashboard.

---

## Repository Structure

This repository contains three main modules:

### 1) mvp/
Core real-time attention detection engine.

- Webcam-based facial landmark tracking
- Eye Aspect Ratio (blink detection)
- Head pose (yaw) distraction detection
- Optional AI-based cognitive load estimation (Random Forest)
- Sound and notification alerts
- Multiple sensitivity modes

See `mvp/README.md` for detailed setup instructions.

---

### 2️) website/
Product website (Next.js / TypeScript).

- Landing page
- Product overview
- UI presentation
- Deployment-ready structure

Live deployment: https://whiz-web.vercel.app

---

### 3️) grafana/
Monitoring and analytics dashboard configuration.

- Attention metrics visualization
- System monitoring panels
- Data tracking for performance insights

---

## System Architecture Overview

Webcam Input  
→ OpenCV Frame Capture  
→ MediaPipe Face Landmark Extraction  
→ Feature Computation (EAR, Head Pose, Behavioral Signals)  
→ Attention Evaluation Logic  
→ Optional ML Model (Random Forest)  
→ Alerts & Feedback  
→ Analytics Dashboard (Grafana)

All processing is performed locally in the MVP prototype.

---

## Tech Stack

### Core Engine
- Python
- OpenCV
- MediaPipe
- NumPy
- scikit-learn
- pygame
- plyer

### Website
- Next.js
- TypeScript
- React
- Tailwind CSS

### Monitoring
- Grafana

---

## Project Purpose

Whiz was developed as a proof-of-concept system to validate the feasibility of real-time, AI-driven attention monitoring using consumer-grade hardware.

The primary objective is to demonstrate that cognitive state estimation can be performed locally, without wearable devices or cloud inference, using lightweight computer vision techniques.

This unified repository represents the early-stage validation of a broader AI-based digital wellbeing and productivity platform.

---

## Future Development

Planned improvements include:

- Deep learning–based gaze estimation
- Enhanced behavioral modeling
- Multi-user detection support
- Cloud-based analytics pipeline
- Performance optimization for long-duration sessions

---

## Disclaimer

This system is an experimental prototype built for research, competition, and early-stage startup validation purposes. It is not intended for medical diagnosis or clinical use.

