<div align="center">

# Adrian Bork

**Offensive security · Munich, Germany**

*I break web applications to understand how they're built — and write up every technique in my own words.*

<br>

[![TryHackMe](https://img.shields.io/badge/TryHackMe-Top%208%25-88CC14?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/chillyka)
[![League](https://img.shields.io/badge/League-Silver-C0C0C0?style=for-the-badge)](https://tryhackme.com/p/chillyka)
[![Rooms](https://img.shields.io/badge/Rooms-71-1F8FFF?style=for-the-badge)](https://tryhackme.com/p/chillyka)
[![eJPT](https://img.shields.io/badge/eJPT-Q4%202026-FF6B00?style=for-the-badge)](#roadmap)

</div>

<br>

> **If I can't explain *why* an attack lands without naming a tool, I don't consider it learned.**

Working toward the **eJPT** and **OSCP** while training as an IT Systems Integration specialist (FISI, IHK). Linux since my early twenties, first server and OPNsense firewall at 26, nine years in the trades — then all-in on security in December 2025.

---

## 🎯 What I work on

<div align="center">

**Injection**

![SQL Injection](https://img.shields.io/badge/SQL_Injection-C0392B?style=flat-square)
![NoSQL](https://img.shields.io/badge/NoSQL-C0392B?style=flat-square)
![LDAP](https://img.shields.io/badge/LDAP-C0392B?style=flat-square)
![ORM](https://img.shields.io/badge/ORM-C0392B?style=flat-square)
![SSTI](https://img.shields.io/badge/SSTI-C0392B?style=flat-square)
![XXE](https://img.shields.io/badge/XXE-C0392B?style=flat-square)
![Command Injection](https://img.shields.io/badge/Command_Injection-C0392B?style=flat-square)

**Authentication & session**

![JWT](https://img.shields.io/badge/JWT-1F6FEB?style=flat-square)
![OAuth](https://img.shields.io/badge/OAuth-1F6FEB?style=flat-square)
![MFA Bypass](https://img.shields.io/badge/MFA_Bypass-1F6FEB?style=flat-square)
![Session Management](https://img.shields.io/badge/Session_Management-1F6FEB?style=flat-square)
![Auth Bypass](https://img.shields.io/badge/Auth_Bypass-1F6FEB?style=flat-square)

**Access control & logic**

![IDOR](https://img.shields.io/badge/IDOR-8250DF?style=flat-square)
![SSRF](https://img.shields.io/badge/SSRF-8250DF?style=flat-square)
![XSS](https://img.shields.io/badge/XSS-8250DF?style=flat-square)
![File Inclusion](https://img.shields.io/badge/File_Inclusion-8250DF?style=flat-square)
![Race Conditions](https://img.shields.io/badge/Race_Conditions-8250DF?style=flat-square)
![Mass Assignment](https://img.shields.io/badge/Mass_Assignment-8250DF?style=flat-square)

**Tooling**

![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white)
![nmap](https://img.shields.io/badge/nmap-4682B4?style=flat-square)
![sqlmap](https://img.shields.io/badge/sqlmap-4682B4?style=flat-square)
![gobuster](https://img.shields.io/badge/gobuster-4682B4?style=flat-square)
![hashcat](https://img.shields.io/badge/hashcat-4682B4?style=flat-square)
![John](https://img.shields.io/badge/John_the_Ripper-4682B4?style=flat-square)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=flat-square&logo=metasploit&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

<br>

**Next up** — Linux & Windows privilege escalation → Active Directory

</div>

---

## 🧠 How I think about a target

The list above is what I've touched. This is what I actually carry between them:

| Attack | The assumption it breaks |
|:---|:---|
| **SSTI** | The server *evaluates* my input instead of displaying it |
| **LDAP Injection** | I can close the filter and inject my own condition |
| **ORM Injection** | The developer reached past the ORM into raw SQL |
| **NoSQL Injection** | I can turn a value into an operator |
| **XXE** | The parser will fetch whatever I point it at |
| **JWT** | The server trusts a token it should be verifying |
| **IDOR** | The object reference is accepted, not authorised |

They're all the same question wearing different syntax: **does the server trust a value I control?**

---

## 📦 Repositories

<table>
<tr><td width="34%">

### [`pentest-writeups`](https://github.com/chillyka0x1/pentest-writeups)

Attack techniques explained in my own words — the mechanism and the mistakes, not the answers.

</td><td width="33%">

### [`periscan`](https://github.com/chillyka0x1/periscan)

Exposure scanner in Python. Shows what's *actually* reachable from outside — built it to verify my segmentation instead of trusting it.

</td><td width="33%">

### [`homelab-infrastructure`](https://github.com/chillyka0x1/homelab-infrastructure)

Proxmox lab: 22+ services, OPNsense segmentation, monitoring. Targets I'm allowed to break.

</td></tr>
</table>

---

## 🔬 How I learn

<details>
<summary><b>The loop — click to expand</b></summary>

<br>

Every technique goes through the same four steps:

1. **Solve it** — hands-on, no walkthrough if I can avoid it
2. **Explain it from memory** — closed notes. Recognition isn't recall.
3. **Write down what I got wrong** — the misconception is the part that sticks
4. **Revisit on a schedule** — spaced repetition, because knowledge decays

Every writeup follows that shape: *when it applies · why it works · how to test it · what it looks like · how to fix it · what I got wrong.*

The last section is the one I'd read first.

</details>

<details>
<summary><b>Why infrastructure matters for offence</b></summary>

<br>

I ran systems before I attacked them. That order helps: you reason about attack surface differently once you've had to keep something alive, patch it, and watch it fall over at 2am.

The lab is where that meets offence — segmented networks, deliberately broken services, and a scanner I wrote to check whether my own assumptions hold.

</details>

---

## 🗺️ Roadmap

<div align="center">

| Milestone | Target |
|:---|:---:|
| **eJPT** | `Q4 2026` |
| **HackTheBox** — OSCP preparation | `2027` |
| **OSCP** | `2028` |
| **FISI** — IT Systems Integration, IHK | `in training until Q4 2027` |

</div>

Long-term: penetration testing, remote.

---

<div align="center">

📫 **borkadrian@proton.me**

<sub>Learning in public. Everything here is my own work — anything borrowed is credited.<br>
All testing on authorised targets only: my own lab, TryHackMe, HackTheBox, and intentionally vulnerable applications.</sub>

</div>
