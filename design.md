# RakshaAI – System Design Document

## 1. System Overview

RakshaAI is a safety-focused emergency response platform designed to provide real-time alerts, evidence capture, and predictive safety intelligence. The system is built as a modular architecture that simulates a scalable cloud deployment while running as a lightweight hackathon prototype.

The design prioritizes speed, reliability, and simplicity under emergency conditions.

---

## 2. Design Goals

- Instant emergency activation
- Reliable alert delivery
- Secure evidence storage
- Real-time tracking
- Offline support capability
- Scalable backend architecture
- Simple and stress-friendly UI
- Modular extensibility

---

## 3. High-Level Architecture

RakshaAI follows a client-server architecture.

Mobile Frontend → Backend Alert Engine → Storage + Notification System

Components:

- Mobile Interface
- Backend Processing Server
- AI Logic Module
- Alert Distribution System
- Evidence Storage Layer
- Simulated Database

The architecture is designed to mirror AWS serverless deployment in a simplified form.

---

## 4. Component Design

### 4.1 Mobile Frontend

Responsibilities:

- SOS activation (button, voice, shake)
- GPS location capture
- Evidence recording trigger
- Timer safety feature
- Fake call interface
- User interaction

Design Principles:

- One-tap emergency action
- Minimal UI complexity
- High visibility buttons
- Fast response feedback

---

### 4.2 Backend Server (Flask)

Responsibilities:

- Receive SOS API requests
- Process emergency logic
- Trigger alert distribution
- Log incidents
- Manage storage operations

Design:

- REST API architecture
- Event-driven alert processing
- Modular function separation

---

### 4.3 Alert Engine

Responsibilities:

- Simulate SMS notifications
- Simulate police alert
- Community broadcast simulation
- Multi-channel alert routing

The alert engine acts as an event dispatcher.

---

### 4.4 Evidence Storage System

Responsibilities:

- Store audio/video evidence
- Maintain timestamped logs
- Secure file handling

Implementation:

- Local folder storage (prototype)
- Designed for S3 migration

---

### 4.5 AI Safety Module

Responsibilities:

- Risk zone prediction
- Incident heatmap simulation
- Safe route logic

Implementation:

- Rule-based AI simulation
- Replaceable with ML model in future

---

### 4.6 Database Layer

Responsibilities:

- Store user profiles
- Incident logs
- Alert history

Implementation:

- JSON file database (prototype)
- DynamoDB-ready schema design

---

## 5. Data Flow

1. User triggers SOS
2. Frontend captures location + evidence
3. API request sent to backend
4. Backend processes alert
5. Alerts distributed to contacts
6. Evidence stored securely
7. Tracking session initiated

The system prioritizes immediate alert dispatch.

---

## 6. Security Design

- Evidence stored with timestamp logs
- Controlled backend access
- No external public endpoints
- Local prototype isolation

Future design includes encryption and authentication.

---

## 7. Scalability Design

The architecture is designed for:

- AWS Lambda migration
- DynamoDB integration
- S3 cloud storage
- Real SMS gateway
- Serverless deployment

Prototype simulates scalable behavior.

---

## 8. Reliability Design

- Offline SMS fallback simulation
- Redundant alert triggers
- Local storage persistence
- Fast failure recovery

System designed for unstable connectivity environments.

---

## 9. User Experience Design

- Emergency-first interface
- Large SOS button
- Minimal decision steps
- Immediate feedback
- Stress-safe UI

Focus: usability during panic situations.

---

## 10. Future Design Extensions

- AI voice distress detection
- Wearable device integration
- Government monitoring dashboard
- Community safety network
- Real-time crime analytics
- Multi-language accessibility

---

## 11. Conclusion

RakshaAI’s design demonstrates a modular, scalable, and emergency-optimized architecture. The prototype validates the system flow while enabling seamless transition to cloud infrastructure in future development.

