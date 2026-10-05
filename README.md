# AquaSort V1.1 - Smart Water Quality Classification & Dual Tank Sorting System
**IoTRIX 2.0 Semi-Final Submission**

## 1. Problem Statement & Proposed Solution
* **Problem Statement:** In many industrial and residential setups, municipal and well water quality fluctuates significantly with unannounced contamination, leading to the wastage of usable water or contamination of entire domestic bulk reserves due to lack of real-time inline verification[cite: 9].
* **Proposed Solution:** AquaSort V1.1 is an automated, sensor-driven IoT gatekeeper solution that analyzes incoming water parameters in real-time under static hold conditions and dynamically routes the water into two specialized storage tanks based on SLS 614:2013 / WHO Potable Water standards[cite: 9]:
  1. **Tank 1 (T1 - Potable Water Tank):** 500L storage for high-purity water dedicated to Drinking and Cooking[cite: 9].
  2. **Tank 2 (T2 - Non-Potable Water Tank):** 500L storage for non-compliant water diverted to secondary utility uses (Laundry, Flushing, Gardening)[cite: 9].

---

## 2. System Architecture & Tech Stack

### System Architecture
Incoming Water Source ➔ 1–2L Stabilization Vent Chamber ➔ 10L Acrylic Sampling Tank (Tsample) ➔ 5-Sensor Array (pH, TDS, Turbidity, ORP, Temp via 16-Bit ADS1115 ADC + ATC) ➔ ESP32 4-State Controller Logic ➔ Dual Solenoid Routing ➔ 2-Tank Storage (T1 Potable / T2 Utility)[cite: 9]

### Technology Stack
* **Hardware:** Microcontrollers (ESP32 DevKit V1 SoC + ADS1115 16-Bit I2C External ADC), Sensors (E-201-C pH, Titanium TDS, TSD-10 Turbidity, Platinum ORP, DS18B20 Temp, XKC-Y25-V Non-contact Level Switches, JSN-SR04T Waterproof Ultrasonic Level Sensors), 12V DC Zero-Pressure Solenoid Valves[cite: 9].
* **Firmware & Embedded Software:** C / C++ (Arduino Framework / ESP-IDF) executing 4-State Machine (FILL ➔ STABILIZE ➔ SAMPLE ➔ DRAIN)[cite: 9].
* **Communication Protocols:** Wi-Fi, MQTT / HTTP Telemetry[cite: 9].
* **Software Tools:** Visual Studio Code, GitHub Desktop, Dedicated IoT Interactive Web Dashboard & Mobile Interface[cite: 9].

---

## 3. Current Progress & Proof of Concept
- [x] Detailed AquaSort V1.1 project proposal and mechanical 2-tier sampling architecture designed[cite: 9].
- [x] SLS 614:2013 standard decision matrix, sensor suite specs, and Bill of Materials (BOM) finalized within 28,082 LKR budget[cite: 9].

---

## 4. Current Limitations & Risks
* Sensor probe crosstalk and electrical interference during simultaneous immersion (Mitigated via >3 cm spatial separation and signal isolation)[cite: 9].
* Hydrodynamic turbulence and micro-air bubble measurement drift (Mitigated via top 1–2 L stabilization vent chamber and 3.5s static hold period)[cite: 9].

---

## 5. Planned Improvements for Final Round
* Complete real-time cloud analytics dashboard with automated alerts for industrial chemical/acidic effluent surges[cite: 9].
* Predictive filtration maintenance alerts and valve life-cycle diagnostics based on cumulative water telemetry data[cite: 9].