# RakshaAI – Requirements Document

## 1. Project Overview

RakshaAI is an AI-powered women safety and emergency response system designed to provide instant alerts, predictive safety intelligence, and secure evidence capture. The platform enables real-time emergency communication with family, authorities, and community responders while maintaining reliable offline functionality.

The goal is to transform safety from reactive response into proactive protection.

---

## 2. Objectives

- Provide instant SOS activation via motion or voice
- Automatically alert emergency contacts and authorities
- Capture and store audio/video evidence securely
- Predict unsafe zones using AI logic
- Enable live location tracking
- Support offline emergency messaging
- Provide scalable architecture for real-world deployment

---

## 3. Functional Requirements

### 3.1 Emergency Trigger System
- User can activate SOS via shake gesture
- User can activate SOS via voice command (“Help me”)
- Manual SOS button must be available on home screen

### 3.2 Location Tracking
- System captures real-time GPS location
- Location shared with emergency contacts
- Live tracking enabled after SOS activation

### 3.3 Alert System
- Alerts sent to registered family contacts
- Alerts sent to nearest police authority (simulated)
- Community users receive proximity alert (simulation)
- Offline SMS fallback when internet is unavailable

### 3.4 Evidence Capture
- Automatic audio/video recording after SOS
- Evidence securely stored in local storage (simulated cloud)
- Timestamped evidence logs

### 3.5 AI Safety Intelligence
- Risk zone prediction (rule-based AI simulation)
- Incident heatmap logic
- Safe route suggestion logic

### 3.6 Timer Safety Check
- User sets travel timer
- Auto-SOS triggered if timer expires without confirmation

### 3.7 Fake Call Escape Feature
- Simulated incoming call screen
- Quick exit support during unsafe situations

---

## 4. Non-Functional Requirements

### 4.1 Performance
- SOS response time under 2 seconds
- Backend processing in real-time

### 4.2 Reliability
- System must function with low connectivity
- Offline SMS backup support

### 4.3 Security
- Evidence stored securely
- No unauthorized data access
- User privacy maintained

### 4.4 Scalability
- Architecture designed for future AWS deployment
- Modular backend structure

### 4.5 Usability
- Simple one-tap emergency interface
- Accessible UI for stressed situations
- Multi-language extension support

---

## 5. System Architecture Requirements

- Mobile frontend interface
- Flask backend server
- REST API communication
- Simulated database (JSON storage)
- Simulated cloud evidence storage
- Alert processing engine
- AI logic module

---

## 6. Technology Stack

- Python (Flask)
- HTML / CSS / JavaScript
- Local storage simulation
- REST API architecture
- Rule-based AI logic

---

## 7. Constraints

- Hackathon prototype scope
- Simulated cloud services
- Limited development time
- Local environment deployment

---

## 8. Future Enhancements

- Real AWS Lambda integration
- DynamoDB cloud database
- S3 secure evidence storage
- Real SMS gateway integration
- Machine learning risk prediction model
- Government dashboard monitoring
- Wearable device integration

---

## 9. Conclusion

RakshaAI is designed as a scalable safety ecosystem that combines emergency response, AI intelligence, and secure evidence capture. The prototype demonstrates feasibility and real-world applicability while allowing future cloud expansion.

