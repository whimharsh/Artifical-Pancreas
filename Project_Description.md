# Project Description

## 🩺 Artificial Pancreas Model – Detailed Overview

This project models the functionality of an artificial pancreas using an Arduino-based system. It simulates blood glucose regulation by using water conductivity to represent glucose levels and a pump to simulate insulin delivery.

### 🧪 Working Principle

- **High Conductivity** (tap water) = Low blood sugar
- **Low Conductivity** (distilled water) = High blood sugar
- The Arduino reads the conductivity sensor value.
- If the "blood sugar" is too high (low conductivity), it turns on the pump to add tap water (simulated insulin).
- Once the level stabilizes at the defined threshold, the pump turns off.

### 🧰 Components Used

- Arduino Uno
- Breadboard & Jumper Wires
- Conductivity Sensor (Aluminum foil + floating base)
- MOSFET (for pump control)
- Submersible Water Pump
- Resistors (e.g., 100 kΩ)
- USB cable & Alligator Clips
- Containers with Distilled and Tap Water

### ⚡ Circuit Connections

1. **Power:**
   - Arduino 5V → Breadboard Power Rail (+)
   - Arduino GND → Breadboard Ground Rail (-)

2. **MOSFET:**
   - Gate → Digital Pin 11
   - Drain → Pump negative terminal
   - Source → GND

3. **Sensor Circuit:**
   - One foil strip → A0 (via resistor)
   - Other foil strip → GND

4. **Pump Circuit:**
   - Positive terminal → 5V
   - Negative terminal → MOSFET middle pin

See the diagram for a visual overview.

---

## 🔁 Feedback Control Logic

- `analogRead()` is used to read sensor voltage
- A threshold is set based on calibration
- If reading > threshold, pump activates
- Pump stops when threshold is reached

## 📊 Data Collection

Readings are visualized using Serial Monitor or exported to CSV for graphing in Excel or Google Sheets.

