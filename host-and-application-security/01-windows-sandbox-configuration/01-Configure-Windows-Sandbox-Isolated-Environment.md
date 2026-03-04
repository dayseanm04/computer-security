# 01 - Configure Windows Sandbox Isolated Environment

## Overview

**Objective:** Implement host or application security solutions. A sandbox is an isolated virtual machine, anything run within a sandbox will impact only the virtual machine and not the host machine.

---


## Step 1: Check if Virtualization is Enabled

1. Right-click the **taskbar** at the bottom of the screen
2. Select **Task Manager**
3. Click the **Performance** tab
4. Look for **Virtualization** — it must say **Enabled**

> **Note:** If it says **Disabled**, you will need to reboot, enter your **BIOS or UEFI**, and turn on virtualization before proceeding.

![SS1](/host-and-application-security/01-windows-sandbox-configuration/01-Images/1.png)

---

## Step 2: Enable Windows Sandbox

1. In the Windows search box on the taskbar, type **Windows Features**
2. Click **Turn Windows features on or off** from the results

![SS2](/host-and-application-security/01-windows-sandbox-configuration/01-Images/2.png)

3. Scroll down and check the **Windows Sandbox** checkbox
4. Click **OK**

![SS3](/host-and-application-security/01-windows-sandbox-configuration/01-Images/3.png)

5. Windows will search for required files and apply the changes
6. When prompted, click **Restart Now** to reboot your PC

![SS4](/host-and-application-security/01-windows-sandbox-configuration/01-Images/4.png)
![SS5](/host-and-application-security/01-windows-sandbox-configuration/01-Images/5.png)

---

## Step 3: Launch Windows Sandbox

1. Search up **Windows Sandbox**

![SS6](/host-and-application-security/01-windows-sandbox-configuration/01-Images/6.png)

2. click **Windows Sandbox** to launch it

![SS7](/host-and-application-security/01-windows-sandbox-configuration/01-Images/7.png)
![SS8](/host-and-application-security/01-windows-sandbox-configuration/01-Images/8.png)

> A protected virtual machine that looks like a Windows instance will start up.


---

## Step 4: Test the Sandbox — Install Google Chrome

1. Inside the Windows Sandbox, open **Microsoft Edge**
2. Download and install **Google Chrome**
3. Confirm the installation completed successfully

![SS9](/host-and-application-security/01-windows-sandbox-configuration/01-Images/9.png)

---

## Step 5: Close the Sandbox

1. Close the Windows Sandbox window
2. A warning will appear:

![SS10](/host-and-application-security/01-windows-sandbox-configuration/01-Images/10.png)

3. Click **OK** to confirm

---

## Step 6: Relaunch and Verify Isolation

1. Relaunch **Windows Sandbox** from the Start menu
2. Check if Google Chrome is still installed

**What happened to Google Chrome?**

Google Chrome was gone. It was deleted because the Windows Sandbox resets completely every time it is closed, nothing installed or changed inside the sandbox is saved to the host machine and the VM. This demonstrates the purpose of a sandbox: **complete isolation**.

![SS11](/host-and-application-security/01-windows-sandbox-configuration/01-Images/11.png)

---

## Step 7: Close All Windows

1. Close the Windows Sandbox
2. Close all remaining open windows

---

## Lab Completed

I have successfully:
- Verified virtualization was enabled on the host machine
- Enabled and configured Windows Sandbox via Windows Features
- Launched the sandbox and installed Google Chrome inside it
- Confirmed that the sandbox environment is fully isolated and resets on every close
