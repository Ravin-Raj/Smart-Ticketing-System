# 🎟️ Smart Rail Ticketing System Using RFID

An **IoT-based railway ticketing solution** designed to automate the ticket validation process using **RFID technology**.  
Built with **NodeMCU ESP8266**, **MFRC522 RFID module**, **Servo Motor**, **Firebase**, and **Twilio**, this system enables seamless ticket verification, real-time updates, and automated gate control with SMS notifications.

---

## 🚆 Overview

The **Smart Rail Ticketing System** modernizes railway ticketing through contactless validation.  
Each passenger carries an **RFID-embedded ticket**, which is scanned at entry and exit gates.

- On scanning, **NodeMCU** reads the RFID tag and verifies it in **Firebase**.  
- If valid, the **servo motor** opens the gate and a **Twilio SMS** confirms journey start or completion.  
- This ensures secure, fast, and efficient boarding and deboarding processes.

---

## 🧩 Components Used

| Component | Description |
|------------|-------------|
| **NodeMCU ESP8266** | IoT controller with built-in Wi-Fi for Firebase and Twilio communication |
| **MFRC522 RFID Reader** | Detects RFID tags and retrieves passenger details |
| **Servo Motor** | Controls physical gate movement upon verification |
| **Jumper Wires** | Connections between components for prototyping |

---

## 💻 Software Tools

| Software | Purpose |
|-----------|----------|
| **Arduino IDE** | Programming and uploading code to NodeMCU |
| **Firebase** | Real-time cloud database for ticket details |
| **Twilio API** | Sends automated SMS alerts for journey status |

---

## ⚙️ Working Principle

1. Passenger scans RFID-enabled ticket at the entry gate.  
2. **NodeMCU** reads the tag and authenticates details via **Firebase**.  
3. Upon validation:
   - Gate opens using **Servo Motor**.
   - SMS sent via **Twilio**: “Your journey has started.”  
4. Passenger scans again at the destination gate.  
5. System updates status and sends SMS: “Your journey has been completed.”  

---

## 🧠 Code Flow Summary

1. Establish Wi-Fi and Firebase connection using credentials.  
2. Initialize RFID module and Servo motor.  
3. Continuously check for card presence.  
4. On tag detection:
   - Extract Name, Ticket ID, and Mobile Number.
   - Send data to Firebase.
   - Trigger gate servo movement.
   - Send SMS via Twilio API.
5. Reset and wait for the next card.

---

## 🚀 Advantages

- **Fast & Contactless Verification** – Reduces queues and manual checks.  
- **Improved Security** – RFID tags are harder to counterfeit.  
- **Real-time Notifications** – SMS updates ensure transparency.  
- **Automated Gate Access** – Fully unmanned ticket validation.  
- **Eco-Friendly** – Paperless digital system.  

---

## 🔮 Future Enhancements

- Mobile app integration for passenger management.  
- Blockchain-based ticket verification for enhanced security.  
- Multi-modal support (Bus, Metro, Airport).  
- AI for passenger tracking and analytics.  
- Fine generation for expired or invalid tickets.  

---

## 🧾 Conclusion

This RFID-based railway ticketing system demonstrates how **IoT and automation** can revolutionize public transportation.  
By integrating **contactless validation**, **real-time database updates**, and **automated gate control**, it enhances efficiency, accuracy, and passenger experience while reducing manual workload.

---

## 👨‍💻 Team Members

- **G. Nandhagopal (23322001)**  
- **M. Madhavan (23322008)**  
- **S. Ravin Raj (23322009)**  

**Department of Computer Science and Applications**  
**The Gandhigram Rural Institute (Deemed to be University)**  
*December 2024*

---

## 📚 References
- [Twilio ESP8266 SMS Integration](https://www.twilio.com/en-us/blog/how-to-send-sms-messages-esp8266-cpp)  
- [Firebase with NodeMCU](https://www.javatpoint.com/iot-project-google-firebase-nodemcu)  
- [RFID RC522 Interfacing](https://www.electronicwings.com/nodemcu/rfid-rc522-interfacing-with-nodemcu)  
- [Servo Motor Control with NodeMCU](https://www.instructables.com/Interfacing-Servo-Motor-With-NodeMCU/)  
- [Arduino Forum Discussion](https://forum.arduino.cc/t/esp8266-nodemcu-communication-failure-with-mfrc522-rfid-module/1183368)

---

## 🪪 License
This project is developed for **academic and research purposes**.  
Free to use and modify under the **MIT License**.
