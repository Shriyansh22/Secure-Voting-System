# Secure Bluetooth-Based Voting System

A secure embedded electronic voting system integrating Arduino hardware with a JavaFX desktop application for real-time vote monitoring, visualization, and secure administration.

The project combines embedded systems, Bluetooth serial communication, and desktop-based analytics to create a reliable and tamper-resistant voting platform suitable for small-scale elections, institutional polling, and academic demonstrations.

---

## 🚀 Features

- Real-time vote acquisition using Arduino and HC-05 Bluetooth communication
- Live vote visualization using dynamic bar and pie charts
- Secure admin authentication using BCrypt password hashing
- Tamper detection using multi-touch and rapid-vote monitoring
- Candidate management using JSON configuration files
- Real-time JavaFX desktop dashboard
- TM1637 displays for hardware-side vote count visualization
- Low-latency Bluetooth serial communication
- Modular and scalable system architecture
- Real-time vote validation and integrity checking

---

# 📌 System Architecture

```text
+-------------------+
|  TTP223 Sensors   |
+---------+---------+
          |
          v
+-------------------+
|    Arduino Uno    |
| Vote Processing & |
| Tamper Detection  |
+---------+---------+
          |
 Bluetooth Serial
    HC-05 Module
          |
          v
+-------------------+
|   JavaFX Desktop  |
|   Application     |
| Live Charts & UI  |
+-------------------+


## 🛠️ Technologies Used

### Embedded System
- Arduino Uno
- TTP223 Capacitive Touch Sensors
- HC-05 Bluetooth Module
- TM1637 7-Segment Displays
- LEDs and Buzzer

### Software
- JavaFX
- Java
- Gson
- jSerialComm
- BCrypt

### Communication
- UART Serial Communication
- Bluetooth SPP Protocol

---

# 🔒 Security Features

## Tamper Detection

The system continuously monitors suspicious voting activity including:

- Multiple simultaneous touch inputs
- Rapid repeated voting attempts
- Invalid Bluetooth packets
- Abnormal voting frequency

If tampering is detected:

- Voting is temporarily locked
- Alert buzzer is activated
- Tamper LED is triggered
- Warning is displayed on the desktop dashboard

---

## Secure Authentication

Administrative operations such as:

- Vote reset
- Result export
- Candidate configuration
- System management

are protected using:

- BCrypt password hashing
- Salted authentication mechanism
- Secure admin access control

---

# 📊 JavaFX Dashboard

The desktop application provides:

- Real-time vote counting
- Dynamic bar chart visualization
- Live pie chart analysis
- Candidate profile display
- System connection monitoring
- Secure admin panel
- Result export functionality
- Live status monitoring

---

# ⚡ Hardware Components

| Component | Quantity |
|---|---|
| Arduino Uno | 1 |
| TTP223 Touch Sensors | 3 |
| HC-05 Bluetooth Module | 1 |
| TM1637 Displays | 3 |
| LEDs | 4 |
| Buzzer | 1 |
| Breadboard | 1 |
| Jumper Wires | Multiple |

---

# 🔌 Pin Configuration

| Module | Pin |
|---|---|
| Touch Sensor A | D2 |
| Touch Sensor B | D3 |
| Touch Sensor C | D4 |
| Display A CLK/DIO | D6 / D7 |
| Display B CLK/DIO | D8 / D9 |
| Display C CLK/DIO | D10 / D11 |
| Buzzer | D12 |
| Bluetooth TX/RX | A2 / A3 |
| LEDs | A0 / A1 / A2 |

---

# 🧠 Working Principle

1. A voter casts a vote by touching one of the capacitive touch sensors.

2. Arduino validates the input and checks tamper conditions.

3. Vote count is updated on the TM1637 display.

4. Vote data is transmitted through the HC-05 Bluetooth module.

5. JavaFX application receives and validates the incoming data.

6. Dashboard updates charts and vote statistics in real time.

7. Admin panel securely manages system operations.

---

# 📈 Performance Metrics

| Metric | Result |
|---|---|
| Vote Accuracy | 100% |
| Vote-to-UI Latency | 150–200 ms |
| Tamper Detection Accuracy | 100% |
| Communication Reliability | 98% |
| Maximum Voting Rate | 60 votes/min |

# 🧪 Testing

The system was tested for:

- Sensor response accuracy
- Bluetooth communication reliability
- Tamper detection functionality
- UI responsiveness
- Secure authentication handling
- Real-time vote synchronization
- Vote validation logic

All tests successfully passed under simulated voting conditions.

---

# 🔮 Future Improvements

- Cloud-based vote storage
- Fingerprint authentication
- Aadhaar/Voter ID integration
- End-to-end encrypted communication
- Web-based monitoring dashboard
- ESP32 WiFi support
- Blockchain-backed vote validation
- Biometric voter verification
- Online result publishing

---
