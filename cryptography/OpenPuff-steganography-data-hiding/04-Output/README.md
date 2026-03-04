# 04-Output

This folder contains the output files generated during the **OpenPuff Steganography Data Hiding** lab/project. It is split into two subfolders representing the two stages of the process.

---

## 📂 Subfolders

### `stegano/`
Contains the **carrier image with the hidden message embedded inside it**. This is the output from the Hide process in OpenPuff. The image looks visually identical to the original carrier file in [**`02-Carrier/`**](../02-Carrier/), but contains the secret message hidden within its data.

### `stegano-out/`
Contains the **recovered secret message** extracted from the carrier image. This is the output from the Unhide process in OpenPuff. The recovered **`Message.zip`** is extracted here, which contains the original **`Message.txt`**.

---

## 🔗 How It's Used

- The **`stegano/`** output is generated in **Step 5** of [**`02-hide-message-with-OpenPuff.md`**](../01-Guide/02-hide-message-with-OpenPuff.md)
- The `stegano-out/` output is generated in **Step 11** of [**`03-unhide-message-with-OpenPuff.md`**](../01-Guide/03-unhide-message-with-OpenPuff.md)

---

## Back to Repo

[OpenPuff-steganography-data-hiding](../README.md)
