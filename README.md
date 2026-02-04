# 🎯 Arduino-Based Automated Radar Targeting System

An **automated radar-guided targeting system** built using **Arduino Uno**, **Ultrasonic and IR sensors**, **dual servo motors**, and a **Processing-based tactical interface**.  
The system performs continuous 180-degree scanning, detects nearby objects, visualizes targets in real time, and actuates a **servo-mounted projectile launcher** automatically.

For demonstration purposes, a **water gun** is used as the projectile launcher.  
With mechanical modifications, the system can be adapted to launch **Nerf-style or other low-power projectiles**.  
**Reloading is manual and not automated.**

---

## 🚀 Key Features

- 📡 Real-time 180° radar scanning
- 🧠 Sensor fusion using Ultrasonic + IR sensors
- ⚙️ Dual servo control:
  - Radar sweep servo
  - Launcher trigger servo
- 🎯 Automated target detection and engagement
- 🖥 Live radar visualization using Processing
- ⚠️ Visual warning and engagement alert
- 🔌 External servo power with common ground
- 🕵️ Tactical / spy-style HUD interface

---

## ⚠️ Safety & Scope Note

This project is intended **strictly for educational and demonstration purposes**.

- Uses **low-power projectile launchers** only (e.g., water gun)
- **No automatic reloading**
- No autonomous targeting beyond short-range sensor detection
- Mechanical launcher modifications are required for other projectile types

---

## 🧰 Hardware Components

- Arduino Uno R3  
- HC-SR04 Ultrasonic Sensor  
- IR Proximity Sensor (Active-Low)  
- 2 × SG90 Servo Motors  
- Servo-mounted projectile launcher (water gun for demo)  
- External 5–6V Battery Pack (for servos)  
- Breadboard & Jumper Wires  

---

## 🔌 Pin Configuration

### Ultrasonic Sensor (HC-SR04)
| Pin | Arduino |
|----|--------|
| VCC | 5V |
| GND | GND |
| TRIG | D9 |
| ECHO | D10 |

### IR Sensor
| Pin | Arduino |
|----|--------|
| VCC | 5V |
| GND | GND |
| OUT | D7 |

### Servos
| Servo Function | Signal Pin |
|---------------|------------|
| Radar Sweep Servo | D6 |
| Launcher Trigger Servo | D5 |

> ⚠️ Both servos are powered using an **external battery**.  
> Battery GND **must** be connected to Arduino GND.

---

## 🧠 System Working

1. Radar servo performs continuous scanning within a fixed 180° field  
2. Ultrasonic sensor measures distance at each angle  
3. IR sensor confirms object presence  
4. Arduino transmits angle, distance, and detection data via serial  
5. Processing renders a real-time radar and HUD interface  
6. When a target is detected within range, the launcher trigger servo is actuated automatically  

---

## 🖥 Software Used

- Arduino IDE  
- Processing IDE  
- Built-in Arduino Servo Library  

---

## 🎯 Applications

- Automated targeting demonstrations  
- Robotics and mechatronics projects  
- Radar and tracking simulations  
- Defense-style UI visualization (educational)  
- Embedded systems learning platforms  

---

## 🚧 Limitations

- Short detection range  
- Single-target response  
- Manual reloading required  
- Projectile launcher must be mechanically modified for different platforms  

---

## 🔮 Future Improvements

- Target lock-on tracking mode  
- Multiple target identification  
- Adjustable firing logic and safety interlocks  
- Wireless control and monitoring  
- Improved launcher mechanisms  

---

## 📜 License

This project is open-source and intended for **educational and non-harmful experimental use only**.
