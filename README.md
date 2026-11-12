# networkwalks-B084-week2-Cybersecurity-Lab-Setup


# Week 2: Footprinting, Reconnaissance & Network Scanning Labs

This repository documents my practical hands-on experience completing **Week 2 Project Modules (W2-PM1 to W2-PM5)** in Cybersecurity & Ethical Hacking. Through these labs, I simulated real-world passive and active reconnaissance workflows to build target profiles, discover exposed assets, and map live network topologies.

## 🛠️ Practical Experience & Executed Modules

### 1. Multi-Tool CLI Reconnaissance (`W2-PM1`)
Performed comprehensive target profiling on a live domain using built-in Kali Linux reconnaissance utilities:
* **Domain & DNS Enumeration:** Executed `whois`, `nslookup`, and `dnsrecon` to extract registrar records, name servers, mail servers (MX), SPF policies, and cPanel SRV records.
* **Web Stack & Header Fingerprinting:** Used `whatweb` and `curl -I` to identify underlying CMS versions, web servers, caching mechanisms, and exposed REST API endpoints.
* **Firewall Detection:** Deployed `wafw00f` to detect the presence of Web Application Firewalls (ModSecurity).

### 2. Google Hacking Database / GHDB (`W2-PM2`)
Conducted zero-touch passive reconnaissance using advanced Google search operators:
* Sourced verified dorks from Exploit-DB's GHDB to identify exposed internet-connected cameras and misconfigured open web directories (`intitle:index.of`).
* Verified live endpoints and documented security misconfigurations to understand how public data leaks expand an organization's attack surface.

### 3. Visual Link Analysis with Maltego (`W2-PM3`)
* Installed, configured, and authenticated Maltego Graph on Windows.
* Executed domain-to-email OSINT transforms to visually map relationships and harvest organizational email addresses.

### 4. Automated OSINT Harvesting (`W2-PM4`)
* Operated `theHarvester` in Kali Linux to query public search engines (Baidu) and aggregated data sources (`-b all`).
* Extracted subdomains, virtual hosts, and public email addresses while managing result limits and source queries.

### 5. Network Discovery & Topology Mapping with Zenmap (`W2-PM5`)
* Identified local IP configurations and LAN subnet boundaries via CLI (`ipconfig`).
* Executed Nmap Ping Scans (`nmap -sn`) via Zenmap GUI to enumerate all live hosts on the local network.
* Extracted host IP addresses, MAC addresses, and vendor details, and exported the complete visual network topology map in PDF format.

---

## 📁 Repository Contents
* `/Screenshots` — Execution proofs, terminal outputs, Maltego graphs, and Zenmap scan results.
* `/Reports` — Exported text outputs and Zenmap PDF network topology maps.

## 🧰 Tools & Technologies Used
* **OS:** Kali Linux, Windows
* **CLI Recon:** `whois`, `whatweb`, `nslookup`, `curl`, `wafw00f`, `dnsrecon`, `theHarvester`
* **GUI & OSINT:** Maltego, Zenmap (Nmap), Google Hacking Database (GHDB)
