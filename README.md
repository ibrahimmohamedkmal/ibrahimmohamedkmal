<h1 align="center">Ibrahim Mohamed — Embedded Systems & IoT Engineer</h1>

<p align="center">
  <b>C/C++ · ESP32 (ESP-IDF / PlatformIO) · FreeRTOS · MQTT · Modbus · Yocto Linux · AVR</b>
</p>

<p align="center">
  <a href="https://linkedin.com/in/ibrahim-mohamed-mostafa">LinkedIn</a> ·
  <a href="mailto:ibrahim.mohamed.kmal@gmail.com">ibrahim.mohamed.kmal@gmail.com</a> ·
  Giza, Egypt
</p>

---

## About Me

Computer & Information Systems graduate (Ain Shams University, Honours, GPA 3.16/4.0) working as a **Junior Embedded Systems & IoT Engineer** at **Skärpt**, where I design and ship ESP32 firmware and the tooling around it.

I work across the stack, from bare-metal AVR firmware and RTOS tasks, to ESP32 products deployed in the field, to custom Yocto Linux images and the backend APIs that connect hardware to the cloud. I also do hands-on hardware repair: PCB fault diagnosis, SMD rework, and BGA reballing.

---

## Currently

**Junior Embedded Systems & IoT Engineer @ Skärpt** (Jun 2026 – present)

Building a line of ESP32-based IoT products. Recent work includes:

- **Cold Chain HUB:** temperature-monitoring hub integrated with Teltonika FMC130 telematics, including a 1-Wire (DS18B20-compatible) sensor emulator on the ESP32-C6 with BLE advertising
- **RS485 / Modbus sensor nodes:** MQTT gateways with SD-card store-and-forward and an NPK soil-sensor bridge over Modbus RTU
- **IR AC controller:** IR timing fixes, WiFi repeater (AP+STA with NAT), and MQTT authentication
- **Zigbee coordinator** on the ESP32-C6 for door sensors via IAS Zone
- **Provisioning tooling:** Python/Tkinter configurators that write NVS settings over serial for repeatable fleet deployments
- **Field work:** flashing, field testing, protocol sniffing, and branded datasheets and wiring documentation

*Product code is proprietary, so it isn't published here.*

---

## Tech Stack

| Domain | Tools & Technologies |
|---|---|
| **Languages** | C, C++, Python, C#, Java, SQL |
| **Embedded & Hardware** | ESP32 / ESP32-C6, ESP8266, AVR ATmega (16/32), Arduino, SIM7000C, NEO-6M GPS, ENC28J60, Si446x, DHT11/22, PIR |
| **Firmware Frameworks** | ESP-IDF, Arduino, PlatformIO (incl. hybrid ESP-IDF builds), FreeRTOS (tasks, queues, semaphores), NVS |
| **Protocols** | MQTT, Modbus RTU, RS-485/RS-232, BLE, Zigbee, 1-Wire, UART, I2C, SPI, AT Commands, TCP/IP, HTTP, REST |
| **Libraries** | PubSubClient, espMqttClient, ModbusMaster, IRremoteESP8266 |
| **Linux** | Yocto Project, Embedded Linux, systemd |
| **Hardware Skills** | PCB Fault Diagnosis, SMD Soldering, BGA Reballing, Schematic Reading, Logic/SPI Sniffing, Multimeter Debugging |
| **Tooling** | Python / Tkinter desktop tools, serial provisioning, binary patching |
| **Backend** | Spring Boot, Flask, REST APIs, JWT, MySQL, PostgreSQL, MongoDB, SQLite, Firebase |
| **AI / ML** | TensorFlow, Keras, Scikit-learn, OpenCV, MNE, EEG Signal Processing |
| **DevOps** | Docker, Kubernetes, Jenkins CI/CD, Git |

---

## Featured Projects

### [Real-Time GPS Vehicle Tracking System](https://github.com/ibrahimmohamedkmal/AIN-Tracking-System-GPS-Based-Real-Time-Vehicle-Tracking)
> ESP32 · C++ · SIM7000C · Flask · React · PostgreSQL · Docker

Graduation project. A full-stack vehicle tracking platform with geofencing, speed alerts, and live GPS updates. An ESP32 + SIM7000C transmits over cellular to a Flask backend; containerized with Docker, orchestrated on Kubernetes, deployed via Jenkins CI/CD.

---

### Custom Embedded Linux Image — Yocto
> Yocto Project · BitBake · C · systemd · Linux

A Poky-based custom image with a BitBake meta-layer and a C socket client auto-started via a systemd service. Demonstrates BSP customization and rootfs configuration.

---

### [Smart Home Monitoring System](https://github.com/ibrahimmohamedkmal/Smart-Home-Monitoring-System)
> C++ · AVR ATmega · Arduino Uno · Bare-Metal Firmware

Bare-metal AVR firmware for PIR, smoke, and temperature sensing. An Arduino Uno hosts an HTTP server for real-time Wi-Fi LED control, with register-level peripheral drivers and no Arduino HAL.

---

### [Image Classification — Bag of Visual Words & CNN](https://github.com/ibrahimmohamedkmal/Image-Classification-Bag-of-Visual-Words-and-CNN)
> Python · OpenCV · TensorFlow

Image classification comparing a classical Bag of Visual Words pipeline against a CNN.

---

### [Motor Imagery BCI Photo Viewer](https://github.com/ibrahimmohamedkmal/Motor-Imagery-BCI-Photo-Viewer)
> Python · MNE · Scikit-learn · EEG · CSP · SVM

An EEG-based brain-computer interface classifying left/right hand motor imagery using Common Spatial Patterns (CSP) + SVM and Random Forest, with MNE for signal processing.

---

### [Cryptography & Security Package](https://github.com/ibrahimmohamedkmal/Security-Package)
> C# · .NET Framework

8+ classical and modern cryptographic algorithms (RC4, MD5, RSA, ElGamal, Diffie-Hellman) with encrypt, decrypt, and cryptanalysis modes in a unified desktop UI.

---

## Experience

- **Junior Embedded Systems & IoT Engineer @ Skärpt** (Jun 2026 – present): ESP32 firmware, IoT hubs and gateways, and provisioning tooling for field deployments (see above).
- **Backend Engineering Intern @ Fuinco:** Built a fleet management REST API (Spring Boot, MySQL, MongoDB) with JWT auth, vehicle/driver modules, and real-time location tracking.
- **Hardware Repair & Diagnostics Trainee** (Jul 2024 – Jan 2025): Diagnosed laptop motherboard faults from schematics; performed BGA reballing of CPUs, GPUs, and PCH chips using hot-air rework stations.

---

<p align="center">
  <i>Open to embedded systems, firmware, and IoT engineering roles in Egypt and remotely.</i>
</p>
