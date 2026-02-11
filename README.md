# Jio eAnalytiX - Smart Fire Protection Dashboard

![Status](https://img.shields.io/badge/Status-Prototype-blue) ![Role](https://img.shields.io/badge/Role-Product_Manager-orange)

## 🚀 Product Overview
**Jio eAnalytiX** is an Industrial IoT (IIoT) dashboard designed to provide real-time visibility into critical Fire Protection Systems (FPS) across multi-site facilities.

In large-scale industrial zones, safety officers often struggle with opaque, on-premise hardware data. This solution bridges the gap between physical assets (Pumps, Tanks, Sensors) and digital decision-making, reducing response time to critical safety events.

**[🔗 Try the Live Simulator Here](https://your-link-here)**

---

## 🏗️ System Architecture
The system follows a standard 3-tier IoT topology, ingesting raw telemetry from edge gateways and visualizing it for facility managers.

![Architecture Diagram](assets/architecture_diagram.png)
*(See `specs/` for detailed data schema)*

---

## ✨ Key Features
* **Real-Time Asset Monitoring:** Live status tracking of Main, Jockey, and Diesel pumps (ON/OFF/AUTO/TRIP).
* **Logic-Based Health Scoring:** auto-calculates "Healthy" vs. "Faulty" panel status based on complex boolean logic (e.g., *Panel is faulty if Main Pump is in Manual Mode*).
* **Critical Alert Engine:** Instant generation of visual alerts for pressure drops, tank level breaches, or pump trips.
* **Admin Simulator:** A built-in "Wizard of Oz" controller allowing stakeholders to simulate edge-case scenarios (e.g., sensor failure) without physical hardware.

---

## 🛠️ Technical Specifications
* **Frontend:** HTML5, CSS3, Vanilla JavaScript (Zero dependencies for lightweight deployment).
* **Data Model:** JSON-based payload ingestion mimicking MQTT device packets.
* **State Management:** LocalStorage/In-browser state for simulation persistence.

### Why Vanilla JS?
As a Product Manager prototyping a solution, I chose a zero-dependency approach to ensure the prototype is:
1.  **Portable:** Can run on any machine without `npm install`.
2.  **Transparent:** Logic is visible and easy for engineering teams to audit during handover.
3.  **Fast:** Instant load times for stakeholder demos.

---

## 📖 How to Run Locally
1.  Clone this repository:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/jio-eanalytix-dashboard.git](https://github.com/YOUR_USERNAME/jio-eanalytix-dashboard.git)
    ```
2.  Open `index.html` in any browser.
3.  **To Simulate Data:**
    * Click the **Gear Icon (⚙️)** in the top-right corner.
    * Paste a custom JSON payload (see `specs/data_dictionary.md` for examples).
    * Click **Update** to see the dashboard react in real-time.

---

## 📬 Contact
**[Your Name]** *Product Manager | Industrial IoT & Data Platforms* [LinkedIn Profile Link] | [Email Address]
