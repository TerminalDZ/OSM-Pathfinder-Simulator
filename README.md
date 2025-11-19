# 🌍 OSM Pathfinder Simulator

> **An interactive simulator for pathfinding algorithms on real-world maps using OpenStreetMap data.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Leaflet](https://img.shields.io/badge/Map-Leaflet.js-green)](https://leafletjs.com/)
[![Data](https://img.shields.io/badge/Data-OpenStreetMap-blue)](https://www.openstreetmap.org/)

## 📖 About the Project

This project is a powerful educational and interactive tool designed to simulate how famous pathfinding algorithms (such as **A\*** and **Dijkstra**) work on **real-world road networks**, rather than abstract grids.

The application dynamically fetches real road data (Nodes & Ways) from **OpenStreetMap** servers based on the area selected by the user. It then constructs a graph structure directly within the browser and visualizes the algorithm's execution step-by-step in real-time.

## ✨ Key Features

* 🗺️ **Real-World Data:** Does not use fake grid squares; relies on actual geographical coordinates and road intersections.
* 🧠 **Multiple Algorithms:** Supports the most popular search algorithms:
    * **A* Search Algorithm:** Smart and fast, using heuristics.
    * **Dijkstra's Algorithm:** Guarantees the absolute shortest path.
    * **Breadth-First Search (BFS):** For unweighted exploration.
* ⚡ **Speed Control:** Full control over simulation speed (from **1x** down to **0.1x**) to study the algorithm's behavior in detail.
* 📊 **Live Statistics:** Instant display of explored nodes count, path length in kilometers, and actual processing time.
* 🎨 **Modern UI:** Sleek **Glassmorphism** design, fully responsive using **Tailwind CSS**.
* 📍 **Interactive:** Drag and drop start/end markers anywhere on the map.

## 🛠️ Technologies Used

* **HTML5 & Vanilla JavaScript (ES6+):** Core logic and project structure.
* **Leaflet.js:** Interactive map library.
* **Overpass API:** To fetch vector road data (Ways/Nodes) from the OSM database.
* **Tailwind CSS:** For rapid and professional UI styling.
* **FontAwesome:** For icons and symbols.

## 🚀 How to Run

This project is fully **client-side** and requires no package installation (No `npm install` needed).

1.  **Clone** the repository or download the source code.
    ```bash
    git clone https://github.com/terminaldz/OSM-Pathfinder-Simulator.git
      ```
2.  Open the `index.html` file directly in any modern web browser (Chrome, Firefox, Edge).
3.  Enjoy the simulation!

## 🧠 How It Works

1.  **Select Points:** The user positions the Start (Green) and End (Red) markers.
2.  **Fetch Data:** The app sends a bounding box query to the **Overpass API** to retrieve all drivable roads in the vicinity.
3.  **Graph Construction:** Raw OSM data is parsed into an adjacency list graph structure in the browser memory. Intersections become "Nodes" and roads become "Edges" with weights based on physical distance.
4.  **Run Algorithm:** The selected algorithm runs on this graph. A visual delay mechanism allows the user to see the "Frontier" (Yellow nodes) expanding.
5.  **Path Reconstruction:** Once the target is reached, the path is traced back and drawn in Blue.


## 👨‍💻 Developer

Developed by **Idriss Boukmouche**.

* Github: [@terminaldz](https://github.com/terminaldz)
