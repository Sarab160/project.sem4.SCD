🧭 NTU Smart Navigation System
A full-featured desktop-based navigation and information system built for National Textile University (NTU), Faisalabad using Python. This application helps students, faculty, and visitors find optimal walking routes between university buildings, visualize them on an interactive map, and even share these maps using dynamically generated QR codes. The system also integrates real-time weather, NTU services, and a web-based Flask map viewer.
________________________________________
✨ Features
✅ Smart Route Finder:
Find the shortest walkable route between any two NTU buildings using OpenStreetMap and NetworkX.
✅ Interactive Map Visualization:
Routes and buildings are displayed using interactive Folium maps.
✅ QR Code Map Sharing:
Generate a QR code for the map with the calculated route, shareable via a local web server.
✅ Real-time Map Viewer:
Includes a Flask web server that displays custom location maps using coordinates.
✅ University Services Integration:
Quick access buttons to NTU’s official student portal, timetable, notice board, admissions, and more.
✅ Live Weather Access:
Click and view NTU's weather via a preloaded web page.
________________________________________
📌 Tech Stack
Component	Technology Used
GUI Framework	CustomTkinter
Mapping	Folium, OSMnx
Graph Algorithms	NetworkX
Web Server	Flask, http.server
QR Code	qrcode, Pillow
Threading	threading (for async servers)
Web Integration	webbrowser, HTML

 


 


 

 


 


 

📂 Project Structure
ntu-smart-navigation/
│
├── main.py                # Entry point (the script you provided)
├── templates/
│   └── index.html         # Flask landing page
│   └── map.html           # Flask map display
├── rmap.html              # Generated map with route
├── fullmap.html           # Full building map
├── weather.html           # Weather web page
├── qrcode.png             # Dynamically generated QR code
└── README.md              # Project documentation


🧪 Usage
GUI Mode
python main.py
From the GUI:
•	Select start and end buildings to find a route.
•	Click "Generate Map" to visualize.
•	Click "Generate QR" to share the map.
•	Explore NTU services and features via side buttons.
Web Mode
•	Launches Flask on http://127.0.0.1:5000/.
•	You can view your location on a map by entering coordinates.

🌐 Sample QR Code Flow
1.	Calculate the route between two buildings.
2.	Click "Generate QR Code".
3.	A local server (http://127.0.0.1:8000) serves the map.
4.	Scan QR to open the route on any mobile browser (connected to same WiFi).

🧠 Algorithms Used
•	Dijkstra’s Algorithm: Used internally via NetworkX for shortest path.
•	Graph Node Mapping: OSMnx finds nearest road nodes to building coordinates.
•	Polyline Drawing: Folium renders interactive map with building and path markers.

📎 Acknowledgements
•	OpenStreetMap
•	Folium
•	OSMnx
•	NetworkX
•	NTU Website

🏁 End Note
The NTU Smart Navigation System is more than just a mapping tool—it's a demonstration of how smart technologies can be tailored to meet the specific needs of a university environment. Designed and developed with a user-centric and modular approach, this system combines real-time navigation, intelligent chatbot support, QR-based location sharing, and academic services—all within a single desktop application.
This project has served as a comprehensive learning experience, showcasing the integration of various technologies including Python, CustomTkinter, Flask, Folium, NetworkX, and PyTorch. It demonstrates practical implementation of software engineering principles, real-time system design, and user interface development.
We hope this system provides valuable utility to NTU students and serves as an inspiration for further innovation in smart campus solutions

