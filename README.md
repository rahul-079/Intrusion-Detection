# Intrusion Detection System using YOLO V8

## Overview
The "Trespassing Detection" system is a sophisticated intrusion detection solution designed for real-time monitoring and early identification of security breaches. By integrating high-quality surveillance hardware with advanced software algorithms, the system provides a robust defense mechanism applicable across residential, commercial, and public spaces. Leveraging computer vision and machine learning, it proactively identifies unauthorized access, ensuring swift and effective responses.

## Motive
The primary motive behind this project is to revolutionize security measures through advanced technology. By utilizing deep learning and real-time monitoring, the system enhances overall safety and security across diverse environments. The project ensures cost-effective surveillance with real-time alerting and reporting mechanisms.

## Features
- **Real-Time Monitoring**: Uses surveillance cameras and an IP camera with RTSP support for continuous monitoring.
- **Object Detection**: Implements YOLOv8 to identify potential intruders.
- **Face Recognition**: Uses FaceNet512 for identifying individuals by comparing facial embeddings.
- **Automated Alerts**: Sends email notifications upon detecting an intruder.
- **User Authentication**: Secures access to the system using PyQt.
- **Graphical Data Representation**: Utilizes PyQtChart for visual insights into detections.

## Hardware Requirements
1. **Surveillance Cameras** – For capturing real-time footage.
2. **Processing Unit** – To handle computational requirements.
3. **Network Equipment** – Ensuring seamless connectivity.
4. **Power Supply** – Providing uninterrupted operation.

## Software Stack
1. **Computer Vision Libraries** – OpenCV for frame processing.
2. **Machine Learning Models** – YOLOv8 for object detection and FaceNet512 for face recognition.
3. **Alerting System** – SMTP for sending email notifications.
4. **GUI Development** – PyQt for building the graphical user interface.
5. **Google Colab** – For training the YOLOv8 model with the prepared dataset.

## System Flowchart
Start → Camera Feed → Processing → Object Detection → Trespassing Detection → Alert Generation → Monitoring and Reporting → End

## Advantages
1. **Early Detection** – Identifies threats before escalation.
2. **Real-time Monitoring** – Ensures continuous surveillance.
3. **Documentation and Evidence** – Stores data for forensic analysis.
4. **Cost-Effective Surveillance** – Reduces dependency on manual security.
5. **Increased Security Awareness** – Enhances safety measures in monitored areas.

## Applications
1. **Residential Security** – Prevent unauthorized access to homes.
2. **Industrial Facilities** – Enhance security in factories and warehouses.
3. **Smart Home and IoT Integration** – Integrate with automated security systems.
4. **Private House Monitoring** – Ensure personal safety and property protection.

## Installation

### Prerequisites
- Python 3.6 or later
- IP Camera with RTSP support
- Google Colab (for model training)

### Setup Instructions

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/rahul-079/Intrusion-Detection.git
    cd Intrusion-Detection
    ```

2. **Virtual Environment Setup:**
    ```bash
    python -m venv intrusion
    source intrusion/bin/activate  # On Windows use intrusion\Scripts\activate.bat
    ```

3. **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Configure Environment Variables:**
    ```bash
    INTRUSALERTS_PASSWORD=Password for Email Alerts
    INTRUSALERTS_FROM_EMAIL=From Email Address
    INTRUSALERTS_TO_EMAIL=To Email Address
    IP_CAM_ADDRESS=rtsp_url
    ADMIN_NAME=User Admin Name
    ADMIN_PASSWORD=User Admin Password
    ```

## Usage

### Accessing the Camera Stream
Update the RTSP URL with your camera's configuration details.

```python
rtsp_url = 'rtsp://username:password@ip_address:port/channel_path'
```

### Running the System

1. **Using Normal Camera**
    ```bash
    python app.py
    ```

2. **Using IP Camera**
    ```bash
    python test.py
    ```

## Training the Model

1. **Dataset Preparation:** Annotate and augment your dataset for training.
2. **Model Training:** Use Google Colab to train the YOLOv8 model.

## Project Structure

- **App.py:** Handles the entire system.
- **Models:** Contains detection and processing modules.
    1. **faceDetection.py:** Detects faces using YOLOv8.
    2. **faceExtraction.py:** Extracts faces from frames.
    3. **faceRecognition.py:** Recognizes individuals using FaceNet512.
    4. **notifications.py:** Manages email alerts.
- **Database:** Stores known individuals for face recognition.
- **Requirements.txt:** List of required dependencies.

## Manual
For detailed setup and usage instructions, refer to the project manual:
- [Intrusion Detection System - User Manual](https://drive.google.com/file/d/1LflM0TR32F9Qckumg76iX-pMx-5EZyvh/view?usp=sharing)

## Team
This project was developed by:
- **[Hanumanthu Lohith](https://github.com/lohith84)**
- **[Mamuduri Jerusha](https://github.com/jerusha08)**
- **[Pamu Rahul](https://github.com/rahul-079)**
- **[Pulimi Rahul](https://github.com/rahul-pulimi-github-link)**

## Contributions
Contributions are welcome! Please fork the repository and submit a pull request.

## Conclusion
The "Trespassing Detection" project enhances security by integrating advanced hardware and software for real-time monitoring and early detection of unauthorized access. Its versatility allows it to be deployed across multiple environments, contributing to heightened security awareness and operational efficiency. This project reflects the evolving landscape of technology-driven security solutions.

