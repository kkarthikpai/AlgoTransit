# 🚌 AlgoTransit: Hybrid MMAS-ABC for Sustainable Bus Optimization
### Project #49 | Urban Development, Mobility & Smart Cities

![Project Status](https://img.shields.io/badge/Phase-2_Execution-success?style=for-the-badge)
![Tech Stack](https://img.shields.io/badge/Python-HTML%20%7C%20CSS%20%7C%20JS-blue?style=for-the-badge)

## 🌍 Overview
**AlgoTransit** is an AI-driven project designed to optimize public transport driving cycles. By utilizing **Swarm Intelligence**, specifically a hybrid of **Max-Min Ant System (MMAS)** and **Artificial Bee Colony (ABC)** algorithms, we aim to reduce fuel consumption and CO₂ emissions in urban bus networks.

This repository contains:
1.  **The Python Core:** Scripts to process raw GPS data and run the optimization algorithms.
2.  **The Web Dashboard:** A responsive HTML/JS interface to visualize the findings and simulate the results.

🔗 **[View Live Dashboard](https://kkarthikpai.github.io/el-phase-2/)** *(Click here to see the website)*

---

## 🚀 Key Features

* **Real-World Data Processing:** Converts raw GPS logs (Latitude/Longitude) into velocity profiles using Geodesic distance calculations.
* **Hybrid AI Model:**
    * 🐜 **Ant Colony (MMAS):** Constructs a smooth baseline path by filtering traffic noise and erratic acceleration.
    * 🐝 **Bee Colony (ABC):** Refines the path using Eco-Driving logic (speed capping, idle reduction).
* **Efficiency Metrics:** Calculates energy consumption ($v^2$ proxy) to quantify fuel savings.
* **Interactive Visualization:** Comparison graphs of Raw vs. Optimized driving cycles.

---

## 🛠️ Tech Stack

### **Backend & Analysis**
* **Python 3.9**
* **Pandas & NumPy:** Data manipulation and matrix operations.
* **Geopy:** Physics calculations (GPS to Meters).
* **Matplotlib:** Static graph generation.

### **Frontend (Dashboard)**
* **HTML5 & CSS3:** Responsive design and layout.
* **JavaScript (ES6):** Logic for the simulation and feedback forms.
* **Chart.js:** Rendering interactive velocity profile charts.

---

## 📂 Project Structure

```text
el-phase-2/
├── index.html          # Home Page
├── problem.html        # Problem Statement & Objectives
├── tools.html          # Tech Stack & Feedback Form
├── findings.html       # Live Simulation Dashboard
├── about.html          # Team & References
├── style.css           # Global Styling
├── script.js           # Chart Logic & Interactivity
│
├── python_scripts/     # (Optional folder for your logic)
│   ├── process_data.py # Converts JSON/CSV GPS data to Speed profile
│   ├── main.py         # Runs the Hybrid MMAS-ABC Algorithm
│   └── real_bus_cycle.csv # The processed dataset used for simulation
│
└── README.md           # This file