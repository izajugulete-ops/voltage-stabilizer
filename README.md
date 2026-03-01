# ⚡ Digital Voltage Stabilizer

![Platform](https://img.shields.io/badge/Platform-Embedded--C-blue)
![Status](https://img.shields.io/badge/Status-Completed-success)

This project is a voltage monitoring and stabilization system designed to protect sensitive electronic equipment from power grid fluctuations. The device measures input voltage in real-time and adjusts the output to maintain a constant level, providing visual feedback to the user via an integrated display.

## 🚀 Key Features

* **Overvoltage Protection:** Automatic power cutoff mechanism when voltage exceeds safety thresholds.
* **Adjustable Output:** Engineered the circuit to provide a stable output voltage between 8.5V and 17V, adjustable via a negative feedback network.
* **Integrated Protection Systems: * Thermal Protection:** Implemented a circuit to limit the series element's temperature to 100°C.
* ** * Overvoltage Protection:** Automatic power cutoff mechanism when voltage exceeds safety thresholds.

## 🛠️ Tech Stack

* **Language:** Embedded C
* **Microcontroller:** (e.g., ATmega328P / Arduino)
* **Peripherals Used:** * **ADC:** For sampling analog voltage signals.
    * **I2C/Parallel LCD:** For the user interface.
    * **GPIO:** For controlling execution elements such as relays.

## 📂 Project Structure

* `voltage_stabilizer.ino` / `main.c`: The primary source code containing the control logic and safety algorithms.
* `lib/`: External libraries used for LCD management and sensor interfacing.
* `.gitignore`: Configured to exclude temporary build files and binary artifacts.

## ⚙️ How It Works

1. **Sensing:** The system reads the voltage from a step-down transformer or a dedicated sensor module.
2. **Processing:** The microcontroller compares the sampled value against a pre-defined reference threshold.
3. **Action:** If the voltage is too low or too high, the system switches relay stages to compensate for the difference.
4. **Safety:** If the voltage reaches a critical range, the system enters "Safe Mode" and disconnects the load to prevent hardware damage.

---
Developed as part of a personal portfolio focusing on **Embedded Systems** and **Analog Electronics**.
