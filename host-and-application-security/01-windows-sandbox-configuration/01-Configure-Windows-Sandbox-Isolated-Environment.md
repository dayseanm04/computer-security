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




