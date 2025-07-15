# Useful Resources for TryHackMe & Cybersecurity Learning

Below is a curated list of tools and websites commonly used in penetration testing, red teaming, and cybersecurity research. These platforms will assist me throughout my TryHackMe (THM) journey and beyond.

---

## Search Engines & Reconnaissance

### [Shodan](https://www.shodan.io)
A powerful search engine for discovering devices connected to the internet. It indexes data such as IPs, open ports, banners, services, and more.

**Use Cases:**
- Identify exposed services (e.g., FTP, RDP, Elasticsearch)
- Enumerate ICS/SCADA systems
- Discover vulnerable IoT devices

---

### [Censys](https://search.censys.io)
A search engine for internet-connected hosts, domains, certificates, and other assets. Similar to Shodan but with a research-oriented API and datasets.

**Use Cases:**
- Passive reconnaissance of IP ranges or certificates
- Monitor attack surfaces
- Correlate certificates and subdomains

---

## Malware Analysis & File Scanning

### [VirusTotal](https://www.virustotal.com)
Allows scanning of files and URLs using multiple antivirus engines. You can also submit hashes (MD5, SHA1, SHA256) to look up existing scan reports.

**Use Cases:**
- Check if a file is malicious
- Analyze payloads and binaries from THM labs
- Scan scripts, executables, and payloads

---

## Vulnerability & Exploit Databases

### [CVE.ORG](https://www.cve.org)
The official Common Vulnerabilities and Exposures (CVE) database. Offers information on publicly disclosed security vulnerabilities and exposures.

**Use Cases:**
- Look up known vulnerabilities by ID (e.g., CVE-2024-XYZ)
- Understand attack vectors and severity scores (CVSS)

---

### [Exploit Database](https://www.exploit-db.com)
A curated archive of publicly available exploits and proof-of-concepts (PoCs) for various software vulnerabilities.

**Use Cases:**
- Search for working exploits for vulnerable services
- Download PoC code for testing in lab environments
- Analyze how a vulnerability is exploited

---

## Developer & Offensive Security Tools

### [GitHub](https://github.com)
While GitHub is primarily a code hosting platform, it's widely used for publishing CVE PoCs, red-team tools, scripts, payloads, and frameworks.

**Use Cases:**
- Search for repositories tagged with a CVE ID or vulnerability name
- Download & fork pentesting tools like `AutoRecon`, `dirsearch`, `impacket`, etc.
- Explore C2 frameworks, enumeration scripts, and password crackers
