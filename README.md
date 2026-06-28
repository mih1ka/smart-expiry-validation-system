# Automated Barcode-Based Expiry Validation and Product Sorting

> **Patent Published** (Application No. **202541093730**)

An Arduino-Python based intelligent inventory management system that automates **barcode scanning, expiry validation, and physical product sorting** to reduce inventory waste and improve consumer safety.

---

## Overview

Manual inspection of product expiry dates is time-consuming, error-prone, and inefficient for large inventories. This project automates the entire workflow by integrating **embedded hardware**, **cloud-based data validation**, and **real-time mechanical sorting**.

The system scans a product barcode, retrieves its expiry information from a cloud-hosted database, determines whether the product is expired, and automatically diverts it into the appropriate category using servo motors.

---

## Features

* Barcode-based product identification
* Arduino Uno controlled embedded system
* Cloud-hosted expiry database lookup
* Python backend for real-time expiry validation
* Serial communication between Arduino and Python
* Automatic servo-based product sorting
* Low-cost and scalable inventory automation
* Patent Published (Application No. **202541093730**)

---

## Tech Stack

### Hardware

* Arduino Uno R3
* GROW-GM805-L Barcode Scanner
* MG996R Servo Motors (2×)
* Breadboard
* Jumper Wires

### Software

* Python
* Arduino IDE
* Pandas
* PySerial
* Datetime

---

## System Architecture

```text
                 Barcode Scanner
                        │
                        ▼
                 Arduino Uno R3
                        │
            USB Serial Communication
                        │
                        ▼
                 Python Backend
                        │
       Cloud-hosted Product Database
                        │
            Expiry Date Validation
                        │
        EXPIRED / NOT_EXPIRED Response
                        │
                        ▼
                 Arduino Uno R3
                        │
                        ▼
                 Servo Motor Control
                        │
                        ▼
             Product Sorted Automatically
```

---

## Workflow

1. Scan the product barcode.
2. Arduino receives the Product ID.
3. Product ID is sent to the Python backend via serial communication.
4. Python retrieves the product's expiry date from the cloud-hosted database.
5. The current date is compared with the expiry date.
6. Python sends the validation result back to the Arduino.
7. Arduino actuates the appropriate servo motor.
8. The product is automatically sorted into:

   * Valid Products
   * Expired Products

---

## Project Structure

```text
Barcode-Expiry-Sorting-System/
│
├── Arduino/
│   └── barcode_sorting.ino
│
├── Python/
│   ├── expiry_validation.py
│   └── requirements.txt
│
├── Dataset/
│   └── products.csv
│
├── Images/
│
└── README.md
```

---

## Hardware Setup

### System Prototype
The hardware prototype integrates an Arduino Uno R3, a GROW-GM805-L barcode scanner, and two MG996R servo motors to perform real-time barcode scanning, expiry validation, and automated product sorting.
### Working Demo

The system scans a product barcode, validates its expiry date through a Python backend using a cloud-hosted database, and automatically diverts the product to the appropriate category using servo motors.

---

## Applications

* Smart Retail Stores
* Supermarkets
* Warehouses
* Inventory Management
* Pharmacies
* Smart Pantry Systems
* Food Safety Monitoring

---

## Future Improvements

* ESP32 Wi-Fi integration
* Mobile application for monitoring
* SQL/Firebase backend
* Conveyor belt automation
* AI-based inventory analytics
* Computer vision-based barcode detection
* Dashboard for expiry statistics

---

## Patent

**Patent Published**

**Application Number:** 202541093730

**Title:**
*Automated Expiry-Based Sorting System Using Barcode Scanning and Arduino*

---

## Author

**Mihika Manish**

---

