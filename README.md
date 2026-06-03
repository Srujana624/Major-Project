# 🚦 Explainable AI for Traffic Violation Detection and Risk Scoring

## 📌 Project Overview

Traffic violations are one of the major causes of road accidents and public safety concerns. This project presents an **Explainable Artificial Intelligence (XAI) based Traffic Violation Detection and Driver Risk Scoring System** that automatically detects traffic violations from video data, calculates driver risk scores, and provides visual explanations for AI decisions using Grad-CAM.

The system combines Computer Vision, Deep Learning, Explainable AI, and Flask APIs to create an intelligent traffic monitoring solution.

---

## 🎯 Objectives

- Detect traffic violations from surveillance videos.
- Classify different types of traffic offenses.
- Calculate risk scores for drivers based on violation history.
- Improve transparency of AI predictions using Explainable AI (Grad-CAM).
- Provide APIs and dashboard support for traffic authorities.

---

## 🏗️ System Architecture

```text
Traffic Video
      │
      ▼
Frame Extraction & Preprocessing
      │
      ▼
CNN-Based Violation Detection
      │
      ▼
Explainable AI (Grad-CAM)
      │
      ▼
Violation Database
      │
      ▼
Risk Scoring Engine
      │
      ▼
Flask API & Dashboard
