# Embedded-Project_Smart-Vault-Door-Lock
Smart Vault Door Lock Dual factor authentication (PIN+RFID) with GSM SMS alerts. Custom PCB design using EasyEDA, ATmega328P microcontroller, secure solenoid lock. Complete embedded C firmware developed and programmed on Ubuntu using avrdude. 
##  Overview

This project presents a **high-security vault door lock system** implementing **dual-factor authentication** – requiring both a **6-digit alphanumeric PIN** (something you know) and an **authorized RFID card** (something you have) before granting access.

The system is built around an **ATmega328P microcontroller** with a **custom-designed PCB** and integrates:
- 4x4 Matrix Keypad (via I²C)
- MFRC522 RFID Reader (via SPI)
- 16x2 LCD with I²C backpack
- SIM900A GSM module for SMS alerts
- Solenoid lock actuator (fail-secure)
- LED + Buzzer feedback system
- Exit button & reset functionality

**Key security feature:** After 3 failed attempts (PIN or RFID), the system triggers a **GSM SMS alert** to authorized personnel and enters a lockout state.

---

##  Development Environment

| Tool | Purpose |
|------|---------|
| **Operating System** | Ubuntu 22.04 / 24.04 LTS |
| **Compiler** | avr-gcc (AVR-GCC toolchain) |
| **Flashing Tool** | avrdude |
| **PCB Design** | EasyEDA (browser-based) |
