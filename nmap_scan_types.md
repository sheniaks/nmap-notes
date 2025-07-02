# 🔍 Nmap Scan Types: SYN, Connect, and UDP Comparison

A quick reference for common Nmap scans used in cybersecurity, penetration testing, and Security+/Network+ certification prep.

---

## ⚙️ Comparison Table

| Scan Type | Nmap Flag | Protocol | Privileges Required | Connection Type     | Speed  | Stealthiness | Use Case                                                |
|-----------|-----------|----------|----------------------|----------------------|--------|--------------|----------------------------------------------------------|
| SYN Scan  | `-sS`     | TCP      | Root/Admin only      | Half-open (stealth) | Fast   | High         | Preferred scan in pen testing; fast and less detectable |
| Connect   | `-sT`     | TCP      | None (no sudo)       | Full 3-way handshake | Medium | Low          | Used when `-sS` isn’t possible (e.g., no root access)    |
| UDP Scan  | `-sU`     | UDP      | Root/Admin preferred | Connectionless       | Slow   | Medium       | Identifying services like DNS, SNMP, DHCP               |

---

## 🧪 Example Combo Scan

```bash
sudo nmap -sS -sU -p T:22,80,U:53,161 192.168.0.103
