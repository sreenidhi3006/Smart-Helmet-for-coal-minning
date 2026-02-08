# Smart-Helmet-for-coal-minning
IoT-based Smart Helmet for Coal Mining using ESP8266 to monitor gas, temperature, and humidity in real time. Provides instant alerts through buzzer and Blynk IoT platform to ensure miner safety. Developed using embedded C and IoT technology.
# Smart Helmet for Coal Mining using IoT

## 📌 Project Description
This project is an IoT-based Smart Helmet designed to improve safety in coal mining environments. The helmet monitors harmful gases, temperature, and humidity in real time using sensors. The ESP8266 microcontroller processes the data and sends it to the Blynk IoT platform for live monitoring. If unsafe conditions are detected, alerts are triggered through a buzzer and IoT notifications.

This system helps reduce accidents and improves miner safety using embedded systems and IoT technology.

---

## 🚀 Features

- Real-time gas detection using MQ gas sensor
- Temperature and humidity monitoring using DHT11
- WiFi-based data transmission using ESP8266
- Live monitoring using Blynk IoT platform
- Emergency alert using push button
- Buzzer alert for unsafe conditions
- Low-cost and efficient safety solution
- Compact and wearable helmet design

---

## 🧰 Components Used

### Hardware Components

- ESP8266 (NodeMCU)
- MQ Gas Sensor
- DHT11 Temperature and Humidity Sensor
- Buzzer
- Push Button
- Jumper Wires
- Breadboard
- Power Supply
- Safety Helmet

### Software Used

- Arduino IDE
- Blynk IoT Platform
- Embedded C/C++

---

## 🔌 Circuit Diagram

The circuit consists of ESP8266 as the main controller connected with sensors and output devices.

### Connections:

- MQ Gas Sensor → Analog pin (A0)
- DHT11 → Digital pin (D4)
- Buzzer → Digital pin (D5)
- Push Button → Digital pin (D6)
- All components connected to 3.3V and GND

The ESP8266 reads sensor data and sends it to the Blynk IoT platform via WiFi.

---

## ⚙️ Working Principle

1. Sensors collect environmental data.
2. ESP8266 processes the sensor data.
3. Data is sent to Blynk IoT platform.
4. If gas level exceeds threshold, buzzer activates.
5. Emergency button sends alert signal.

---

## 📱 Output

- Real-time monitoring on Blynk mobile app
- Buzzer alert during dangerous conditions
- Emergency alert notification

---

## 👩‍💻 Team Members

- Sreenidhi K
- Jeevitha
- Deepika

---

## 🛠️ Technologies Used

- IoT (Internet of Things)
- Embedded Systems
- ESP8266 WiFi Module
- Arduino Programming
- Blynk IoT

---

## 📄 License

This project is developed for educational purposes.
