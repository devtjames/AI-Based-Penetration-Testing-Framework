# AI-Based Penetration Testing Framework

## Overview

This project is an automated penetration testing framework designed to scan web applications for common security vulnerabilities such as SQL Injection (SQLi) and Cross-Site Scripting (XSS).

The system allows users to input a target URL and automatically performs vulnerability testing by injecting predefined payloads and analyzing server responses. It combines rule-based detection with AI-assisted pattern recognition to improve accuracy and reduce manual effort.

The goal of the system is to provide a simple, fast, and accessible way to identify security weaknesses in web applications.

---

## Problem Statement (Optional)

Manual penetration testing is often:

- Time-consuming
- Repetitive
- Dependent on tester experience
- Inconsistent across different environments

Many small teams and students lack access to advanced security tools.

This project addresses these issues by automating vulnerability detection and simplifying the testing process through a web-based interface.

---

## Core / Key Features

- Automated SQL Injection detection
- Automated Cross-Site Scripting (XSS) detection
- URL-based vulnerability scanning
- Payload injection and response analysis
- AI-assisted pattern recognition for detection
- Real-time scan results
- Vulnerability classification (Vulnerable / Secure)
- Scan history and report storage
- CSV and PDF report export

---

## Screenshots

Screenshots included in this repository demonstrate:

- LANDING PAGE
<img width="1366" height="768" alt="HOME" src="https://github.com/user-attachments/assets/5df7929a-914d-4fa8-a6d3-b6a7ad9d0bb2" />


- DASHBOARD - URL input interface
<img width="1366" height="768" alt="DASHBOARD" src="https://github.com/user-attachments/assets/8591a510-b4a0-4152-adad-fdcf1e3d961a" />


- RAW OUPUT - Scan execution process
<img width="1366" height="768" alt="RAW OUTPUT" src="https://github.com/user-attachments/assets/97d1b1ef-4f00-459b-9312-c7cf9dfc67e8" />


- ENDPOINT - Real-time vulnerability results
<img width="1366" height="768" alt="ENDPOINT" src="https://github.com/user-attachments/assets/f1589dc6-9c29-4f85-b714-824bf33ba83f" />


- VULNERABILITY - Report generation and export
<img width="1366" height="768" alt="VULNERABILITY" src="https://github.com/user-attachments/assets/56cc8927-3f8b-4c10-8f9f-695ed258dd2d" />



---

## Tech Stack

- **Backend:** Python  
- **Framework:** Streamlit  
- **Database:** SQLite  
- **Networking:** requests, socket  
- **Security Tools:** Nmap (optional), TCP fallback scanning  
- **Data Processing:** pandas, regex  
- **Reporting:** CSV, PDF (fpdf)  
- **Version Control:** Git and GitHub  

---

## My Role

I handled the full development of the system, including:

- System architecture and design
- Vulnerability scanning logic (SQLi, XSS)
- Payload injection and response analysis
- AI-assisted detection logic
- Report generation and data storage
- UI development using Streamlit
- Testing using vulnerable environments (DVWA, testphp)

---

## System Architecture

The system follows a modular architecture with automated scanning and analysis:

- Input layer for target URL submission
- Scanning engine (Nmap or TCP fallback)
- Vulnerability testing layer (SQLi, XSS, header checks)
- AI-assisted response analysis
- Reporting and storage layer

A detailed breakdown is available in the `architecture.md` file.

---

## Development Notes

- The system is designed for educational and authorized security testing only.
- It supports both automated and fallback scanning modes.
- Detection currently focuses on common vulnerabilities (SQLi, XSS).
- The system is extendable to include more advanced security checks.

---

## Contact

If you would like to discuss this project or review the implementation, feel free to reach out.
