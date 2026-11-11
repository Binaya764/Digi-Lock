# 🛡️Digi-Lock — Smart Home Authentication System

> A modern, real-time IoT smart home security platform integrating biometric hardware with a responsive web dashboard.

---

## 🌟 Overview

**Digi-Lock** is an intelligent access control system designed to bridge physical hardware with cloud-connected software. Built for modern smart homes, it provides instantaneous biometric verification, secure user enrollment, and live status monitoring through a clean, centralized web interface.

---

## ✨ Key Features

* **Biometric Access Control:** Fast, secure fingerprint recognition that instantly validates authorized residents and actuators.
* **Smart User Enrollment:** A streamlined, two-step registration process that separates biometric scanning from database profile creation to ensure data accuracy.
* **Real-Time Dashboard Monitoring:** Live status updates tracking whether doors are locked or unlocked, alongside hardware connectivity indicators—all without manual page refreshing.
* **Fail-Secure Architecture:** Designed with robust security defaults, ensuring the system prioritizes locked states and safety protocols during unexpected network or hardware disconnects.
* **Comprehensive Audit Trail:** Tracks and logs access events in real time for complete household security oversight.

---

## 🛠️ Technology Stack

* **Frontend Dashboard:** React.js, Tailwind CSS for a sleek, modern UI.
* **Backend Core:** Node.js & Express.js handling business logic and API requests.
* **Real-Time & Hardware Communication:** Socket.io and lightweight WebSockets for sub-second hardware-to-browser telemetry.
* **Database:** MongoDB for secure, structured user profile and access log storage.
* **Hardware Simulation:** ESP32 Microcontroller environment (simulated via Wokwi).

---

## 🔄 How It Works

1. **Verification Mode (Default):** When a user places a finger on the sensor, the hardware communicates with the backend server, which instantly evaluates the fingerprint against approved database records and triggers the door lock mechanism.
2. **Enrollment Mode:** Administrators can initiate a secure registration session from the web dashboard. The system captures the new biometric signature safely and links it to a user profile before saving it to the database.
3. **Live Telemetry:** The hardware continuously pings its status to the server, which broadcasts the live lock state to the web dashboard so administrators always know the exact state of their entry points.

---

## 🚀 Quick Start Guide

### Prerequisites
* Node.js installed on your machine
* MongoDB database instance (local or cloud)

### Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/dwarpal-smart-lock.git](https://github.com/your-username/dwarpal-smart-lock.git)
   cd dwarpal-smart-lock
