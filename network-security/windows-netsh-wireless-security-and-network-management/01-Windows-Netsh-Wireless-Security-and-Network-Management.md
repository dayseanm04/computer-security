# Windows Netsh Wireless Security and Network Management

## Overview
In this lab, I will demonstrate how to use Windows netsh commands to view and manage wireless network settings. This includes checking wireless drivers, viewing available networks, managing saved profiles, and blocking specific networks.

This lab shows how command-line tools can be used to control wireless network behavior and improve security.

---

## Objective

- Use netsh to manage wireless networks
- View wireless adapter and driver information
- Display available networks and saved profiles
- Connect and disconnect from networks
- Block and unblock specific wireless networks


---

## Lab Environment

| Component | Details |
|---|---|
| Operating System | Windows 10/11 |
| Tool | Windows PowerShell (Admin) |
| Network | Wireless LAN |

Note: Your device must have a wireless network interface card

---

### Step 1: Open PowerShell as Administrator

1. Search for **PowerShell** and click **Run as Administrator**
3. Click **Yes** if prompted.

<img width="874" height="495" alt="1" src="https://github.com/user-attachments/assets/6a6d0a5b-4e10-4b14-a556-d2e3a0a543b9" />
<img width="786" height="265" alt="2" src="https://github.com/user-attachments/assets/0e2b21f5-49f3-4dc2-affa-c3e7a34a5fb7" />

### Step 2: Start Netsh

1. In PowerShell, type: **netsh** and press **Enter**

<img width="805" height="195" alt="3" src="https://github.com/user-attachments/assets/6cf61f5c-829b-4703-8572-05e19e8bda14" />

2. Type **wlan** and press **Enter**

<img width="765" height="226" alt="4" src="https://github.com/user-attachments/assets/682ca784-3f6f-42d4-88a4-e711d8c5d882" />

---

### Step 3: View Wireless Driver Information

Run **show drivers**

<img width="974" height="571" alt="5" src="https://github.com/user-attachments/assets/5bf5068d-d6e1-47c9-98bd-b903948b8ee3" />

This displays:
- Wireless adapter name
- Driver version
- Supported radio types
- Authentication and encryption support






























