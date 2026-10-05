# AquaSort - Smart Water Quality Classification & Distribution System
**IoTRIX 2.0 Semi-Final Submission**

## 1. Problem Statement & Proposed Solution
* **Problem Statement:** In many industrial and residential setups, water quality fluctuates significantly, leading to the wastage of usable water or contamination of high-purity reserves due to proper real-time sorting mechanisms lacking.
* **Proposed Solution:** AquaSort is an automated, sensor-driven IoT solution that analyzes incoming water parameters in real-time and dynamically routes the water into three specialized storage tanks:
  1. **Potable Water Tank** (High purity for drinking/food processing)
  2. **Non-Potable Water Tank** (Secondary use / general cleaning)
  3. **Agricultural Water Tank** (Suitable for irrigation/farming)

---

## 2. System Architecture & Tech Stack

### System Architecture
Incoming Water Source ➔ Sensor Array (pH, Turbidity, TDS) ➔ Microcontroller Logic ➔ Dynamic Actuator/Valve Control ➔ 3-Tank Routing (Potable / Non-Potable / Agricultural)

### Technology Stack
* **Hardware:** Microcontrollers (ESP32 / Arduino), Water Quality Sensors (pH, Turbidity, TDS/EC), Relay Modules & Solenoid Valves / Servo Actuators.
* **Firmware & Embedded Software:** C / C++ (Arduino Framework / ESP-IDF)
* **Communication Protocols:** Wi-Fi, MQTT / HTTP
* **Software Tools:** Visual Studio Code, GitHub Desktop, MATLAB (Simulation & Analysis)

---

## 3. Current Progress & Proof of Concept
- [x] Initial IoT project concept and three-tank architecture designed.
- [x] Hardware component selection and schematic baseline finalized.
- [ ] Sensor calibration and multi-tank routing logic integration (In Progress).
- [ ] Physical prototype assembly and live test validation (In Progress).

---

## 4. Current Limitations & Risks
* Sensor calibration drift over prolonged exposure to contaminated water.
* Actuator response time delay during high-flow water inlet conditions.

---

## 5. Planned Improvements for Final Round
* Real-time cloud dashboard monitoring for system diagnostics and water usage metrics.
* Predictive filtration alert system based on turbidity data trends.

