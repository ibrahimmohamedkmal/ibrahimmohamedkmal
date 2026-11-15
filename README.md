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

- **Cold Chain HUB:** temperature-monitoring hub integrated with Teltonika FMC130 telematics, including a 1-Wire (DS18B20-compatible) sensor emulator on the ESP32 with BLE advertising
- **RS485 / Modbus sensor nodes:** MQTT gateways with SD-card store-and-forward and an NPK soil-sensor and sn-3002-gzws-n01 bridge over Modbus RTU
- **IR AC controller:** IR timing fixes, WiFi repeater (AP+STA with NAT), and MQTT authentication
- **Zigbee coordinator** on the ESP32-C6 for door sensors via IAS Zone
- **Provisioning tooling:** Python/Tkinter configurators that write NVS settings over serial for repeatable fleet deployments
- **Field work:** flashing, field testing, protocol sniffing, and branded datasheets and wiring documentation

*Product source code is proprietary, so it isn't published here. The Skärpt repositories below are documentation-only: architecture, behavior, configuration and wiring.*

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

## Skärpt Product Documentation

Design and behavior write-ups for the ESP32 products I work on at Skärpt. These repositories are **documentation only**; firmware source, configurator source and binaries are not published.

### [Cold Chain HUB (SK-V-094)](https://github.com/ibrahimmohamedkmal/Skarpt-Cold-Chain)
> ESP32 · 1-Wire · BLE · DHT22 · Teltonika FMC130

A THS202-compatible 1-Wire temperature and humidity hub for cold-storage monitoring. To an existing 1-Wire master it looks exactly like a THS202 sensor, so the Teltonika FMC130 needs no changes. The same readings are broadcast over BLE every 100 ms. Also covers door monitoring, a local audible alarm, a relay mirror and a health-validation output with dual watchdogs. Includes the datasheet and FMC130 wiring diagram.

---

### [RS485 Environmental Sensor Node](https://github.com/ibrahimmohamedkmal/Skarpt-rs485-sensor-node)
> ESP32 · RS485 · Modbus RTU · Modbus TCP · MQTT · SD Store-and-Forward · Python/Tkinter

Polls a Modbus RTU sensor (temperature, humidity, illuminance) and delivers readings over independent paths: MQTT with application-level ACK, a TCP client (Modbus TCP or JSON), and two raw RS485 gateways (RTU-over-TCP and RTU-over-MQTT). A bus-arbitration scheme gives gateway requests priority over polling, and undelivered readings are queued on SD with at-least-once delivery. A Windows configurator writes NVS settings over USB and preserves other namespaces so the message-id counter is never reset.

---

### [Wi-Fi Sensor Node (V2.18)](https://github.com/ibrahimmohamedkmal/Skarpt-wifisensor)
> ESP32 · DHT22 · SSD1306 OLED · TP4056 + 18650 · MQTT · SD Queue · Python/Tkinter

Measures temperature, humidity and battery state, shows them on an OLED and publishes to MQTT. Features include a hand-written bit-banged DHT22 driver, on-device calibration, a battery-percentage model with smoothing and deadband, SD store-and-forward with a persistent drain cursor, a low-battery mode, a non-blocking buzzer alarm, and watchdog/heap-monitor stability checks. Configurable over serial, MQTT or a desktop Config Writer.

---

### [ESP32 IR AC Controller](https://github.com/ibrahimmohamedkmal/Skarpt-IR-AC-Controller)
> ESP32 · ESP-IDF + Arduino · PlatformIO · MQTT · IRremoteESP8266 · MIT

An MQTT-driven infrared air-conditioner controller with about 70 built-in AC protocols or learned raw codes from any remote. Supports dual MQTT brokers, an AP+STA Wi-Fi repeater with NAT, state restore after power loss, and no-reflash configuration via a desktop GUI or remotely over MQTT. Documents the reliability design (watchdogs, heap monitor, back-off retries, protected IR timing window) and known limitations.

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
