# 🏭 Industrial Data Acquisition & Control System (DAQ) 
*A modern, responsive desktop application for real-time hardware monitoring, sensor scaling, and relay automation.*

> **Note:** This repository serves as a visual and architectural portfolio. Due to NDA/proprietary constraints, the full source code is kept private. Below is a comprehensive demonstration of the application's interface, core features, and system architecture.

---

## 🎥 Video Demonstration


[[Watch the Demo]](https://github.com/daaa-z1/TestBenchExpert/blob/main/docs/2026-07-23%2015-27-13.mkv)
*Click the link to watch the full video demonstration.*

---

## 📸 Interface Gallery

| Gauge Panel | Configuration Panel |
| :---: | :---: |
|<img width="1919" height="771" alt="Screenshot 2026-07-23 162341" src="https://github.com/user-attachments/assets/34afec5b-1944-495c-8e5d-18d1eb7244e2" />| <img width="1916" height="301" alt="Screenshot 2026-07-23 162518" src="https://github.com/user-attachments/assets/d8e7676b-bd5c-4e36-9638-67c42c3d4609" />|
| *Real-time monitoring of Pressure, Flow, and Temperature.* | *Dynamic sensor scaling, limit configuration, and relay control.* |

---

## 🚀 Project Overview
This application was developed to interface with the **DAQ hardware**, bridging the gap between raw physical sensor data and a user-friendly digital interface. It handles multi-channel analog inputs, applies mathematical scaling in real-time, and controls a matrix of digital relays.

The application allows operators to monitor critical industrial parameters safely, configure system limits via a local database, and export test results for reporting.

---

## ✨ Key Features Developed
*   **Real-Time Data Processing:** Continuously reads and processes 10 analog inputs at high frequency (10ms intervals), calculating exact physical values based on configurable min/max scales.
*   **Relay Automation Control:** Intelligent control logic for 23 digital outputs, ensuring safe switching states (e.g., mutually exclusive relay activations).
*   **Dynamic Database Configuration:** Uses a local database to store and retrieve user-defined parameters, including sensor limits, scaling factors, and default hardware states.
*   **Automated Data Logging:** Features a built-in test data exporter that formats real-time session data and saves it directly into structured CSV files for post-analysis.
*   **Separation of Concerns (Architecture):** Implemented a robust architecture separating the backend logic (Python/PyQt5) from the frontend presentation (QML), ensuring a smooth, non-blocking UI.

---

## 🛠️ Tech Stack & Technologies
*   **Backend System:** Python 3
*   **Frontend / UI:** PyQt5, QML (Qt Modeling Language)
*   **Hardware Integration:** Hardware Driver Library
*   **Database:** SQLite (via Python DB-API)
*   **Data Handling:** CSV, Math calculations

---

## 💡 My Technical Contributions
As the primary developer for this software, my responsibilities included:
1.  Designing the asynchronous communication bridge between the Python backend (`QObject`, `pyqtSignal`, `pyqtSlot`) and the QML frontend.
2.  Developing the mathematical models to translate raw voltage inputs from the LabJack into accurate, human-readable units (Pressure, Current, Temperature).
3.  Architecting the SQLite database schema to allow multiple "Configurations" or profiles, enabling operators to switch machine setups instantly.
4.  Implementing safety constraints in the code to prevent conflicting relay activations (e.g., ensuring `Relay1` and `Relay2` cannot be triggered simultaneously).

---

## 📫 Let's Connect
I am currently open to new opportunities in Software Engineering, UI/UX Development, and Python Development.

*   **LinkedIn:** [Connect!](https://www.linkedin.com/in/huda-rahmat)
*   **Email:** [Mail](mailto:hudac00@gmail.com)
*   **Instagram:** [DM!](www.instagram.com/iydaaaiy)
