# 01 - Windows Sandbox Configuration

A hands-on lab demonstrating how to enable and configure **Microsoft Windows Sandbox** an isolated virtual environment for security tests without affecting the host machine.

## Objective

Implement host or application security solutions.


### What is Windows Sandbox?

Windows Sandbox is a lightweight, isolated virtual machine built into Windows 10/11. Anything run inside the sandbox, software installs, file downloads, configuration changes is completely discarded when the sandbox is closed. It never affects the underlying host machine.

---

## Tools Used

| Tool | Purpose |
|------|---------|
| W**indows Features** | Enabling Windows Sandbox |
| **Task Manager** | Verifying virtualization is enabled |
| **Windows Sandbox** | Isolated environment for testing |
| **Google Chrome** | Used to test sandbox isolation |

---

## Lab Guide

| File | Description |
|------|-------------|
| [**`01-Configure-Windows-Sandbox-Isolated-Environment.md`**](./01-Configure-Windows-Sandbox-Isolated-Environment.md) | Full step-by-step guide of enabling, configuring, and testing Windows Sandbox |

---

## Key Takeaway

Windows Sandbox provides an **isolated environment** completely separate from the host system. Any changes are permanently discarded when the sandbox is closed, making it an ideal tool for safely testing untrusted software or suspicious files without risking the host machine.
