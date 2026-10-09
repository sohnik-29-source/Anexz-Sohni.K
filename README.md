# 🛡️ SecureCorp – Cybersecurity Assessment Capstone

## 📌 Project Overview

The **SecureCorp Cybersecurity Assessment Capstone** is a hands-on cybersecurity project designed to identify vulnerabilities, perform security testing, monitor security logs, and recommend solutions to improve system security.

The assessment was performed in a controlled training laboratory using Ubuntu WSL, Metasploitable2, DVWA, Nmap, and Wazuh Cloud.

## 🎯 Objectives

* Identify open ports and running services using Nmap.
* Perform web application vulnerability testing using DVWA.
* Understand common cybersecurity attacks and their impacts.
* Monitor security-related logs using Wazuh.
* Assess security risks and recommend mitigation strategies.
* Understand the CIA Triad: Confidentiality, Integrity, and Availability.

## 🧰 Tools and Technologies

| Tool            | Purpose                                   |
| --------------- | ----------------------------------------- |
| Ubuntu WSL      | Attacker and analysis environment         |
| Metasploitable2 | Intentionally vulnerable target system    |
| DVWA            | Web application security testing          |
| Nmap            | Network scanning and service discovery    |
| Wazuh Cloud     | Security log monitoring                   |
| GitHub          | Project documentation and version control |

## 🧪 Vulnerabilities Tested

1. **Brute Force** – Testing login protection.
2. **SQL Injection** – Testing database input validation.
3. **Cross-Site Scripting (XSS)** – Testing input filtering and output encoding.
4. **Command Injection** – Testing unsafe system command execution.
5. **File Inclusion** – Testing unauthorized local file access.
6. **File Upload** – Reviewing file upload security.
7. **FTP and SSH Security** – Assessing authentication risks.

*All security testing was intended for the controlled training lab.*

## 🔍 Methodology

1. **Build:** Set up the cybersecurity lab.
2. **Discover:** Identify open ports and running services using Nmap.
3. **Attack:** Test selected vulnerabilities in DVWA.
4. **Log:** Collect available security logs.
5. **Detect:** Review monitoring information in Wazuh.
6. **Investigate:** Analyze available evidence.
7. **Assess:** Evaluate risks and potential impacts.
8. **Remediate:** Recommend security improvements.
9. **Report:** Document findings and recommendations.

## 📊 Key Findings

* Multiple legacy network services were exposed on the target.
* SQL Injection could expose database information.
* XSS could allow untrusted scripts to execute.
* Command Injection could enable unauthorized command execution.
* File Inclusion could expose local system files.
* Weak authentication protection could increase brute-force risks.
* Target-side Wazuh monitoring requires further verification.

## 🔐 Security Recommendations

* Use parameterized SQL queries.
* Validate user inputs and encode outputs.
* Avoid executing system commands directly from user input.
* Restrict access to sensitive files.
* Implement strong passwords, rate limiting, and multi-factor authentication.
* Disable unnecessary services and restrict inbound ports.
* Replace insecure FTP with SFTP where possible.
* Patch outdated software.
* Configure and verify target-side security monitoring.
* Maintain regular backups and review security alerts.

## 🏗️ Lab Architecture

**Ubuntu WSL → Metasploitable2 / DVWA → Security Testing → Wazuh Cloud Monitoring**

Note: The Wazuh agent was confirmed active on Ubuntu WSL. Target-side monitoring was not confirmed by the available evidence.

## 📁 Project Structure

```text
SecureCorp-Cybersecurity/
│
├── README.md
├── SecureCorp_Final_Submission_Report.docx
└── screenshots/
    ├── nmap-scan.png
    ├── dvwa-testing.png
    └── wazuh-monitoring.png
```

*Add the screenshots folder and image files only if you have the corresponding evidence.*

## ⚠️ Disclaimer

This project was conducted for educational purposes in an authorized, controlled cybersecurity training environment. Do not perform security testing against systems without explicit permission.

## 👩‍💻 Author

**Sohni Koppula**

Cybersecurity Assessment Capstone

---

⭐ This project demonstrates practical learning in network reconnaissance, web application security testing, vulnerability assessment, security monitoring, and remediation planning.
