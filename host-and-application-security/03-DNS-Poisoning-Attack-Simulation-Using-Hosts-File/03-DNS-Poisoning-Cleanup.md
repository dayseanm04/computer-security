# 03 DNS Poisoning Cleanup

## Overview
In this section, I will to remove the changes made to the hosts file.

After simulating a DNS poisoning attack, it is important to clean up the system to prevent unintended redirection and ensure proper domain name resolution.

**Note: I used a sandbox for this lab but I will still cleanup**

---

## Objective

- Remove malicious entries from the hosts file
- Clear cached DNS records

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


























