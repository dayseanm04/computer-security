# DNS Poisoning Attack Simulation (Hosts File)

## Overview
This lab demonstrates how DNS poisoning can be performed locally by modifying the Windows hosts file. The lab shows how domain name resolution can be manipulated to redirect users to a different IP address without changing any external DNS servers.

The project was completed in a **Windows Sandbox environment** to safely simulate a real-world attack scenario.

---

## Objectives

- Simulate a DNS poisoning attack using the hosts file
- Redirect a legitimate domain to a different IP address
- Restore the system to its original state

---

## Lab Breakdown

### 1. Setup
- Launched Windows Sandbox
- Installed Notepad++
- Identified IP addresses using ping and online tools

### 2. Attack
- Modified the hosts file with administrative privileges
- Mapped a legitimate domain to a different IP address
- Flushed DNS cache
- Observed domain redirection

### 3. Cleanup
- Removed the malicious hosts file entry
- Flushed DNS cache again









