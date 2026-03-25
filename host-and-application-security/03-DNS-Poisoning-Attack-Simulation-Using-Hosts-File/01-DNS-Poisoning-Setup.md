# 01 DNS Poisoning Setup

## Overview
This section is the initial setup for a DNS poisoning attack simulation using a local hosts file. 
The setup phase includes preparing a safe testing environment, installing required tools, and gathering network information 
such as IP addresses.

---

## Objective

- Set up the lab environment using Windows Sandbox
- Install Notepad++ for editing system files
- Identify IP addresses of target websites

---

## Lab Environment

| Component | Details |
|---|---|
| Environment | Windows Sandbox |
| Operating System | Windows 10/11 |
| Tools | Notepad++ |

---

### Step 1: Launch Windows Sandbox

1. Open the Start menu.
2. Search for **Windows Sandbox**.
3. Launch the application.

<img width="844" height="432" alt="10" src="https://github.com/user-attachments/assets/1f531b10-5032-417e-8d29-366649f35bb4" />

---

### Step 2: Install Notepad++

1. Open a Microsoft Edge inside Windows Sandbox.
2. Navigate to: **https://notepad-plus-plus.org/downloads/** or search up Notepad++ Download
3. Download and install Notepad++.
4. Go to Download Folder and Run the installer

---

### Step 3: Access Target Websites

1. Open a web browser.
2. Navigate to a website example: https://www.wku.edu

<img width="855" height="582" alt="11" src="https://github.com/user-attachments/assets/c8e341a1-f20f-4b3d-b757-4155ca341275" />

3. Open another website such as your school or organization site, example: https://www.nyu.edu/

<img width="848" height="475" alt="12" src="https://github.com/user-attachments/assets/4e30f060-53cd-41d8-86d9-701abb1c5470" />

---

### Step 4: Identify IP Addresses

To simulate DNS poisoning, you need the IP addresses of the target websites.

### Method 1: Using ping

1. Open Command Prompt.
2. Run: **ping nyu.edu**

<img width="807" height="434" alt="13" src="https://github.com/user-attachments/assets/62488c83-2425-49d6-8238-b434206a2f64" />

3. Run: **ping www.wku.edu**

<img width="747" height="438" alt="15" src="https://github.com/user-attachments/assets/7868d80b-e618-469f-88fb-e4e8564b5300" />

---

### Method 2: Using an IP Lookup Website

1. Go to: **https://ipaddress.com**

<img width="990" height="471" alt="14 3" src="https://github.com/user-attachments/assets/82f1ee55-406b-4c62-a7b7-645733aacff8" />

2. Click on the **Search bar** top right
3. Search up the domain names

#### NYU
<img width="913" height="577" alt="14" src="https://github.com/user-attachments/assets/d1a11234-8f1e-4704-b1f9-a6e451f10677" />

#### WKU

<img width="904" height="664" alt="14 2" src="https://github.com/user-attachments/assets/a08df2ef-02d3-4ef8-9af6-82baf3b0c06d" />

### Step 5: Verify IP Address

To confirm the IP address belongs to the correct website:

1. Enter the IP address in Microsoft Edge

<img width="782" height="307" alt="16" src="https://github.com/user-attachments/assets/9484ca3e-ee39-4b4c-98e8-e3909b6a5c50" />


































