# UC2D - Integrated Crop Care System

## Project Overview

UC2D is a comprehensive automated crop monitoring and management ecosystem combining IoT hardware, AI-powered microservices, and intelligent analytics. The system employs sensor-based data collection with computer vision analysis to detect plant health needs, automate irrigation decisions, and provide precision agriculture recommendations. Built on a scalable microservices architecture with Flask-based AI services, Node.js composite backend, and React dashboard interface.

This enterprise-grade agricultural technology demonstrates end-to-end IoT integration, machine learning deployment, payment processing, and real-time agricultural analytics for modern precision farming applications.

## Link 

  [https://projects.uc2d.chiragbansal.in/login](https://projects.uc2d.chiragbansal.in/login)

## System Architecture

```
UC2D Integrated Crop Care System/
├── hardware/
│   ├── sensors/
│   │   ├── soil_moisture.py          # Moisture level monitoring
│   │   ├── temperature_humidity.py   # Environmental sensors
│   │   └── camera_module.py          # Image capture system
│   ├── controllers/
│   │   ├── irrigation_control.py     # Automated watering
│   │   └── data_transmission.py      # Backend communication
│   └── firmware/
│       └── main_controller.ino       # Arduino/ESP32 firmware
├── microservices/
│   ├── plant-detection-service/
│   │   ├── app.py                    # Flask plant identification API
│   │   ├── models/                   # AI models for plant classification
│   │   └── utils/                    # Image processing utilities
│   ├── water-detection-service/
│   │   ├── app.py                    # Flask water need analysis
│   │   ├── algorithms/               # Water stress detection
│   │   └── sensor_integration/       # Hardware data processing
│   ├── fertilizer-detection-service/
│   │   ├── app.py                    # Flask nutrient analysis
│   │   ├── nutrient_models/          # Deficiency detection AI
│   │   └── recommendation_engine/    # Fertilizer suggestions
│   └── pesticide-detection-service/
│       ├── app.py                    # Flask pest/disease detection
│       ├── disease_models/           # Plant disease classification
│       └── pest_recognition/         # Pest identification system
├── composite-service/ (Node.js)
│   ├── controllers/
│   │   ├── authController.js         # User authentication
│   │   ├── deviceController.js       # Hardware management
│   │   └── analyticsController.js    # Data aggregation
│   ├── services/
│   │   ├── microserviceOrchestrator.js # Flask API coordination
│   │   ├── paymentService.js         # Razorpay integration
│   │   └── loggingService.js         # Data persistence
│   └── models/
│       ├── User.js                   # User management schema
│       └── DeviceData.js             # Sensor data schema
└── frontend/ (React)
    ├── src/
    │   ├── components/
    │   │   ├── Dashboard.js          # Main monitoring interface
    │   │   ├── DeviceStatus.js       # Hardware status display
    │   │   ├── Analytics.js          # Usage and health metrics
    │   │   └── SubscriptionManager.js # Plan management
    │   └── services/
    │       ├── apiService.js         # Backend communication
    │       └── chartService.js       # Data visualization
   

 ```

## Hardware Design 

<img width="2732" height="2456" alt="1 1" src="https://github.com/user-attachments/assets/95a69b11-95c0-4a6b-9611-24c2d4c7cfdf" />

## Software Design

<img width="1332" height="1103" alt="image" src="https://github.com/user-attachments/assets/913229f1-b8fc-4ea3-8d64-50da9a8d72ea" />

## Technical Details

**Technology Stack:**
- **Hardware**: Arduino/ESP32, Environmental Sensors, Camera Module, Relay Controllers
- **Microservices**: Flask, TensorFlow/PyTorch, OpenCV, NumPy
- **Backend**: Node.js, Express.js, MongoDB, JWT Authentication
- **Frontend**: React 18, Recharts, Tailwind CSS
- **Payment**: Razorpay Gateway Integration
- **Communication**: REST APIs, WebSocket for real-time updates

**Core Features:**
- Automated plant identification and growth stage detection
- Real-time water stress monitoring with automated irrigation
- AI-powered nutrient deficiency analysis and fertilizer recommendations
- Computer vision-based pest and disease detection
- Subscription-based premium analytics and extended device management
- Comprehensive data logging for model improvement and historical analysis

## System Interface

<img width="1898" height="868" alt="image" src="https://github.com/user-attachments/assets/da9bfef7-7fb7-42fc-8841-1399d601cfc9" />

<img width="1331" height="818" alt="image" src="https://github.com/user-attachments/assets/040ff030-015a-402f-9e63-7269aff5a739" />

## How to Use and Setup

### Hardware Installation
```bash
# Hardware Setup
1. Install sensors in field according to placement diagram
2. Connect camera module and environmental sensors
3. Configure WiFi/cellular communication module
4. Deploy irrigation control system
5. Power up and test connectivity
```

### Software Deployment
```bash
# Microservices Setup
git clone https://github.com/organization/uc2d-system.git
cd uc2d-system

# Deploy Flask AI Services
cd microservices/plant-detection-service && python app.py
cd ../water-detection-service && python app.py
cd ../fertilizer-detection-service && python app.py  
cd ../pesticide-detection-service && python app.py

# Deploy Node.js Composite Service
cd ../../composite-service
npm install && npm start

# Deploy React Frontend
cd ../frontend
npm install && npm start
```
Access at `http://localhost:3000`

### System Operation
1. Hardware automatically collects sensor data and captures plant images
2. AI microservices analyze data for plant health assessment
3. Composite service aggregates results and stores historical data
4. Dashboard displays real-time status and actionable recommendations
5. Automated systems execute irrigation and alert users for manual interventions

### Controls & Features
- **Controls**: Manual irrigation trigger, sync controls, report generation, subscription management
- **Features**: AI-powered plant analysis, automated recommendations, real-time monitoring, premium analytics, payment integration
