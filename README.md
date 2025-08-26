# IoT-PIT: IoT-based Presence and Identity Tracker

An automated attendance tracking system using IoT technology and facial recognition for educational institutions.

## Project Overview

IoT-PIT is a comprehensive solution for automated attendance management that combines ESP32-CAM modules, facial recognition technology, and cloud-based processing to eliminate manual attendance tracking processes.

## Documentation

### System Design
- **[SystemDesign.md](./SystemDesign.md)** - Technical architecture and system flow diagram showing the two-phase operation (Registration and Attendance phases)

### Requirements
- **[ProductRequirementDocument.md](./ProductRequirementDocument.md)** - Comprehensive Product Requirement Document (PRD) detailing all functional, non-functional, and technical requirements

## Key Features

- **Automated Attendance**: Contactless attendance tracking using facial recognition
- **Real-time Processing**: Immediate attendance logging with timestamp
- **Scalable Architecture**: Supports multiple ESP32-CAM devices and thousands of students
- **Secure Data Handling**: Encrypted storage and secure data transmission
- **Dashboard Interface**: Optional real-time monitoring and reporting capabilities

## System Components

1. **ESP32-CAM Modules**: IoT devices for image capture
2. **Python Server**: Flask/FastAPI backend for processing
3. **Face Recognition Engine**: OpenCV + face_recognition library
4. **Database System**: Storage for face encodings and attendance records
5. **Web Dashboard**: User interface for monitoring and administration

## Getting Started

This repository contains the system design and requirements documentation for the IoT-PIT project. Implementation details and source code will be added in future updates.

## Technology Stack

- **Hardware**: ESP32-CAM modules
- **Backend**: Python (Flask/FastAPI)
- **Computer Vision**: OpenCV, face_recognition
- **Database**: SQL/NoSQL database systems
- **Frontend**: Web-based dashboard (optional mobile app)
- **Communication**: Wi-Fi, HTTP/HTTPS protocols

## Project Status

Currently in requirements and design phase. The system architecture has been defined and comprehensive requirements have been documented.