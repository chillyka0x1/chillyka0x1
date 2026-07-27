<div align="center">

# Adrian Bork

### Offensive security · Munich, Germany

*I break web applications to understand how they're built —*
*and write up every technique in my own words.*

<br>

[![TryHackMe](https://img.shields.io/badge/TryHackMe-chillyka%20·%20Top%208%25%20·%20Silver%20·%2071%20rooms-88CC14?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/chillyka)

</div>

<br>

> **If I can't explain *why* an attack lands without naming a tool, I don't consider it learned.**

Working toward the **eJPT** and **OSCP** while training as an IT Systems Integration specialist (FISI, IHK). Linux since my early twenties, first server and OPNsense firewall at 26, nine years in the trades — then all-in on security in December 2025.

<br>

---

## 🧠 How I think about a target

Every one of these is the same question in different syntax: **does the server trust a value I control?**

<br>

| | Attack | The assumption it breaks |
|:--|:---|:---|
| 💉 | **SSTI** | The server *evaluates* my input instead of displaying it |
| 💉 | **SQL / NoSQL Injection** | My input becomes part of the query instead of staying data |
| 💉 | **LDAP Injection** | I can close the filter and inject my own condition |
| 💉 | **ORM Injection** | The developer reached past the ORM into raw SQL |
| 📄 | **XXE** | The parser will fetch whatever I point it at |
| 🔑 | **JWT** | The server trusts a token it should be verifying |
| 🔑 | **OAuth · MFA · Sessions** | The second factor and the session are enforced client-side |
| 🚪 | **IDOR · Mass Assignment** | The reference is accepted, not authorised |
| 🌐 | **SSRF · File Inclusion** | The server fetches on my behalf |
| ⏱️ | **Race Conditions** | There's a gap between check and use |

<br>

**Next up** — Linux & Windows privilege escalation → Active Directory

<br>

---

## 🛠️ Tooling

<div align="center">

![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=for-the-badge&logo=metasploit&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Kali](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=for-the-badge&logo=proxmox&logoColor=white)

<sub>also — nmap · sqlmap · gobuster · ffuf · hashcat · John the Ripper · OPNsense</sub>

</div>

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
<summary><b>Why infrastructure matters for offence</b></summary>

<br>

I ran systems before I attacked them. That order helps — you reason about attack surface differently once you've had to keep something alive, patch it, and watch it fall over at 2am.

The lab is where that meets offence: segmented networks, deliberately broken services, and a scanner I wrote to check whether my own assumptions actually hold.

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
| **FISI** — IT Systems Integration, IHK | `in training until Q4 2027` |

</div>

<br>

Long-term: penetration testing, remote.

<br>

<div align="center">

📫 **borkadrian@proton.me**

<sub>Learning in public. Everything here is my own work — anything borrowed is credited.<br>
All testing on authorised targets only: my own lab, TryHackMe, HackTheBox, and intentionally vulnerable applications.</sub>

</div>
