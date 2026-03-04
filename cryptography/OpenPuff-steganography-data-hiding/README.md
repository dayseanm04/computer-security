# OpenPuff Steganography & Data Hiding

A hands-on cybersecurity project demonstrating **steganography**, the practice of concealing secret data within an ordinary file, using **OpenPuff**.

<img width="427" height="299" alt="OpenPuff" src="https://github.com/user-attachments/assets/81583a15-f326-4bfa-a180-cf45f6ebf03d" />

---

## What is Steganography?

Unlike **cryptography**, which scrambles a message so it cannot be read, **steganography hides the message**. A secret file is embedded inside a carrier file (such as an image), and to anyone without the passwords, the carrier looks completely normal and unchanged.

---

## Project Objective

- Understand the difference between cryptography and steganography
- Use OpenPuff to embed a hidden message inside a carrier image
- Recover and verify the hidden message using the Unhide feature

---

## Tools Used

| Tool | Purpose |
|------|---------|
| [**`OpenPuff`**](https://embeddedsw.net/OpenPuff_Steganography_Home.html) | Steganography & watermarking software |
| Windows Notepad | Creating the secret message |
| PowerShell | Creating project folders |

---

## How It Works

**1. Hide**
A secret message (**`Message.txt`**) is zipped and embedded into a carrier image (**`openPuff_Screenshot.png`**) using three different password in OpenPuff. The output image is visually identical to the original.

**2. Unhide**
Using the same three passwords and the carrier image, OpenPuff extracts and recovers the original **`Message.zip`**, which is then unzipped to reveal the secret message.

---

## Step-by-Step Guide

| Step | Guide |
|------|-------|
| 1 | [**`Download and Setup OpenPuff`**](./01-Guide/01-download-and-setup-OpenPuff.md) |
| 2 | [**`Hide Message with OpenPuff`**](./01-Guide/02-hide-message-with-OpenPuff.md) |
| 3 | [**`Unhide Message with OpenPuff`**](./01-Guide/03-unhide-message-with-OpenPuff.md) |

---

## Key Takeaway

> Steganography is a technique used in both **cybersecurity defense** and **threat actor tactics**. Understanding how data can be hidden inside ordinary files is essential knowledge for anyone working in security, digital forensics, or threat analysis.

## Author

**Daysean Mensah**  
Computer Systems student with a concentration in Network & Security. Passionate about threat analysis, security awareness, and building practical, real-world skills through hands-on labs and projects.

This project was completed as part of my personal cybersecurity learning journey.
