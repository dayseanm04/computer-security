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

---

### Step 4: View Wireless Interfaces

Run: **show interfaces**

<img width="810" height="522" alt="6" src="https://github.com/user-attachments/assets/f17b7dcc-31c8-42a7-9d5b-e19f20af809e" />

This displays:
- Interface name
- SSID (connected network)
- Authentication type
- Connection status

---

### Step 5: View Wireless Settings

Run: **show settings**

<img width="887" height="302" alt="7" src="https://github.com/user-attachments/assets/ff3db8b4-5aa4-486b-8c27-2f758da0c3ef" />

This shows global wireless settings.

---

### Step 6: View Available Networks

Run: **show networks**

<img width="985" height="681" alt="8" src="https://github.com/user-attachments/assets/1eee8743-aa3f-42a3-977e-554e7abc36c0" />

---

### Step 7: View Saved Profiles

Run: **show profiles**

<img width="908" height="446" alt="9" src="https://github.com/user-attachments/assets/8d3a8c3f-d264-4271-b068-2307403d4b47" />

This shows all saved Wi-Fi profiles on the system.

Profiles represent networks the system has connected to before

---

### Step 8: Delete a Saved Profile (Optional)

To remove a profile: **delete profile name=profile-name**

<img width="579" height="95" alt="10" src="https://github.com/user-attachments/assets/cef90471-6ceb-4aae-bb35-f8ee79bd61d2" />

---

### Step 9: Disconnect from Network

Run: **disconnect**

<img width="748" height="157" alt="11" src="https://github.com/user-attachments/assets/73df01a6-8101-45dc-a715-2984b5946350" />

<img width="251" height="58" alt="12" src="https://github.com/user-attachments/assets/aca24fab-b348-48d9-a55a-048fbe3cff6e" />

---

### Step 10: Reconnect to Network

Run: **connect name=profile-name ssid=ssid-name**

<img width="742" height="90" alt="13" src="https://github.com/user-attachments/assets/3edfc201-e68b-48c5-a728-aa9f14c56b1f" />

---

### Step 11: Block a Wireless Network

1. Identify a network using: **show networks**

<img width="985" height="681" alt="14" src="https://github.com/user-attachments/assets/1eee8743-aa3f-42a3-977e-554e7abc36c0" />

<br/>

2. Block the network: **add filter permission=block ssid=TMOBILE-D051 networktype=infrastructure**

<img width="770" height="108" alt="15" src="https://github.com/user-attachments/assets/5aedd8c0-38ab-40a0-8757-722257005d00" />

The blocked network will not appear in the list.

Ran **show networks**

<img width="918" height="411" alt="17" src="https://github.com/user-attachments/assets/841cf4a5-481f-44a5-b621-ebba4d3b7ab4" />

The blocked network doesn't show

---

## Step 12: Verify Blocked Network

1. Run: **set blockednetworks display=show**

<img width="670" height="85" alt="16" src="https://github.com/user-attachments/assets/ac9bcd85-cdc2-4bc6-9020-8f55cc7df96a" />

2. then run **show networks**

<img width="762" height="387" alt="18" src="https://github.com/user-attachments/assets/ef4ca927-b6e3-4b7d-9565-4462bb9a2213" />

The blocked network is now displayed

---

### Step 14: Verify in Wi-Fi Menu

1. Click the Wi-Fi icon in the system tray.
2. Locate the blocked network.

<img width="805" height="497" alt="19" src="https://github.com/user-attachments/assets/753ab211-2eb0-4b42-afe3-edd85ce683fa" />

Observation:
- The network appears with a blocked indicator (X symbol) 

Run: **delete filter permission=block ssid=TMOBILE-D051 networktype=infrastructure**

<img width="812" height="73" alt="29" src="https://github.com/user-attachments/assets/58fefb94-58b8-4e82-a88f-cd08f90de1b7" />















