# DVWA Security Testing — Write-up

## Objective
Perform manual and automated web application security testing on DVWA (Damn Vulnerable Web Application) across Low, Medium, and High difficulty levels, covering key OWASP Top 10 vulnerability categories.

## Environment
- **Attacker Machine:** Kali Linux
- **Target:** DVWA (Damn Vulnerable Web Application)
- **Proxy Tool:** Burp Suite

## 1. SQL Injection
- Tested login and search forms across all difficulty levels to identify SQL Injection points.
- Used Burp Suite to intercept and modify HTTP requests, bypassing client-side input validation.
- Extracted database information by manipulating query parameters at Low and Medium levels; analyzed filtering mechanisms at the High level.

## 2. Cross-Site Scripting (XSS)
- Tested Reflected, Stored, and DOM-based XSS across all difficulty levels.
- Injected payloads to test input sanitization and identify insecure server-side handling.
- Documented which filters could be bypassed at each difficulty setting.

## 3. Command Injection
- Tested input fields for OS command injection vulnerabilities.
- Chained commands using shell operators to execute arbitrary system commands where input validation was weak.

## 4. Brute Force
- Attempted brute-force login attacks against the DVWA authentication form.
- Analyzed rate-limiting and lockout mechanisms across difficulty levels.

## 5. Defensive Validation
- Deployed **SafeLine WAF** as a countermeasure in front of the DVWA instance.
- Re-tested all above attack vectors to validate that OWASP Top 10 blocking rules correctly mitigated the identified vulnerabilities.

## Result
Successfully identified and exploited SQL Injection, XSS, Command Injection, and Brute-Force vulnerabilities across DVWA's difficulty levels, then validated defensive mitigation using a WAF.

## Tools Used
DVWA, Burp Suite, SafeLine WAF, Kali Linux

---
*Performed in a personal, isolated lab environment for educational purposes.*
