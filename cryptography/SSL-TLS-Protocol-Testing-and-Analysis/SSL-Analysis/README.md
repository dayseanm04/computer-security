# SSL/TLS Analysis

<img width="1426" height="234" alt="ssl-labs-logo" src="https://github.com/user-attachments/assets/9000da60-6623-45ed-afca-003c3ea06d26" />

## Overview

This section documents the SSL/TLS security testing I performed as part of the **SSL-TLS Protocol Testing and Analysis** lab. The objective of this lab was to evaluate the security configuration of a web server using industry-standard tools and to analyze how different web browsers interact with SSL/TLS connections.

The analysis includes both **server-side security assessment** and **client-side browser testing** to observe certificate validation and connection security detail.

The **Qualys SSL Labs** testing platform was used to analyze the server’s TLS configuration and identify potential weaknesses in the implementation.

---

## Lab Navigation

| Step | Analysis | Description |
|-----|-----|-----|
| 1 | [**`SSL Server Security Assessment`**](./01-SSL-Server-Security-Assessment.md) | Evaluates the server's TLS configuration and security posture using Qualys SSL Labs. |
| 2 | [**`SSL Client Test – Google Chrome`**](./02-SSL-Client-Test-Google-Chrome.md) | Examines certificate and connection security details using the Chrome browser. |
| N/A | Google Chrome Test Report | Raw output and documentation from the Chrome browser test. |
| 3 | [**`SSL Client Test – Microsoft Edge`**](./04-SSL-Client-Test-Microsoft-Edge.md) | Analyzes SSL/TLS connection details using Microsoft Edge. |
| N/A | Microsoft Edge Test Report | Raw output and documentation from the Edge browser test. |

---

## Analysis Scope

This lab focuses on three primary components of SSL/TLS security evaluation:

### 1. Server Security Assessment

The server configuration was analyzed using **Qualys SSL Labs**, which evaluates: **TLS protocol versions**, **Certificate configuration**, **Key exchange mechanisms**, **Cipher suite security** and **Overall SSL/TLS security rating**

This analysis helps identify whether the server follows modern cryptographic security standards.

---


