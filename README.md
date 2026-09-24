<div align="center">

# 🔐 Cybersecurity Labs

### Hands-on penetration testing, vulnerability assessment & security documentation

![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP_Top_10-000000?style=for-the-badge&logo=owasp&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PortSwigger](https://img.shields.io/badge/PortSwigger_Academy-FF6633?style=for-the-badge&logo=portswigger&logoColor=white)
![Status](https://img.shields.io/badge/status-actively_building-success?style=for-the-badge)

</div>

---

## 📋 Table of Contents

- [About](#-about)
- [Labs](#-labs)
- [Methodology](#-methodology)
- [Tools & Techniques](#️-tools--techniques)
- [Roadmap](#-roadmap)
- [Ongoing Training](#-ongoing-training)
- [About Me](#-about-me)

---

## 👋 About

Hands-on cybersecurity practice covering network security, vulnerability assessment, penetration testing, and web application security — built alongside my M.Sc. Global Software Development studies at Hochschule Fulda.

I treat this repo as a working lab notebook, not a trophy case: every entry documents what I actually tested, what I found, why it mattered, and how I'd fix it. All testing here is performed against deliberately vulnerable applications or my own systems in authorized, controlled environments.

---

## 📁 Labs

### 🕸️ [01 — Web Application Pentesting](./01-web-application-pentesting)

Reconnaissance and vulnerability assessment against a deliberately vulnerable web application, in an authorized, controlled environment.

**What was tested:**
- Authentication & authorization weaknesses
- IDOR (Insecure Direct Object Reference)
- Session management and file-security issues
- Cryptographic failures in password storage
- Findings mapped against the **OWASP Top 10**

**Tools used:** Kali Linux · Burp Suite · OWASP ZAP · Gobuster · WPScan · Nikto

Each finding is documented with impact, root cause, and remediation steps — not just a list of what was run.

---

## 🧭 Methodology

My approach to every lab in this repo:

1. **Scope** — define what's being tested and what's explicitly out of bounds
2. **Recon** — enumerate the attack surface before touching anything
3. **Test** — attempt exploitation methodically, one hypothesis at a time
4. **Document** — record evidence as I go, not reconstructed afterward
5. **Remediate** — every finding gets a fix recommendation, not just a "vulnerable" label

I care more about being able to explain *why* something is a vulnerability and *how* I'd fix it than about collecting tool output.

---

## 🛠️ Tools & Techniques

| Category | Tools |
|---|---|
| Web App Security | Burp Suite, OWASP ZAP, Gobuster, WPScan, Nikto |
| Network Security | Nmap, Wireshark, Metasploit |
| Platform | Kali Linux |
| Scripting | Python, Bash |
| Cloud Security | AWS CLI *(in progress)* |

---

## 🗺️ Roadmap

What's actively being built and added to this repo next:

- [ ] **Network Security Lab** — Nmap/Wireshark/Metasploit writeups against a home lab environment
- [ ] **SIEM/SOC Mini-Lab** — Splunk or Security Onion, detection rules, and a SOC-analyst-style incident writeup
- [ ] **AWS Cloud Security** — flaws.cloud walkthrough covering S3 misconfigurations and IAM privilege escalation
- [ ] **TryHackMe/HackTheBox Writeups** — structured methodology breakdowns, not just "room completed"
- [ ] **GRC Documentation** — ISO 27001-style risk register and NIS2 applicability analysis

This list is intentionally public — it's my actual build plan, and I'd rather show honest progress than a repo that looks finished when it isn't.

---

## 📚 Ongoing Training

Currently working through the **[PortSwigger Web Security Academy](https://portswigger.net/web-security)** — completed labs and techniques applied are reflected in the Web Application Pentesting folder above as they're finished.

---

## 🎓 About Me

M.Sc. Global Software Development student at Hochschule Fulda, focused on cybersecurity, vulnerability management, and secure software development.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/venkat-bhavan-tati-261032184)

</div>

</div>
