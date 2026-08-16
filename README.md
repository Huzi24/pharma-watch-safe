# VigiTrack 🛡️

**A pharmacovigilance and drug safety monitoring platform for tracking adverse drug reactions, checking drug interactions, and detecting emerging safety signals.**

Live demo: [pharma-watch-safe.base44.app](https://pharma-watch-safe.base44.app)

---

## 📋 Overview

VigiTrack is a web-based pharmacovigilance tool designed to help healthcare professionals log, monitor, and analyze Adverse Drug Reactions (ADRs). It combines structured ADR reporting with automated drug interaction checking and statistical signal detection to surface potential safety concerns before they become critical.

---

## ✨ Features

### 📊 Dashboard
A centralized overview of pharmacovigilance activity, giving users a quick snapshot of reporting trends and system status.

### 📝 Log ADR
A guided, multi-step form for submitting structured adverse drug reaction reports:
1. **Patient Information** — age, gender, weight
2. **Suspected Drug** — drug name, dose, frequency, route of administration
3. **Reaction Details** — reaction type, severity, and clinical description

### 📁 Reports
A searchable, filterable log of all ADR reports on record. Each entry includes:
- Drug name, dosage, and route
- Reaction type and severity
- Clinical narrative (e.g. "GI bleeding with melena")
- Filter by severity and free-text search across drug, reaction, or patient

### 🔄 Drug Interaction Checker
Checks two drugs against an internal reference library of clinically significant interactions (28+ pairs and growing). Users enter **Drug A** and **Drug B** and receive an instant interaction flag.

### 🔔 Signal Alerts
Automated safety signal detection: when a drug accumulates **3 or more reports of the same reaction type**, VigiTrack raises a signal. Each signal displays:
- Total reports
- Serious and severe/fatal event counts
- Severity mix breakdown (severe / moderate)
- Linked related report IDs for traceability

Example signals detected:
- **Warfarin → Bleeding** (3 reports, 2 severe)
- **Fluoxetine → Serotonin Syndrome**

---

## 🧠 How It Works

1. Clinicians or pharmacists log ADRs through the structured reporting form.
2. Each report is stored with drug, dosage, reaction, and severity metadata.
3. The **Interaction Checker** cross-references reported drug combinations against a curated reference set.
4. The **Signal Engine** continuously scans reports and automatically flags drugs that cross the 3-report threshold for the same reaction — a standard pharmacovigilance signal detection heuristic.

---

## 🛠️ Tech Stack

- Built and deployed on [Base44](https://base44.com)
- Frontend: React-based UI with a responsive, mobile-friendly design
- Real-time data sync between reporting, interaction checking, and signal modules

---

## 🎯 Use Cases

- Pharmacy students and clinicians practicing structured ADR documentation
- Rapid prototyping of pharmacovigilance workflows
- Educational tool for understanding signal detection in drug safety monitoring
- Portfolio project demonstrating healthcare-focused product design

---

## 📄 License

This project is available for demonstration and educational purposes.

---

## 🙋 Author

Built by **Huzi24** — combining a Pharm.D background with AI-assisted rapid app development.
https://github.com/Huzi24/pharma-watch-safe/blob/main/.gitignore

