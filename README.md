# Cybersecurity Labs

Hands-on offensive security lab write-ups covering VulnHub Boot2Root machines and DVWA web application testing — built and documented end-to-end in a personal lab environment.

**Author:** Prem Chauhan  
**Focus areas:** Penetration Testing · Web Application Security · Vulnerability Assessment

---

## About this repository

Each folder below is a self-contained project with its own detailed write-up: reconnaissance steps, exploitation chain, exact commands used, and the final result. These are hands-on engagements performed in a personal lab environment.

## Projects

| # | Project | What it demonstrates | Tools / Stack |
|---|---------|----------------------|----------------|
| 1 | [Nullbyte Pentest](./projects/nullbyte-pentest) | VulnHub Boot2Root machine — reconnaissance, steganography-based clue, web exploitation, privilege escalation via SUID/cron misconfigurations | Nmap, Kali Linux |
| 2 | [DVWA Security Testing](./projects/dvwa-security-testing) | Web application vulnerability testing across Low, Medium, High difficulty — SQL Injection, XSS, Command Injection, Brute Force | DVWA, Burp Suite, Kali Linux |

## Skills demonstrated across these labs

- **Reconnaissance & Enumeration:** Nmap, service/port scanning
- **Exploitation:** SQL Injection, XSS, Command Injection, Brute-Force attacks, steganography
- **Privilege Escalation:** SUID binary abuse, cron job misconfiguration
- **Web App Security:** Manual and automated testing with Burp Suite, OWASP Top 10 coverage
- **Defensive Security:** WAF deployment (SafeLine), OWASP Top 10 mitigation validation

---

*All labs were performed in isolated, self-hosted virtual lab environments for educational and skill-building purposes.*
