# 📡 Nmap Notes for Security+ and Network+

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![Repo Size](https://img.shields.io/github/repo-size/sheniaks/nmap-notes)
![Last Commit](https://img.shields.io/github/last-commit/sheniaks/nmap-notes)

> Practical Nmap examples for cybersecurity learners prepping for **CompTIA Security+**, **Network+**, or entering **penetration testing** and **network security**.

---

## 🧭 Table of Contents

- [🔍 Scan Types Comparison](./nmap_scan_types.md)
- [🧪 Example Usage](#example-usage)
- [🛡️ Security+ Relevance](#security-relevance)
- [🚀 Learning Roadmap](#learning-roadmap)
- [👤 Author & Contact](#author--contact)

---

## 🔍 Scan Types Comparison

📄 View full table in [`nmap_scan_types.md`](./nmap_scan_types.md)

Side-by-side breakdown of `-sS`, `-sT`, and `-sU` scans, privileges, speed, and use cases.

---

## 🧪 Example Usage

Basic TCP and UDP combo scan:

```bash
sudo nmap -sS -sU -p T:22,80,U:53,161 192.168.0.103
```

Other useful examples:

```bash
nmap --script vuln 192.168.0.103
nmap -A --reason 192.168.0.103
```

---

## 🛡️ Security+ Relevance

These scans align with the following SY0-701 exam objectives:

- **4.2**: Vulnerability scanning
- **4.3**: Monitoring tools and enumeration
- **5.5**: Penetration testing and security assessments

---

## 🚀 Learning Roadmap

**✅ Current focus:**

- TCP/UDP scanning basics
- Aggressive scans with `-A`
- NSE scripting with `--script vuln`

**📌 Coming soon:**

- Output formats (`-oN`, `-oG`, `-oX`)
- Scan evasion techniques
- Subnet scanning (`/24`, `/16`)
- Automating Nmap with Python (`python-nmap`)

---

## 👤 Author & Contact

**Oleksandr Sheniak**  
Cybersecurity Student | Penetration Testing Enthusiast  
🔗 [GitHub](https://github.com/sheniaks)  
🔗 [LinkedIn](https://ca.linkedin.com/in/sheniaks)

---

> ☕️ If this helped you, please ⭐ star the repo and share it with other learners!
