# 🧭 NTU Smart Navigation System

A real-time, AI-powered smart campus navigation assistant for National Textile University (NTU). This system combines dynamic map routing, friend location sharing, and a responsive academic chatbot—all in one desktop experience.

---

## 📌 Project Summary

The NTU Smart Navigation System is built to help students and faculty navigate the NTU campus intelligently. It enhances campus life with features like:

- Live GPS-based pathfinding  
- QR-code enabled friend finder  
- Chatbot support for academic queries  
- Weather integration and service quick-access  

This cross-functional tool ensures that users always know where they are, where they're going, and how to get there.

---

## 🧩 Core Modules

### 🗺️ Dynamic Campus Mapping
- Uses open-source map rendering tools to display campus buildings and roads.  
- Calculates optimized routes, including building entrances and service paths.

### 📍 Real-Time Friend Locator
- Share your live campus location via QR code.  
- Friends can scan the code and view your current position on a web-based map.  
- Flask server enables real-time map sharing across devices.

### 💬 Academic Assistant Chatbot
- Understands user queries related to subjects, rooms, schedules, and faculty.  
- Trained using natural language processing and custom datasets.  
- Built to respond to both general and university-specific questions.

### ☁️ Weather & Campus Info
- Fetches current weather conditions for the NTU campus.  
- Suggests whether it’s safe to walk across campus in real-time.

---

## 🧠 Technology Stack

| Area        | Tools & Frameworks                                                  |
|-------------|----------------------------------------------------------------------|
| UI          | CustomTkinter, Tkinter                                               |
| Maps        | Folium, Leaflet.js, OSMnx, NetworkX                                  |
| Backend     | Flask, Threading, Requests, Webbrowser                               |
| AI/NLP      | PyTorch, NLTK, custom-trained intent model                           |
| QR System   | qrcode, Pillow                                                       |
| Weather     | PyOWM (OpenWeatherMap API)                                           |

---

## 🧱 System Architecture

1. **Desktop App (GUI Layer)**: Handles all visual components and user interactions.  
2. **Map Engine**: Generates interactive HTML maps using geographical data.  
3. **QR Generator**: Encodes and decodes user locations to enable friend-finding.  
4. **Flask Server**: Launches a local server to serve shared maps.

---

## 🧪 Functional Highlights

- **Shortest Route Calculation**: Includes all access paths and avoids unreachable areas.  
- **Cross-Building Navigation**: Recognizes building-to-building movement logic.  
- **Location Persistence**: User’s location can be encoded, shared, and viewed later.  
- **Multithreaded Operation**: Keeps server, chatbot, and UI responsive simultaneously.  
- **Multi-modal UI**: Switch between navigation, assistant, and utilities effortlessly.

---

## 🎓 University Use Cases

| Use Case              | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| New Student Orientation | Helps freshmen find lecture halls and service offices.                     |
| Faculty Assistance      | Enables professors to locate department rooms or labs.                     |
| Friends Meetup          | Share and follow live location on campus during events.                    |
| Class Schedule Lookup   | Ask chatbot about today's classes and their respective rooms.              |
| Real-time Weather Alerts| View campus-specific weather before heading to a destination.              |

---

## 🧠 Design Patterns

| Pattern     | Functionality                                                                 |
|-------------|-------------------------------------------------------------------------------|
| Singleton   | Ensures shared services like weather or routing run as single instances.      |
| Adapter     | Integrates legacy data or alternative APIs.                                   |
| Strategy    | Switches routing logic (e.g., shortest time vs shortest distance).            |
| State       | GUI transitions smoothly across modes like “Navigation” and “Chatbot.”        |
| Observer    | Updates map view automatically when user location changes.                    |
| Decorator   | Adds optional features to the map without altering base logic.                |
| Facade      | Provides a simplified interface for initiating services.                      |

---


---

## 🏁 End Note

This project was developed to simplify campus navigation and enhance the NTU student experience through real-time location tracking, smart routing, and helpful academic tools. It reflects practical implementation of AI, mapping, and user-friendly design in one integrated system.
