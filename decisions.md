# Technical Decisions

## Automation over Manual Testing

The system was designed to automate repetitive penetration testing tasks in order to:

- Save time
- Reduce human error
- Provide consistent results

---

## SQL Injection and XSS Focus

Initial development focused on SQL Injection and XSS because:

- They are among the most common web vulnerabilities
- They provide a strong baseline for testing system effectiveness
- They are easy to validate in controlled environments

---

## Dual Scanning Approach (Nmap + TCP Fallback)

The system supports:

- Nmap scanning for full-featured environments
- TCP fallback scanning for systems without Nmap

This ensures flexibility and wider usability.

---

## AI-Assisted Detection

AI-based pattern recognition was introduced to:

- Improve detection accuracy beyond simple string matching
- Handle less obvious or obfuscated responses
- Provide more intelligent classification of vulnerabilities

---

## SQLite for Data Storage

SQLite was selected because:

- It is lightweight and easy to integrate
- No external database setup is required
- Suitable for local and small-scale deployments

---

## Streamlit for Interface

Streamlit was used to:

- Quickly build an interactive web interface
- Simplify user interaction
- Display real-time results with minimal setup

---

## Known Limitations

- Focused on basic vulnerabilities (SQLi, XSS)
- Does not cover advanced attack vectors yet
- Requires proper authorization before scanning real systems

These limitations were accepted to maintain simplicity and clarity of the system.
