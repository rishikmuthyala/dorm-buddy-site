# DormBuddy 🏠💡

Smart IoT Dorm Hub Built in 36 Hours at HackUMass XI

Real-time roommate coordination through hardware + software integration.

## 🎯 The Problem

Ever knocked on your roommate's door only to find them sleeping? Or wondered if they're even in the room? DormBuddy eliminates the guesswork - an IoT system that bridges physical and digital, giving roommates instant visibility into room status through hardware indicators and a web app.

## ⚡ What It Does

🚪 **Smart Door Monitoring** - Ultrasonic sensor detects door status with real-time sync to web dashboard

💡 **Visual Availability System** - RGB LED indicators show roommate status at a glance:
- 🟢 Green: Available - come on in!
- 🟡 Yellow: Busy - knock first  
- 🔴 Red: Do Not Disturb

🌡️ **Environmental Dashboard** - Live temperature and humidity monitoring with historical tracking

📱 **Remote Control** - Update your status from anywhere - instant LED changes reflected on hardware (sub-500ms latency)

## 🛠️ Tech Stack

**Hardware:** Arduino (C++), Ultrasonic Sensor, DHT22, RGB LEDs, LCD Display

**Backend:** Node.js, Express, MongoDB Atlas, JWT, Railway

**Frontend:** Next.js 13, Tailwind CSS, WebSockets, Vercel

**Infrastructure:** Docker, Railway, MongoDB Atlas

## 📸 Hardware Setup

![Arduino IoT Hub](path/to/image1.png)

![System in Action](path/to/image2.png)

## 🚀 Key Technical Achievements

**Bi-Directional IoT Communication** - Arduino polls backend every 5 seconds. Web commands execute on hardware within 500ms. Perfect sync between hardware and web app state.

**Production-Ready Architecture** - JWT authentication with secure token refresh. MongoDB schema designed for multi-device scaling. Error handling and retry logic for unreliable WiFi. Rate limiting to prevent API abuse.

**Real-Time Data Pipeline** - Sensor data flows from Arduino → Express API → MongoDB → WebSocket broadcast → Next.js UI in under 500ms total latency.

## 🔗 Project Repositories

💻 [Frontend (Next.js)](https://github.com/AbhiK1212/dorm-buddy-site)

⚙️ [Backend (Node/Express)](https://github.com/AbhiK1212/dorm-buddy-backend)

🔌 [Hardware (Arduino)](https://github.com/AbhiK1212/dorm-buddy-arduino)

## 🧠 What I Learned

**Technical Wins:** IoT Architecture - bridging Arduino constraints with cloud scalability. Real-time Systems - minimizing hardware-web communication latency. C++ on Embedded - writing efficient code within memory constraints. Full-Stack Integration - coordinating 3 codebases as one system.

**Challenges Overcome:** Implemented exponential backoff for WiFi reliability. State synchronization to prevent conflicting hardware/web states. JWT auth despite hardware processing limitations.

**If I Built This Again:** Add MQTT for more efficient real-time communication. Implement WebSocket directly to Arduino (no polling). Create multi-room support for entire dorm floors.

## 🤝 The Team

Built by four UMass engineers in 36 hours:

**Rishik Muthyala** - Lead Arduino integration, backend API, system architecture

**[@AbhiK1212](https://github.com/AbhiK1212)** - Next.js frontend, WebSocket implementation

**[@romanobro56](https://github.com/romanobro56)** - Backend infrastructure, JWT auth, DevOps

**Jaden Borla** - Hardware assembly, sensor calibration, installation

## 🏆 HackUMass XI - November 2024

36-hour sprint from concept to deployed IoT system. Why we built this: Every college student deals with awkward roommate situations. We turned a universal dorm problem into a technical solution that people actually use.

## 📬 Connect

**Rishik Muthyala**

🌐 [Portfolio](https://rishikmuthyala.com) | 💼 [LinkedIn](https://linkedin.com/in/rishik-muthyala) | 📧 rishik@example.com

Currently: AI Engineer @ Handshake AI | CS + Math @ UMass Amherst | Building EducatEd.AI

## 📝 License

MIT License - Free to use for your own IoT projects!

---

⭐ Star this repo if you found it interesting!

Built with 💻 + 🔌 + ☕ at UMass Amherst

Making dorm life smarter, one LED at a time
