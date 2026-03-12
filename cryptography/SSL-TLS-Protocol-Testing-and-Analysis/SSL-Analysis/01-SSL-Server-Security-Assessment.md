# 01-SSL-Server-Security-Assessment

## Overview
This lab evaluates the security configuration of web servers and web browsers using the Qualys SSL Labs testing platform. The purpose is to understand how SSL/TLS configurations protect communications between clients and servers and to identify potential security weaknesses.

In this assessment, SSL Labs is used to analyze:
- SSL/TLS protocol support
- Digital certificate configuration
- Cipher suite strength
- Key exchange mechanisms

---

## Objectives
- Analyze the SSL/TLS security configuration of web servers
- Understand how SSL Labs evaluates server security
- Identify weak protocols and insecure cipher suites
- Review certificate chains and trust relationships

---

### Step 1: Access SSL Labs

1. Open a web browser.
2. Navigate to the SSL Labs website: **https://www.ssllabs.com**

![SS1](../Screenshots/SS1.png)
3. Click **"Test Your Server"**.

![SS2](../Screenshots/ss2.png)

---

### Step 2: Analyze a Highly Rated Server
1. Under **Recent Best**, select the first website listed.

![SS3](../Screenshots/SS3.png)


Review the **Summary** section and record the following:

- Overall Rating

![SS4](../Screenshots/SS4.png)

- Certificate 

![SS5](../Screenshots/SS5.png)

- Protocol support score

![SS7](../Screenshots/SS7.png)

A strong server configuration typically receives an **A or A+ rating**, indicating secure protocol configuration and strong encryption.

---

### Step 3: Review Certificate Information
Scroll down to **Certificate #1**.

![SS5](../Screenshots/SS5.png)

Observe:
- Certificate issuer
- Signature algorithm
- Key size
- Validity dates
- Site alternative names





























