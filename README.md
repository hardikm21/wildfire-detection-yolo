Real-Time Wildfire Detection using UAV

A real-time wildfire detection system using YOLOv8, optimized for edge deployment on low-power devices like Raspberry Pi and Jetson Nano. Designed for UAV-based monitoring, enabling rapid detection and response.

Key Highlights
⚡ < 2 seconds alert response time
📉 INT8 quantization for faster inference & smaller model
🌐 REST API integration for real-time alerts
📍 Geo-tagged image snapshots
🔋 Designed for low-power edge devices

Problem Statement

Wildfires spread rapidly and require early detection systems that can operate in remote, resource-constrained environments. Traditional systems are slow or require high computational power.

👉 This project solves it using Edge AI + Deep Learning.

💡 Solution
Built a YOLOv8-based detection model for fire & smoke
Optimized using INT8 quantization for edge devices
Deployed on Raspberry Pi 3 & Jetson Nano
Integrated REST API for instant alerts


Tech Stack
Programming: Python
Model: YOLOv8
Computer Vision: OpenCV
Deployment: Raspberry Pi 3, NVIDIA Jetson Nano
Backend: REST API


⚙️ System Architecture
UAV Camera / Input
        ↓
YOLOv8 Model (Fire & Smoke Detection)
        ↓
INT8 Quantized Model (Fast Inference)
        ↓
Detection Trigger
        ↓
REST API Call
        ↓
Alert + Geo-tagged Image


Workflow
Capture live video via UAV/webcam
Process frames using YOLOv8 model
Detect fire/smoke in real-time
Run optimized INT8 model for faster inference
Send alert via REST API
Attach geo-tagged snapshot
Generate response in < 2 seconds