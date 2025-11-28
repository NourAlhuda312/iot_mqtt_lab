![Header Image](screenshots/ReadMeImage.png)
---

## 🌐 Introduction

This project demonstrates a fully functional **MQTT-based IoT communication system** using the **Mosquitto Broker** and **Paho MQTT client library**.
The idea is to simulate multiple sensors publishing data in real-time and multiple subscribers receiving only the data meant for them — just like real IoT cloud communication.

This lab was created as part of the **IoT & Big Data course**, showcasing practical hands-on experience with MQTT messaging, topic filtering, and multi-terminal interaction.

---

## 🚀 What This Project Does

✔ Runs **Mosquitto MQTT Broker** locally  
✔ Uses **Paho clients** to simulate IoT sensors  
✔ Includes **multiple publishers**:

* 🌡️ Temperature Sensor
* 💧 Humidity Sensor
* 🔢 People Counter Sensor

✔ Includes **multiple subscribers**, each listening to its own topic  
✔ Each message includes  **My ID → 12219823**  
✔ Organized logs + screenshots for both publishers and subscribers

---

## 🧩 System Architecture

MQTT Topics used in this lab:

```
sensors/temperature
sensors/humidity
sensors/people_counter
```

Each publisher sends JSON-like messages containing sensor readings and My ID.
Each subscriber listens to exactly one topic in a dedicated terminal.


## 🎯 Learning Outcomes

Through this lab, I learned:

* How to install & run **Mosquitto MQTT broker**
* How to use **Paho** to publish & subscribe to MQTT topics
* How MQTT handles **topic filtering** and **message flow**
* Multi-terminal real-time IoT communication
* Structuring sensor data for IoT use cases

---

## 👤 Author

**Nour Alhuda Daraghmeh**  
**Student ID — 12219823**

## 👨‍🏫 Instructor

**Dr. Mo'men Abu Ghazaleh**

---

## 📊 MQTT Topics Overview

| Sensor Type | Topic | Publisher File | Subscriber File |
|-------------|-------|----------------|-----------------|
| 🌡️ Temperature | `sensors/temperature` | `pub_temperature.py` | `sub_temperature.py` |
| 💧 Humidity | `sensors/humidity` | `pub_humidity.py` | `sub_humidity.py` |
| 🔢 People Counter | `sensors/people_counter` | `pub_people.py` | `sub_people.py` |
---

**Made with 💙 for IoT Learning**
