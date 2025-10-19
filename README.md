# 🌾 IoT-Based Strawman’s Eye

## 📌 Project Overview
**IoT-Based Strawman’s Eye** is an intelligent crop protection system developed using IoT technology.  
It monitors agricultural fields and automatically detects animal movements to prevent crop damage.  
The system combines real-time surveillance, motion detection, and automated image capture with email alerts.

---

## ⚙️ Key Features
- **ESP32-CAM Integration:** Captures images in real-time and transfers them using Wi-Fi.  
- **PIR Motion Sensor:** Detects movement in the crop area with high sensitivity.  
- **Servo Motor Mechanism:** Rotates between **0° to 180°** to cover a wide surveillance range.  
- **Email Notification System:** Automatically sends captured images to a registered email when motion is detected.  
- **Compact and Cost-Effective:** Designed as a low-power, low-cost solution ideal for rural and agricultural environments.

---

## 🧠 Working Principle
1. The **PIR sensor** detects any motion in front of it.  
2. Once motion is detected, the **ESP32-CAM** captures an image.  
3. The **servo motor** continuously rotates from 0° to 180° to scan the entire field area.  
4. The captured image is **sent to a pre-registered email ID** via the ESP32-CAM’s Wi-Fi and SMTP configuration.  
5. The system resets and continues monitoring for the next motion event.

---

## 🔧 Hardware Components
- ESP32-CAM Module  
- PIR Motion Sensor (HC-SR501)  
- SG90 Servo Motor  
- Jumper Wires  
- Power Supply Module (5V)  
- Breadboard or PCB Mount  
- Supporting Casing/Structure  

---

## 💻 Software Requirements
- Arduino IDE  
- ESP32 Board Package  
- Libraries:
  - `ESP32_MailClient.h`
  - `Servo.h`
  - `WiFi.h`

---

## 🧩 Circuit Connections
| Component | ESP32-CAM Pin |
|------------|---------------|
| PIR Sensor Output | GPIO 13 |
| Servo Signal | GPIO 12 |
| Power (VCC) | 5V |
| Ground (GND) | GND |

---

## 🚀 How It Works
1. Upload the Arduino code to the ESP32-CAM using an FTDI module.  
2. Connect to Wi-Fi and configure the SMTP email settings.  
3. Place the setup in the crop field for monitoring.  
4. When motion is detected, the servo rotates, ESP32-CAM captures an image, and sends it to the email.  

---

## 📫 Output
- Motion detection captured via PIR sensor  
- Image sent directly to registered email inbox  
- Continuous surveillance between 0°–180°  

---

## 🧰 Technologies Used
**ESP32-CAM | PIR Sensor | Servo Motor | IoT | Email Automation (SMTP)**

---

## 🏁 Outcome
Successfully developed a smart IoT-based surveillance prototype that enhances crop security by detecting intrusions and alerting farmers remotely through real-time image emails.

---

## 📷 Project Preview
![IoT-Based Strawman’s Eye](your-image-link-here)

---

### 💡 Future Improvements
- Add night vision capability using IR LEDs  
- Implement SMS alerts or Telegram bot notifications  
- Use solar power for sustainable operation  

---

**Author:** Anurag Purohit  
**Field:** IoT | Embedded Systems | Smart Agriculture  
