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

🛠️ Technologies Used
Programming Languages
Python
JavaScript
HTML
Frameworks & Libraries
Flask
TensorFlow / Keras
OpenCV
NumPy
Matplotlib
Flask-CORS
AI & XAI Techniques
Convolutional Neural Networks (CNN)
Grad-CAM (Gradient-weighted Class Activation Mapping)

📂 Project Structure
Explainable-AI-Traffic-Violation-Detection/
│
├── app.py                      # Flask Backend API
├── index.html                  # Frontend Dashboard
├── preprocessing.py            # Video Frame Extraction
├── violation_model.py          # CNN Model
├── gradcam.py                  # Explainable AI Module
├── risk_scoring.py             # Driver Risk Scoring
├── visualization.py            # Analytics Dashboard
├── frames/                     # Extracted Frames
├── dataset/                    # Training Dataset
└── README.md

⚙️ Features
🚗 Traffic Violation Detection
Detects violations from traffic video footage.
CNN-based classification model.
Supports multiple violation categories.

🔍 Explainable AI (Grad-CAM)
Generates heatmaps highlighting important image regions.
Improves model transparency and trustworthiness.
Helps authorities understand why a violation was detected.

📊 Driver Risk Scoring

Risk scores are assigned based on violation frequency.

Score Range	Risk Level
0 - 10	Low Risk
20 - 29	Medium Risk
30+	High Risk

🌐 REST APIs
Add traffic violations
Retrieve violations
Calculate driver risk score

📈 Data Visualization
Violation distribution charts
Traffic analytics dashboards
Risk analysis reports

🔄 Workflow
Step 1: Video Preprocessing

Traffic videos are processed and converted into frames using OpenCV.

Step 2: Violation Detection

A CNN model analyzes extracted frames and predicts violation categories.

Step 3: Explainability

Grad-CAM highlights image regions responsible for predictions.

Step 4: Risk Assessment

Driver risk scores are computed from accumulated violations.

Step 5: Dashboard & API

Results are served through Flask APIs and displayed on the frontend dashboard.

🚀 Installation
Clone Repository
git clone https://github.com/yourusername/Explainable-AI-Traffic-Violation-Detection.git
cd Explainable-AI-Traffic-Violation-Detection
Create Virtual Environment
python -m venv venv
Activate Environment

Windows:

venv\Scripts\activate

Linux/Mac:

source venv/bin/activate
Install Dependencies
pip install -r requirements.txt

▶️ Running the Project
Start Flask Backend
python app.py

Backend runs at:

http://localhost:5000
Open Frontend

Open:

index.html

in your browser.

📡 API Endpoints
Add Violation

POST

/api/add_violation

Request:

{
  "driver_id": "driver1",
  "violation_type": "signal_jump",
  "location": "Hyderabad"
}

Response:

{
  "message": "Violation recorded"
}
Get Driver Risk Score

GET

/risk_score/<driver_id>

Example:

/risk_score/driver1

Response:

{
  "driver_id": "driver1",
  "risk_score": 20
}
Get All Violations

GET

/violations
