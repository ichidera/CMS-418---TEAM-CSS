# CMS 418 — TEAM CSS

**Course:** CMS 418 — Netcentric Computing
**Lecturer:** Dr. Chima Igiri  
**Institution:** Rivers State University  
**Team:** CSS

---

## Task Description

Recreate the UI of the **Wireless Emergency Telemedicine System (WETS)** — a 2013 desktop/web application developed at the EE Department, Faculty of Engineering, Assiut University. The original system was designed to monitor and transmit patient vital signs wirelessly to remote doctors.

Reference screenshots of the original 2013 system are in the [`Task/`](./Task/) folder.

---

## System Overview

The original WETS had the following key screens/components:

| Screen | Description |
|---|---|
| **Login / Authentication** | User login page with username, password, and new user registration |
| **Main Interface** | Navigation dashboard with New Patient, Find Patient, Patient Connection, Medication |
| **Add New Patient** | Patient registration form — personal info, address, doctor assignment, photo import |
| **Search / Find Patient** | Search patients by name or ID; displays results in a table |
| **Vital Signs Monitor** | Real-time display of ECG waveform, Temperature, Heart Rate, SpO2, Blood Pressure, Respiration |

### System Architecture (Figure 1)

The telemedicine system consists of four main tiers:

```
Patient's Side  →  Data Communication Networks  →  Medical Server  →  Management Unit
```

- **Patient's Side:** Biosignal sensors → Processing unit → Communication unit
- **Networks:** Cellular network (GPRS) and Internet (TCP/IP)
- **Doctors** access data via HTTP (desktop) or GPRS (mobile)

### Hardware Components

- **Temperature sensor** — with calibration circuit and 100x amplifier gain
- **SpO2/HR sensor** — pulse oximeter for oxygen saturation and heart rate
- **MCU (PIC18f458)** — connected to: vital signs acquisition circuit, GSM/GPRS module, Ethernet module, LCD/keypad module, Flash memory

### Mobile-Care Unit Workflow

```
Start → Request to send? → [Yes] → process
                         → [No]  → Manual operation? → Sensors init →
                                   Vital signs processing →
                                   Patient status normal? → [Yes] → Internet → Send raw data
                                                          → [No]  → GPRS → Send raw data → Alarm
```

---

## Repository Structure

Each team member implements their assigned screen(s) in their own folder:

```
CMS 418 - TEAM CSS/
├── README.md          ← this file
├── Task/              ← reference screenshots of the original 2013 system
└── ichidera/          ← Ichidera's implementation
```

> Other team members should add their folders here as they work on their assigned screens.

---

## Tech Stack

Plain **HTML & CSS** — no frameworks, matching the CMS 418 (Netcentric Computing) focus on UI design and layout.

