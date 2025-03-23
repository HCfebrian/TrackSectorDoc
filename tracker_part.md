# 🏎️ Go-Kart Tracker - Required Parts

## 📡 1. GPS Tracker (Racer Device)
This is the hardware each racer will use to track and transmit location data.

### 🔧 Required Components
- **ESP32** (for WiFi connectivity & processing)
- **UBX-M10050-KB GPS Module** (for accurate location tracking)
- **Battery (LiPo or 18650 pack)** (for portability)
- **Voltage Regulator** (to ensure stable power delivery)
- **3D Printed / Enclosure** (to protect the components)
- **Wires, Connectors, and PCB (optional)**

### 📌 Notes
- The ESP32 will communicate with the server over WiFi (via an iPhone hotspot).
- GPS accuracy needs to be tested in open track conditions.

---

## 🖥️ 2. Server (ZimaBoard Setup)
The server will handle incoming GPS data, process positions, and manage the leaderboard.

### 🔧 Required Components
- **ZimaBoard** (or another low-power mini PC)
- **SSD / Storage Drive** (to store race data logs)
- **Linux-based OS** (Debian recommended)
- **MQTT Broker / WebSockets Server** (to handle real-time communication)
- **Database (SQLite/PostgreSQL)** (to store race data)

### 📌 Notes
- The server will run a backend service to process incoming GPS data.
- MQTT/WebSockets will be used for real-time communication.
- A web-based dashboard (`visualization.html`) will connect to this server.

---

## 🖥️ 3. Admin Client (Web Dashboard & iOS App)
The admin client is used to monitor racers in real-time and manage the race.

### 🔧 Required Components
- **Web-based Dashboard (`visualization.html`)**
  - JavaScript frontend (WebSockets for real-time updates)
  - Map-based kart tracking
  - Leaderboard sorting logic
  - Sector-based progress tracking
- **iOS App (SwiftUI + MapKit)**
  - Displays kart positions on the track
  - Syncs leaderboard data from the server
  - Allows race officials to monitor lap times & positions

### 📌 Notes
- The web client will be used for **real-time tracking**.
- The iOS app will provide a **mobile-friendly** way to track the race.
- Both clients need efficient real-time data updates from the server.

---
### 🚀 Next Steps
- **Get GPS module working** on ESP32 and test data transmission.
- **Set up the server** with MQTT/WebSockets to handle data flow.
- **Develop a basic visualization** for tracking karts in real-time.

This document will be updated as the project progresses! 🚀
