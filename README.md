📡 Nmap Notes for Security+ and Network+



Practical Nmap examples for cybersecurity learners prepping for CompTIA Security+, Network+, or entering penetration testing and network security.

🧭 Table of Contents
🔍 Scan Types Comparison

🧪 Example Usage

🛡️ Security+ Relevance

🚀 Learning Roadmap

👤 Author & Contact

🔍 Scan Types Comparison
📄 View full table in nmap_scan_types.md

Side-by-side breakdown of -sS, -sT, and -sU scans with privileges, stealth, and usage context.

🧪 Example Usage
TCP + UDP combo scan:

nginx
Copy
Edit
sudo nmap -sS -sU -p T:22,80,U:53,161 192.168.0.103
Aggressive scan with reasons:

css
Copy
Edit
sudo nmap -A --reason 192.168.0.103
Run vulnerability scripts:

nginx
Copy
Edit
sudo nmap --script vuln 192.168.0.103
🛡️ Security+ Relevance
These scans align with the following Security+ SY0-701 exam domains:

4.2: Vulnerability management

4.3: Monitoring and enumeration tools

5.5: Penetration testing activities

🚀 Learning Roadmap
✅ Current:
TCP/UDP scanning fundamentals

Aggressive scans with -A

Vulnerability scanning via NSE (--script vuln)

📌 Coming Soon:
Output formats (-oN, -oG, -oX)

CIDR subnet scanning (192.168.1.0/24)

Scan evasion (--data-length, --decoy)

Automating Nmap with Python (python-nmap)

👤 Author & Contact
Oleksandr Sheniak
Cybersecurity Student | Penetration Testing Enthusiast

🔗 GitHub
🔗 LinkedIn
