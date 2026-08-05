<div align="center">

# Adrian Bork

### Offensive security · Munich, Germany

*I break web applications to understand how they're built — and write up every technique in my own words.*

<br>

[![TryHackMe](https://img.shields.io/badge/TryHackMe-Top_7%25-88CC14?style=flat-square&logo=tryhackme&logoColor=white&labelColor=2B2B2B)](https://tryhackme.com/p/chillyka)
[![League](https://img.shields.io/badge/League-Gold-FFD700?style=flat-square&labelColor=2B2B2B)](https://tryhackme.com/p/chillyka)
[![Rooms](https://img.shields.io/badge/Rooms-77-1F8FFF?style=flat-square&labelColor=2B2B2B)](https://tryhackme.com/p/chillyka)
[![eJPT](https://img.shields.io/badge/eJPT-Q4_2026-FF6B00?style=flat-square&labelColor=2B2B2B)](#roadmap)
[![FISI](https://img.shields.io/badge/FISI-until_Q4_2027-8250DF?style=flat-square&labelColor=2B2B2B)](#roadmap)

</div>

<br>

> **If I can't explain *why* an attack lands without naming a tool, I don't consider it learned.**

<br>

---

## 🎯 What I work on

<div align="center">

**Injection**

![SQL Injection](https://img.shields.io/badge/-SQL_Injection-C0392B?style=flat&labelColor=C0392B)
![NoSQL](https://img.shields.io/badge/-NoSQL-C0392B?style=flat&labelColor=C0392B)
![LDAP](https://img.shields.io/badge/-LDAP-C0392B?style=flat&labelColor=C0392B)
![ORM](https://img.shields.io/badge/-ORM-C0392B?style=flat&labelColor=C0392B)
![SSTI](https://img.shields.io/badge/-SSTI-C0392B?style=flat&labelColor=C0392B)
![XXE](https://img.shields.io/badge/-XXE-C0392B?style=flat&labelColor=C0392B)
![Command Injection](https://img.shields.io/badge/-Command_Injection-C0392B?style=flat&labelColor=C0392B)

**Authentication & session**

![JWT](https://img.shields.io/badge/-JWT-1F6FEB?style=flat&labelColor=1F6FEB)
![OAuth](https://img.shields.io/badge/-OAuth-1F6FEB?style=flat&labelColor=1F6FEB)
![MFA Bypass](https://img.shields.io/badge/-MFA_Bypass-1F6FEB?style=flat&labelColor=1F6FEB)
![Session Management](https://img.shields.io/badge/-Session_Management-1F6FEB?style=flat&labelColor=1F6FEB)
![Auth Bypass](https://img.shields.io/badge/-Auth_Bypass-1F6FEB?style=flat&labelColor=1F6FEB)

**Access control & logic**

![IDOR](https://img.shields.io/badge/-IDOR-8250DF?style=flat&labelColor=8250DF)
![SSRF](https://img.shields.io/badge/-SSRF-8250DF?style=flat&labelColor=8250DF)
![XSS](https://img.shields.io/badge/-XSS-8250DF?style=flat&labelColor=8250DF)
![File Inclusion](https://img.shields.io/badge/-File_Inclusion-8250DF?style=flat&labelColor=8250DF)
![Race Conditions](https://img.shields.io/badge/-Race_Conditions-8250DF?style=flat&labelColor=8250DF)
![Mass Assignment](https://img.shields.io/badge/-Mass_Assignment-8250DF?style=flat&labelColor=8250DF)

**Tooling**

![Burp Suite](https://img.shields.io/badge/Burp-Suite-FF6633?style=flat&logo=burpsuite&logoColor=white&labelColor=2B2B2B)
![nmap](https://img.shields.io/badge/-nmap-4682B4?style=flat&labelColor=2B2B2B)
![sqlmap](https://img.shields.io/badge/-sqlmap-4682B4?style=flat&labelColor=2B2B2B)
![gobuster](https://img.shields.io/badge/-gobuster-4682B4?style=flat&labelColor=2B2B2B)
![ffuf](https://img.shields.io/badge/-ffuf-4682B4?style=flat&labelColor=2B2B2B)
![hashcat](https://img.shields.io/badge/-hashcat-4682B4?style=flat&logo=hashcat&logoColor=white&labelColor=2B2B2B)
![John the Ripper](https://img.shields.io/badge/-John_the_Ripper-4682B4?style=flat&labelColor=2B2B2B)
![Wireshark](https://img.shields.io/badge/-Wireshark-1679A7?style=flat&logo=wireshark&logoColor=white&labelColor=2B2B2B)
![Metasploit](https://img.shields.io/badge/-Metasploit-2596CD?style=flat&logo=metasploit&logoColor=white&labelColor=2B2B2B)
![Kali](https://img.shields.io/badge/-Kali_Linux-557C94?style=flat&logo=kalilinux&logoColor=white&labelColor=2B2B2B)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white&labelColor=2B2B2B)

<br>

**Next up** — Linux & Windows privilege escalation → Active Directory

</div>

<br>

---

## 🧠 The pattern underneath

Every one of those is the same question in different syntax: **does the server trust a value I control?**

| Attack | The assumption it breaks |
|:---|:---|
| **SSTI** | The server *evaluates* my input instead of displaying it |
| **SQL / NoSQL** | My input becomes part of the query instead of staying data |
| **LDAP** | I can close the filter and inject my own condition |
| **ORM** | The developer reached past the ORM into raw SQL |
| **XXE** | The parser will fetch whatever I point it at |
| **JWT** | The server trusts a token it should be verifying |
| **IDOR** | The reference is accepted, not authorised |

<br>

---

## 📦 Repositories

<table>
<tr>
<td width="34%" valign="top">

### [`pentest-writeups`](https://github.com/chillyka0x1/pentest-writeups)

Attack techniques in my own words — the mechanism and the mistakes, not the answers.

Plus the checklist I work through **before** opening a walkthrough.

</td>
<td width="33%" valign="top">

### [`periscan`](https://github.com/chillyka0x1/periscan)

Exposure scanner in Python.

Shows what's *actually* reachable from outside. On its first run it found an accidentally exposed Proxmox — which is why it exists.

</td>
<td width="33%" valign="top">

### [`homelab-infrastructure`](https://github.com/chillyka0x1/homelab-infrastructure)

Proxmox lab: 22+ services, OPNsense segmentation, monitoring.

Targets I'm allowed to break.

</td>
</tr>
</table>

<br>

---

## 🔬 How I learn

<details>
<summary><b>The loop</b></summary>

<br>

1. **Solve it** — hands-on, no walkthrough if I can avoid it
2. **Explain it from memory** — closed notes. Recognition isn't recall.
3. **Write down what I got wrong** — the misconception is the part that sticks
4. **Revisit on a schedule** — spaced repetition, because knowledge decays

Every writeup follows that shape: *when it applies · why it works · how to test it · what it looks like · how to fix it · what I got wrong.*

The last section is the one I'd read first.

</details>

<details>
<summary><b>Background</b></summary>

<br>

Linux since my early twenties, first server and OPNsense firewall at 26, nine years in the trades — then all-in on security in December 2025. Currently training as an IT Systems Integration specialist (FISI, IHK).

I ran systems before I attacked them. That order helps: you reason about attack surface differently once you've had to keep something alive, patch it, and watch it fall over at 2am.

</details>

<br>

---

## 🗺️ Roadmap

<div align="center">

| Milestone | Target |
|:---|:---:|
| **eJPT** | `Q4 2026` |
| **HackTheBox** — OSCP preparation | `2027` |
| **OSCP** | `2028` |
| **FISI** — IT Systems Integration, IHK | `until Q4 2027` |

</div>

<br>

<div align="center">

📫 **borkadrian@proton.me**

<sub>Learning in public. Everything here is my own work — anything borrowed is credited.<br>
All testing on authorised targets only: my own lab, TryHackMe, HackTheBox, and intentionally vulnerable applications.</sub>

</div>
