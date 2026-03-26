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


<img width="876" height="537" alt="20" src="https://github.com/user-attachments/assets/99d01c8c-3cb0-4ae1-a2d3-9012a265784f" />

5. Click **Open**

### Step 3: Remove Malicious Entry

1. Locate the entry that was added during the attack phase.
2. 161.6.96.74 www.nyu.edu
3. Delete this line from the file.

<img width="775" height="522" alt="21" src="https://github.com/user-attachments/assets/92885af8-c08e-44df-9962-d06987472d7b" />

---

### Step 4: Save the File

1. Click **File** and **Save**
2. Close **Notepad++**


---

### Step 5: Flush DNS Cache

To remove cached DNS records:

1. Open Command Prompt.
2. Run: **ipconfig /flushdns**

---


### Step 6: Verify Restoration

1. Open a web browser.
2. Navigate to the domain **https://www.nyu.edu**

<img width="848" height="475" alt="12" src="https://github.com/user-attachments/assets/4e30f060-53cd-41d8-86d9-701abb1c5470" />









































