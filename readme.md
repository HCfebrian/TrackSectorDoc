# 🏎️ Go-Kart Tracker Project Roadmap

## 📌 Overview
This project aims to build a **real-time go-kart telemetry system** using ESP32, GPS, a server, and an iOS app for live monitoring.

## 📅 Milestones & Tasks

### ✅ 1. GPS Data Flow (ESP32 → Server)
- [ ] Connect **UBX-M10050-KB GPS module** to ESP32
- [ ] Read GPS data (latitude, longitude, timestamp)
- [ ] Transmit GPS data over **WiFi** to the server
- [ ] Debug and ensure reliable data transmission

### 🖥️ 2. Server Development (Data Processing)
- [ ] Choose communication protocol: **MQTT vs WebSockets**
- [ ] Set up **ZimaBoard** as the server
- [ ] Create an endpoint to receive GPS data
- [ ] Store GPS data in a database or file
- [ ] Implement data parsing & processing

### 🌍 3. Web Visualization (Real-Time Map & Leaderboard)
- [ ] Create `visualization.html`
- [ ] Display kart positions on a **track map**
- [ ] Update kart positions in real-time
- [ ] Implement **dynamic track sectors**
- [ ] Add **leaderboard sorting by real-time position**
- [ ] Add a **clear data button**

### 📱 4. iOS App Development (SwiftUI + MapKit)
- [ ] Create a SwiftUI app
- [ ] Implement **MapKit** to show kart positions
- [ ] Sync data from the server
- [ ] Add UI elements for tracking & leaderboard
- [ ] Optimize for real-time updates

### 🔧 5. Extra Features & Optimizations
- [ ] Improve data accuracy & filtering
- [ ] Implement **lap timing & sector analysis**
- [ ] Design better **UI/UX** for mobile & web
- [ ] Optimize server performance

## 🚀 Next Steps
- Start with **ESP32 GPS setup** and ensure data is flowing to the server.
- Choose the best protocol (**MQTT/WebSockets**) for real-time data transfer.
- Develop a **simple web visualization** before refining leaderboard logic.
- Begin work on the **iOS app** after data transmission is stable.

---
### 📌 Notes
This roadmap will evolve as the project progresses. Keep refining and updating it! 🚀
