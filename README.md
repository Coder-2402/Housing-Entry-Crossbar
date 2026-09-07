# Housing Entry Barrier System with ESP32-Based RFID Access Control
![WhatsApp Image 2025-12-02 at 12 06 46](https://github.com/user-attachments/assets/d8c0ac2c-0c15-4f13-928e-cdfbeaf823a1)

## Project Domain
This project focuses on a real-time Iot-Based smart housing access control system using RFID RFC522 for identity verification and IR Obstacle Sensors for vehicle safety monitoring, controlled via an ESP32 microcontroller, integrated with a Servo for mechanical actuation and Google Sheets for real-time cloud data logging.

### Problem Statements
- Physical limitations of security guards in monitoring housing 24 hours a day.
- Potential negligence of security guards in allowing unknown person enter the area without inspection.
- Queues of housing residences during rush hour which is time-consuming and inefficient.

### Goals
- Create a prototype for advanced security system that utilizes ESP 32, RFID for validate access, and servo motor as a crossbar driver.
- Implement an efficient algorithm in processing card identity data to minimize vehicle queue.
- Building an IoT integration by utilizing wireless features on ESP 32 to send notifications and log to database.

### Solution Statements
- Use an RFID RC522 reader to scan and verify the Unique Identifier (UID) of access card for resident authorization.
- Implement an IR Obstacle Sensor (FC-51) as a safety mechanism to detect the presence of vehicles and prevent the barrier from closing prematurely.
- Use an ESP32 microcontroller to manage system logic, local data processing, and WiFi-based internet connectivity.
- Control a Servo Motor to perform mechanical actuation of the gate barrier based on validation and safety inputs.
- Integrate with Google Sheets via Google Apps Script for real-time cloud data logging and centralized access monitoring.
- Include a Buzzer and LED indicators to provide immediate auditory and visual feedback on the access status.

## Prequisites

### Component Preparation

- **ESP32**: Microcontroller for data processing and servo control.
- **RFID RC522 Module**: Reader component for emitting radio waves to read the unique identifier (UID) data from the RFID card.
- **RFID Card**: Passive card that stores identity data in the form of a Unique Identifier (UID) and is used by users to verify their access authority to the system.
- **Servo Motor SG90**: Converts the control signal (PWM) from the ESP32 into a rotational movement from 0° to 90° in order to open and close the gate.
- **IR Obstacle Sensor FC-51**: Ddtect the presence of vehicles in the gate area.
- **5V Active Buzzer**: Provides auditory feedback in the form of a beep sound.
- **LED (Red and Green)**: Visual indicator lights showing the access status.
- **220Ω Resistor**: Used as a current limiter in the LED circuit to prevent damage caused by excessive current.
- **Jumper Wires (Male-to-Male & Female-to-Female)**: Used to connect data and power lines between components in the circuit.
- **Breadboard & Expansion Board**: Prototype boards used to facilitate wiring between the microcontroller pins and sensors.
* **Micro USB Cable**: To supply power from an electrical source to the ESP32 and to upload programs from a computer.
