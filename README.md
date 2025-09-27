# Real-Time Landslide Detection System

## Abstract

This project proposes a **cost-effective Landslide Detection System** designed for the timely detection and warning of potential geological hazards. Landslides pose significant risks to life, property, and infrastructure, often occurring suddenly and with little warning. The system uses an **Arduino UNO** microcontroller to integrate a **Soil Moisture Sensor (e.g., FC-28)** and an **SW-420 Vibration Sensor** to monitor critical environmental parameters: **soil saturation** and **ground instability**. Utilizing these inputs, the system provides real-time alerts through a **16x2 I2C LCD display** and an audible **buzzer**, thereby enhancing public safety and enabling proactive responses to potential landslide conditions.

---

## Components Used

The following apparatus is required to build the Landslide Detection System:

| Component | Function |
| :--- | :--- |
| **Arduino UNO** | Processes sensor inputs and controls outputs. |
| **SW-420 Vibration Sensor** | Detects ground vibrations signal instability. |
| **Soil Moisture Sensor (e.g., FC-28)** | Measures soil moisture levels. |
| **Buzzer** | Sounds alerts for critical conditions. |
| **16x2 I2C LCD** | Displays real-time data and alerts. |
| **Jumper Wires** | Connects components. |
| **Breadboard** (Optional) | Used for prototyping connections. |

---

## Working and Demonstration

### Setup and Code Execution

1.  Assemble the components and connect the Arduino to the computer via USB.
2.  Upload the project code using the Arduino IDE.
3.  Open the **Serial Monitor** in the Arduino IDE, set at **9600 baud rate**, to view debug messages.

### Real-Time Monitoring and Results

The system is designed to provide alerts based on two critical conditions:

#### 1. Soil Moisture Alert
* The LCD displays real-time readings of the soil moisture percentage.
* If moisture levels **exceed 60%**, the system triggers an alert.
* The alert message **"Landslide Alert!"** is displayed on the LCD, and an audible alarm is activated through the buzzer.

#### 2. Vibration Detection Alert
* To simulate ground vibrations, gently shake or tap near the **SW-420 sensor**.
* When vibration is detected, a message indicating **"Detected vibration... Activating buzzer."** appears in the Serial Monitor.
* An audible buzzing sound is heard for up to 5 seconds.

---
## Project Image

![photo_6244277060314972284_y](https://github.com/user-attachments/assets/6607bacd-e6f6-4a3e-b989-dc00a7676a9a)

## Advantages

The system offers several advantages for risk mitigation:

* **Early Warning Capability:** Provides real-time alerts for potential landslides, enabling timely evacuations and risk mitigation.
* **Cost-Effective Solution:** Utilizes affordable components, making it accessible for deployment in various regions without high costs.
* **Real-Time Data Display:** Displays soil moisture levels and alerts on the 16x2 I2C LCD, facilitating immediate understanding of conditions.
* **Low Power Consumption:** Operates efficiently, suitable for remote locations with limited power supply.
* **Scalability:** Easily expandable by adding more sensors to cover larger areas or multiple monitoring points.

---

## Limitations

The project has certain constraints to consider:

* **Limited Detection Range:** The system may only monitor specific areas, potentially missing landslides occurring outside the monitored range.
* **Sensitivity Issues:** The vibration sensor may not detect all ground movements, which could lead to false alarms or missed alerts for minor vibrations.
* **Environmental Sensitivity:** Weather conditions, such as heavy rain or snow, can affect sensor performance and accuracy.
* **Maintenance Requirements:** Regular maintenance is needed to ensure sensors function properly, as they can become damaged or corroded over time.
* **Cost Implications:** While initial costs may be low, deploying multiple sensors across larger areas can become expensive.

---







