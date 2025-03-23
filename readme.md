# 🏎️ Go-Kart Tracker
A real-time go-kart tracking system that allows racers, officials, and spectators to monitor race progress, kart positions, and leaderboard standings.

## 📌 Overview
This project consists of three main components:
1. **GPS Tracker (Racer Device):** A portable device mounted on each kart to collect and send GPS data.
2. **Server:** Processes GPS data, calculates positions, and manages the leaderboard.
3. **Admin Client:** A web dashboard and iOS app for monitoring live race data.

## 🚀 Features
- **Real-time GPS tracking** using WiFi-enabled ESP32 modules.
- **Dynamic leaderboard** based on actual race positions.
- **Web-based visualization** for live monitoring.
- **iOS app integration** for race officials to track lap times and positions.

## 📂 Project Structure
- `gps_tracker_parts.md` → List of required components for racer devices.
- `server_parts.md` → Required hardware and software for the server.
- `admin_client_parts.md` → Components needed for the web and iOS monitoring applications.

## 🔧 Setup Guide
1. **Prepare GPS Tracker:** Assemble the hardware and configure the ESP32 to transmit data.
2. **Set Up Server:** Install dependencies, configure MQTT/WebSockets, and deploy the backend.
3. **Deploy Admin Client:** Launch the web dashboard and iOS app for live tracking.

## 📝 Contributing
Contributions and suggestions are welcome! Feel free to open an issue or submit a pull request.

## 📜 License
This project is licensed under [MIT License](LICENSE).
