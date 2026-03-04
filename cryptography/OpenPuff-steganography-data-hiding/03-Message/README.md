# 03-Message

This folder contains the **secret message** used in the OpenPuff steganography lab/project, in both its plain text and zipped forms.

---

## 📁 Files

| File | Description |
|------|-------------|
| **`Message.txt`** | Plain text file containing the secret message |
| **`Message.zip`** | Zipped version of `Message.txt`, this is the file loaded into OpenPuff for hiding |

---

## What is the Message?

The secret message is a plain text file containing:

```
This is a secret message
```

OpenPuff requires the message to be in a **zip format** before it can be embedded into the carrier file.

---

## How It's Used

- **`Message.txt`** is created in **Step 4** of [**`01-download-and-setup-OpenPuff.md`**](../01-Guide/01-download-and-setup-OpenPuff.md)
- **`Message.zip`** is created in **Step 5** of [**`01-download-and-setup-OpenPuff.md`**](../01-Guide/01-download-and-setup-OpenPuff.md)
- **`Message.zip`** is loaded into OpenPuff in **Step 3** of [**`2-hide-message-with-OpenPuff.md`**](../01-Guide/02-hide-message-with-OpenPuff.md)

---

## Back to Repo

[OpenPuff-steganography-data-hiding](../README.md)
