# Project Synapse

[![Status](https://img.shields.io/badge/status-active-brightgreen.svg)](#)
[![Platform](https://img.shields.io/badge/platform-ESP32%20%7C%20ESP8266%20%7C%20Android%20%7C%20iOS-lightgrey.svg)](#)

# 🧠 Project Synapse

> A distributed, privacy‑focused cyber security platform built on low‑cost **ESP‑based** devices. Each node operates as a headless *Agent*, remotely controlled by a mobile *Commander App*. Together, they form a flexible and cooperative system for wireless network analysis and privacy defense — fully interoperable across both **ESP8266** and **ESP32** hardware.

---

## 🚀 Overview

Project Synapse introduces a scalable architecture where multiple low‑cost microcontroller boards work together to analyze, test, and protect wireless networks in a controlled and ethical manner.

* **Commander:** A mobile control application managing all Agents remotely.
* **Agents:** Headless devices (ESP8266 / ESP32) that execute assigned network operations autonomously.
* **Control Network:** A secure Wi‑Fi network established by the Commander to coordinate communications.

Agents connect, receive REST‑based commands, temporarily switch into test mode, execute their tasks (e.g., Wi‑Fi scans or simulations), and then reconnect to report results.

---

## ⚙️ Core Features

* 🛰️ **Distributed Operation:** Multiple Agents performing tasks simultaneously under one Commander.
* 🔐 **Privacy Defense Tools:** Network activity simulations to test resilience against passive tracking or metadata collection.
* 🌐 **REST API Control:** Simple command‑based communication for easy mobile or desktop integration.
* 💤 **Power Efficiency:** Headless design with deep sleep support for extended field use.
* ⚡ **Interoperability:** Seamless collaboration between ESP8266 and ESP32 devices — no hardware modification required.
* 🧩 **Scalability:** Easily expand the system with new Agents for larger operations or experiments.

---

## 🧭 Concept in Action

### Control Flow Summary

1. **Commander App** creates a protected Wi‑Fi network.
2. **Agents** connect and register themselves.
3. **Commander** sends REST commands for tasks (e.g., scanning or simulation).
4. **Agents** temporarily switch to analysis mode, perform the task, and store results.
5. **Agents** reconnect to report results and await new commands.

This architecture ensures high stability and avoids radio conflicts common in dual‑mode setups.

---

## 🔐 Example Use Case — Privacy Protection

Large retail centers often use Wi‑Fi probe request tracking to analyze visitor behavior. Project Synapse can conceptually generate controlled “noise” to test and evaluate such systems, ensuring they cannot easily correlate user identities.

By simulating randomized probe activity, Synapse demonstrates how network privacy defenses can protect users against passive location tracking.

---

## 🧩 Advanced Concept Modes (Planned)

> **Note:** The following modes are for controlled research, simulation, or laboratory testing only. They are not active in the public firmware.

* **Deauthentication Simulation** – Testing network resilience by simulating temporary disconnect waves.
* **Beacon & Probe Flood Simulation** – Generating randomized SSID broadcast traffic for privacy stress‑tests.
* **Snooping / Passive Capture** – Capturing and analyzing nearby signals for research purposes.

All modes are disabled by default and require explicit activation in test environments with authorization.

---

## 🎬 Concept Videos / Illustrative Clips

> **Important:** The videos/images referenced here are **illustrative concept clips** (icons/placeholders). They **do not** represent a finished or publicly deployable system — they are planned examples showing how features could behave in a controlled test setup. Use of disruptive modes is subject to legal and ethical restrictions as described above.

E
### 1) Distributed Deauthentication 

**Summary:** An illustrative clip showing the Commander issuing simultaneous deauthentication commands to three Agents, each targeting a different Wi‑Fi network. Demonstrates parallel task distribution and synchronized execution.

<!-- VIDEO/ICON 1 -->

[![Concept 1 Thumbnail](videos/concept1_thumbnail.png)](videos/concept1.mp4)

### 2) Cooperative Power Scaling 

**Summary:** Concept clip showing cooperative load‑sharing — initially one Agent fails to affect a strong network, but after coordination, multiple Agents jointly complete the task. Illustrates teamwork and adaptive response.

<!-- VIDEO/ICON 2 -->

[![Concept 2 Thumbnail](videos/concept2_thumbnail.png)](videos/concept2.mp4)

### 3) Concurrent Sensing & Reporting 

**Summary:** Illustrative clip showing multiple Agents simultaneously monitoring multiple networks and relaying telemetry to the Commander. Demonstrates the intended multi‑channel sensing design.

<!-- VIDEO/ICON 3 -->

[![Concept 3 Thumbnail](videos/concept3_thumbnail.png)](videos/concept3.mp4)

### 4) Heterogeneous ESP Interoperability 

**Summary:** Placeholder clip showing ESP8266 and ESP32 devices exchanging data and coordinating tasks — proving cross‑generation compatibility purely via software.

<!-- VIDEO/ICON 4 -->

[![Concept 4 Thumbnail](videos/concept4_thumbnail.png)](videos/concept4.mp4)

---

## ⚖️ Legal, Ethical & Safety Notes

* All test and simulation modes are **disabled by default**.
* Any active testing must be done **in isolated lab environments** with **explicit authorization**.
* The project aims to promote education, research, and responsible experimentation — **never disruption**.

---

## 📜 License

MIT License — for educational and ethical research use only.
