# 📡 Nmap Notes for Security+ and Network+

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![Repo Size](https://img.shields.io/github/repo-size/sheniaks/nmap-notes)
![Last Commit](https://img.shields.io/github/last-commit/sheniaks/nmap-notes)

> Practical Nmap examples for cybersecurity learners prepping for **CompTIA Security+**, **Network+**, or entering **penetration testing** and **network security**.

---

## 🧭 Table of Contents

- [🔍 Scan Types Comparison](#-scan-types-comparison)
- [🧪 Example Usage](#-example-usage)
- [🛡️ Security+ Relevance](#️-security-relevance)
- [🚀 Learning Roadmap](#-learning-roadmap)
- [👤 Author & Contact](#-author--contact)

---

## 🔍 Scan Types Comparison

📄 [View full table here](./nmap_scan_types.md)

A side-by-side breakdown of `-sS`, `-sT`, and `-sU` scans, privileges, speed, and usage in the field.

---

## 🧪 Example Usage

```bash
sudo nmap -sS -sU -p T:22,80,U:53,161 192.168.0.103
