# 🤖 Bluetooth-Controlled RC Robot with Ultrasonic Sensor (Arduino Project)

## 📌 Objective

This project focuses on designing and building a remote-controlled robot that utilises Bluetooth communication. The robot is also equipped with an **ultrasonic sensor** for obstacle detection, adding semi-autonomous functionality. The robot can detect obstacles in its path and stop or change direction accordingly, providing both manual control and collision avoidance.

---

## 🔧 Components Used

- **Arduino Uno** (microcontroller)
- **L298N Motor Driver** (to control motors)
- **HC-05 / HC-06 Bluetooth Module** (for wireless communication)
- **HC-SR04 Ultrasonic Sensor** (for obstacle detection)
- **2 DC Motors** (for robot movement)
- **Robot Chassis & Wheels**
- **Jumper Wires**
- **Battery / Power Supply**

---

## 🚀 Features

### 📱 Bluetooth Remote Control
- Controlled via a Bluetooth-enabled device (e.g., smartphone).
- Command format:
  - `'F'` → Move Forward
  - `'B'` → Move Backward
  - `'L'` → Turn Left
  - `'R'` → Turn Right
  - `'S'` → Stop

### 🧠 Obstacle Detection (Autonomous Behavior)
- Ultrasonic sensor mounted at the front.
- Detects obstacles within a **15 cm** range.
- Automatically stops the robot to prevent collisions.

### 🎯 Smooth Motor Control
- Motors controlled via L298N driver.
- **PWM (Pulse Width Modulation)** used for speed regulation.
- Smooth turning and movement transitions.

---

## ⚙️ How It Works

1. **Bluetooth Communication**  
   The HC-05/06 module receives serial commands via the **SoftwareSerial** library on the Arduino.

2. **Movement Control**  
   Commands control the L298N motor driver to drive the robot forward, backward, left, right, or stop.

3. **Obstacle Detection**  
   The HC-SR04 ultrasonic sensor continuously checks for obstacles. If an object is detected within 15 cm, the robot halts to avoid a collision.

4. **Autonomous Integration**  
   Combines remote control with real-time autonomous decision-making for obstacle avoidance.

---

## 🧩 Challenges Faced

- **Bluetooth Interference:**  
  Maintaining stable communication and pairing between the smartphone and HC-05 was sometimes difficult due to signal loss or delay.

- **Sensor Optimization:**  
  Writing the obstacle avoidance logic required careful calibration of distance thresholds and response times for accurate behavior.

---

## 📚 Learning Outcomes

- 🛠️ **Arduino Programming:**  
  Gained hands-on experience in integrating multiple hardware modules and writing efficient Arduino code.

- ⚡ **Motor Driver + PWM:**  
  Learned how to control motor speed and direction using pulse-width modulation.

- 📡 **Wireless Communication:**  
  Understood Bluetooth protocols and managing real-time command input from a mobile device.

---

## 🚀 Future Enhancements

- Add additional sensors (IR or ultrasonic) for full 360° awareness.
- Implement voice command integration via mobile app.
- Build a GUI-based mobile app for real-time sensor feedback and joystick-style control.
- Add path planning for full autonomy.

---

## 🧑‍💻 Author

**Arijit Bhattacharjee**  
🎓 B.Tech CSE | Hardware Enthusiast | Arduino Developer  
🔗 GitHub: [https://github.com/wiskey067](https://github.com/wiskey067)  
📧 Email: [ab9777816@gmail.com]

---

> This project demonstrates a blend of manual control and intelligent behaviour using affordable electronic components. It’s a great starting point for anyone interested in robotics, embedded systems, or IoT.
