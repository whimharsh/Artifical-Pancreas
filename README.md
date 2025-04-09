# Artificial Pancreas Model using Arduino

This project simulates an artificial pancreas using an Arduino, conductivity sensor, and water pump to model insulin regulation in diabetes management. The system monitors "blood glucose levels" (modeled by water conductivity) and uses a feedback loop to simulate insulin delivery.

## 💡 Project Overview

- **Hardware Used:** Arduino UNO, Conductivity Sensor, MOSFET, Pump, Breadboard, Jumpers, Aluminum Foil
- **Software:** Arduino IDE
- **Control Strategy:** On/Off feedback loop based on sensor threshold; can be upgraded to PID.

## 🔧 Features

- Real-time sensor calibration
- Automatic insulin delivery simulation
- Feedback-based control loop
- Graphical analysis of response over time

## 📁 Directory Structure

- `/Arduino_Code`: Contains the `.ino` file for Arduino
- `/Images`: Circuit diagrams and setup photos
- `README.md`: Project overview and instructions
- `LICENSE`: MIT License (modifiable)
- `.gitignore`: Arduino and system-specific exclusions

## 📷 Circuit Diagram
![Circuit Diagram](Images/circuit_diagram.png)

## 🚀 Getting Started

1. Clone the repo
2. Open `artificial_pancreas.ino` in Arduino IDE
3. Upload to Arduino
4. Follow the setup guide in the [Science Buddies tutorial](https://www.sciencebuddies.org/science-fair-projects/project-ideas/HumBio_p040/human-biology-health/developing-an-artificial-pancreas)

## 📈 Future Improvements

- Implement proportional or PID control
- Use real-time glucose simulators
- Integrate with IoT dashboards for remote tracking

## 🧠 Credits

Based on the science project by Science Buddies  
Adapted and implemented by Harsh Saini

---

© 2025 Harsh Saini | MIT License
