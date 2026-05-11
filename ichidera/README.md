# ichidera — CMS 418 Contribution

**Contributor:** Ichidera  
**Project:** Wireless Emergency Telemedicine System (WETS) — 2013 UI Recreation  
**Course:** CMS 418 — Netcentric Computing, Rivers State University  
**Lecturer:** Dr. Chima Igiri

---

## My Assignment

**Screen: Home Patient Monitoring — Vital Signs Dashboard** (Figure 15)

This is the main doctor-facing monitoring screen. It shows:

- **Top navigation bar** — Vital signs, Raw Data, Patient's Notes, Medical Record, Personal Information, Sessions, Home
- **Action bar** — Add consultation, Add Drug prescription, Show personal info., Add new patient, Patient Search
- **Patient info panel** — Patient MRN, Monitoring start date, Current state; with a doctor greeting showing summary counts (monitored patients, emergency events, notifications)
- **Vital Signs Monitoring panel:**
  - ECG waveform display
  - Pulse (bpm) with heart icon
  - Blood Pressure — DIA / SYS (mmHg)
  - Temperature (°C) with thermometer graphic
  - SpO2 (%)
- **Bottom controls** — Load, Save, Pause, Stop, UDP, Connect

---

## Folder Structure

```
ichidera/
├── README.md     ← this file
├── index.html    ← Home Patient Monitoring screen
└── style.css     ← stylesheet
```

---

## Approach

Modern 2026 HTML + CSS interpretation of the 2013 original — same layout intent and information hierarchy, cleaner typography, CSS custom properties, and accessible markup. No frameworks, no JavaScript (static UI only).


---

## Reference

All screenshots of the original 2013 WETS system are in [`../Task/`](../Task/).  
See the project-wide [`../README.md`](../README.md) for the full system overview.
