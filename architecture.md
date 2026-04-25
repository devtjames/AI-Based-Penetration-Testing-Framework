# System Architecture

## Overview

The AI-Based Penetration Testing Framework is designed as a modular scanning system that automates vulnerability detection and reporting for web applications.

---

## Core Components

### 1. Input Layer

- Accepts target URL or domain
- Validates and normalizes input
- Resolves hostname and IP address

---

### 2. Scanning Engine

- Uses Nmap for network and service scanning (if available)
- Falls back to TCP socket scanning when Nmap is not available
- Identifies open ports and exposed services

---

### 3. Vulnerability Testing Layer

- Injects SQL Injection payloads into URL parameters
- Injects XSS payloads into input fields
- Performs HTTP header analysis
- Detects exposed sensitive files (.env, .git, etc.)

---

### 4. Analysis Layer

- Uses string matching to detect known vulnerability patterns
- Applies AI-assisted pattern recognition for improved detection
- Classifies results based on response behavior

---

### 5. Reporting Layer

- Displays results in real-time via Streamlit interface
- Stores scan results in SQLite database
- Generates downloadable reports (CSV, PDF)

---

## Data Flow

1. User inputs target URL  
2. System validates and prepares target  
3. Scanning engine analyzes services and endpoints  
4. Payloads are injected into the target  
5. Responses are analyzed for vulnerabilities  
6. Results are classified and displayed  
7. Reports are stored for future reference  

---

## Security Considerations

- Intended for authorized testing environments only
- Includes warnings for safe usage
- Prevents misuse through controlled input and user guidance
