# VirusTotal File and URL Analysis Lab Part 1

A hands-on cybersecurity lab demonstrating how to use **VirusTotal** to analyze files and URLs for malware and other threats, an important skill in general or for threat analysis and detection.

---

## Objective

- Perform file analysis using VirusTotal
- Analyze URL
- Interpret multi-engine antivirus scan results
- Evaluate the effectiveness and limitations of public malware scanning platforms
- Understand how threat intelligence tools are used by defenders, and potentially abused by attackers

---


## Tools Used

| Tool | Purpose |
|------|---------|
| [**`VirusTotal`**](https://www.virustotal.com) | File and URL threat analysis |
| Web Browser | Accessing the VirusTotal platform |
| Microsoft Word | file creation for test upload |

---

##  Lab Guides

| Section | Description |
|---------|-------------|
| [**VirusTotal File Analysis**](./VirusTotal-File-Analysis/Malware-Detection-Using-VirusTotal.md) | Upload and analyze a file across multiple AV engines |
| [**VirusTotal URL Analysis**](./VirusTotal-URL-Analysis/URL-Analysis-with-VirusTotal.md) | Submit and analyze a URL for malicious indicators |
| [**Reflection Questions**](./01-Reflection-Questions.md) | Reflection Questions for the lab |


## Security Implications

### How VirusTotal Benefits Users:
- Provides fast verification of suspicious files and URLs
- Aggregates 60+ antivirus engines for broader detection coverage
- Helps validate endpoint alerts

### How It Benefits Security Researchers:
- Enables malware trend analysis
- Assists in hash-based threat intelligence
- Supports investigation of suspicious artifacts

### Potential for Abuse:
Attackers may use public malware scanning platforms to test their malware before distribution to ensure it avoids detection.

### Defensive Countermeasures:
- Isolated testing environments such as secure sandboxes
