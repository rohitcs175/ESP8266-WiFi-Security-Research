# ESP8266 WiFi Security Research

> **Disclaimer:** This project is intended **ONLY** for educational purposes and authorized penetration testing.
> Do **NOT** use it on networks without **explicit permission** from the network owner.
> The author is **not responsible** for any misuse of this tool.

## 📌 About
This project demonstrates how an **ESP8266** microcontroller can be used for Wi-Fi penetration testing through **Evil Twin** and **Captive Portal** techniques.  
It scans nearby Wi-Fi networks, clones a selected SSID, hosts a fake login page, and optionally simulates deauthentication to encourage clients to connect.

This project is built purely for **cybersecurity research** and **IoT security awareness**.

---

## ✨ Features
- 📡 Scan and list nearby Wi-Fi networks (SSID, BSSID, Channel)
- 🛰 Select a target network to clone
- 🌐 Create a cloned Wi-Fi hotspot (Evil Twin)
- 🖥 Host a customizable captive portal
- 🔄 Simulate deauthentication of clients (limited by ESP8266 capabilities)
- 📜 Log credentials entered into the captive portal
- 🔒 Educational use for penetration testing and training

---

## 🛠 Hardware Requirements
- ESP8266 board (NodeMCU, Wemos D1 Mini, etc.)
- Micro USB cable
- Computer with Arduino IDE installed
- Internet connection

---

## ⚙️ Installation
1. **Install Arduino IDE**  
   Download from: https://www.arduino.cc/en/software
2. Add the **ESP8266 Board Manager URL**:  
   `File → Preferences → Additional Board Manager URLs`  
3. Go to **Tools → Board → Board Manager** and install **ESP8266 by ESP8266 Community**.
4. Select your ESP8266 board (e.g., NodeMCU 1.0).
5. Install required libraries:
- `ESP8266WiFi`
- `ESP8266WebServer`
- `DNSServer`
6. Clone this repository:
```bash
git clone https://github.com/rohitcs175/ESP8266-WiFi-Security-Research.git
```

7. Open the **.ino** file in Arduino IDE.
8. Connect your Esp8266 borad and select the correct COM Port.
9. Upload the code.

## 🚀 Usage
1. power on the ESP8266 after uploading.
2. Connect to the default access point
-` SSID: WiPhi_34732`
-`Password: d347h320`
3. Open the web interface (usually -`192.168.4.1`).
4. Scan and select the target network.
5. Start the Evil Twin and optional Deauth process.
6. When a client connects to your cloned AP, the captive portal will appear.
7. Entered credentials will be shown in the Arduino Serial Monitor.

## ⚠ Disclaimer
This tool is made for.
*   Cybersecurity traning
*   IoT device security testing
*   Educational demonstratinos

**Do NOT** use it for any malicious or illegal activities.
You are solely responsible for your actions.


