# RESQ-AI
# 🚑 ResQ-AI: Intelligent Ambulance Dispatch System
> **"Not Nearest, But Fastest."**

## 📖 Overview
**ResQ-AI** is an AI-powered emergency response platform designed to optimize the "Golden Hour." Unlike traditional systems that dispatch the *geographically nearest* ambulance, ResQ-AI uses predictive traffic modeling to dispatch the ambulance that will arrive **fastest**. It also integrates real-time hospital bed availability to prevent "patient bouncing" (rejection due to lack of capacity).

## 💡 The Problem
1.  **Inefficient Dispatch:** Traffic congestion often means the closest ambulance (distance) is not the quickest to arrive (time).
2.  **Hospital Rejection:** Patients are often routed to the nearest hospital, only to be turned away because ICU/Trauma beds are full.
3.  **Static Routing:** Drivers lack real-time decision-making support when traffic conditions change mid-journey.

## 🚀 The Solution
ResQ-AI solves this with a three-part ecosystem:
1.  **Smart Dispatch Engine:** Calculates real-time ETAs for all available ambulances using Google Maps Routes API to find the lowest Time-to-Arrival.
2.  **Hospital Sync:** A dashboard for hospitals to update bed status instantly. The system only routes patients to hospitals with *confirmed* availability.
3.  **Dynamic Rerouting:** Continuously monitors traffic during the trip and proactively reroutes drivers to save critical minutes.

## 🛠️ Tech Stack & Google Technologies
This project leverages the following Google technologies:
* **Google Maps Platform:**
    * **Routes API:** For calculating precise ETAs and identifying traffic bottlenecks.
    * **Distance Matrix API:** To compare travel times for multiple ambulances simultaneously.
* **Firebase Realtime Database:** For millisecond-latency synchronization of ambulance GPS locations and hospital bed status.
* **Flutter:** Used to build the cross-platform Driver App (Android/iOS) and Hospital Admin Panel (Web).
* **Vertex AI (Concept):** For training models on historical traffic data to predict congestion zones.


## ⚙️ How to Run the Prototype
Since this is a hackathon MVP, the core interface logic is demonstrated via high-fidelity interactive simulations.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/RESQ-AI.git](https://github.com/your-username/RESQ-AI.git)
    ```
2.  **Open the Simulation:**
    * Navigate to the `mvp-screens/` folder.
    * Open `dispatch_map.html` in your browser to see the **Dispatcher View**.
    * Open `driver_application.html` to see the **Mobile Navigation View**.
    * Open `hospital_dashboard.html` to see the **Admin Panel**.

## 🔮 Future Roadmap
* **🚦 Green Corridor Integration:** Connecting with Smart City Traffic Lights to auto-clear intersections for approaching ambulances.
* **🚁 Drone First-Responders:** Deploying AED-carrying drones for "Zone Zero" immediate response.
* **⌚ Wearable API:** Auto-dispatching ambulances based on critical health alerts (e.g., Apple Watch Fall Detection).

## 👥 Team
* **Team Lead:** Pratham Shah
* **Developer:** Pratham Shah,Nirvaan Shetty,Lucky Solanki
* **Designer:** Pratham Shah,Nirvaan Shetty,Lucky Solanki

---
*Built for GDG On Campus TechSprint 2024*
