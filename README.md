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

<table>
<tr>
<td valign="top" width="50%">

**Injection**

`SQL Injection` — second-order, WAF bypass, OOB, header injection
`NoSQL` · `LDAP` · `ORM` · `SSTI` · `XXE` · `Command Injection`

</td>
<td valign="top" width="50%">

**Authentication & session**

`JWT` · `OAuth` · `MFA bypass`
`Session Management` · `Authentication Bypass`

</td>
</tr>
<tr>
<td valign="top">

**Access control & logic**

`IDOR` · `SSRF` · `XSS` · `File Inclusion`
`Race Conditions` · `Mass Assignment`

</td>
<td valign="top">

**Recon & tooling**

`nmap` · `Burp Suite` · `gobuster` · `sqlmap`
`hashcat` · `John` · `Wireshark` · `Metasploit`

</td>
</tr>
</table>

**Next up:** Linux & Windows privilege escalation → Active Directory

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
