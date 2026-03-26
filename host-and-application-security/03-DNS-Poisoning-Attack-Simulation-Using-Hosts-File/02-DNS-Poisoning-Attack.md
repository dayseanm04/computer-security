# 02 DNS Poisoning Attack

## Overview

This lab shows how changing the hosts file can redirect a website to a different IP address.

---

## Objective

- Modify the local hosts file
- Redirect a legitimate domain to a different IP address
- Observe how DNS resolution is overridden

---

## Lab Environment

| Component | Details |
|---|---|
| Environment | Windows Sandbox |
| Operating System | Windows 10/11 |
| Tool | Notepad++ (Administrator) |

---

### Step 1: Open Notepad++ as Administrator
1. Click the Start menu.
2. Search for **Notepad++**.
3. Click **Run as administrator**.

<img width="1086" height="413" alt="18" src="https://github.com/user-attachments/assets/121c7ec2-ab48-4c9c-93ed-0f9ab6404bfd" />

---

### Step 2: Open the Hosts File

1. In Notepad++, click **File** and **Open**.

<img width="630" height="259" alt="19" src="https://github.com/user-attachments/assets/fef14820-438c-4909-94aa-ace09b3742d1" />

2. Navigate to C:\Windows\System32\drivers\etc\
3. Select **host**
4. Ensure **All type** is the file type

<img width="876" height="537" alt="20" src="https://github.com/user-attachments/assets/99d01c8c-3cb0-4ae1-a2d3-9012a265784f" />

5. Click **Open**

<img width="775" height="522" alt="21" src="https://github.com/user-attachments/assets/92885af8-c08e-44df-9962-d06987472d7b" />


---

### Step 3: Add Malicious Entry

Scroll to the bottom of the hosts file.

Add a new entry using the following: **161.6.96.74 www.nyu.edu**



























