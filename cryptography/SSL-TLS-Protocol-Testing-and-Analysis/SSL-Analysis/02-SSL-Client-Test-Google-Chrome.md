# 02 SSL Client Test Google Chrome

## Overview
This lab evaluates the SSL/TLS security capabilities of the **Google Chrome web browser** using the **Qualys SSL Labs Client Test** tool.

The test analyzes how the browser handles encrypted communications, including supported protocols, cipher suites, and vulnerability protections. Understanding browser SSL/TLS capabilities is important because web browsers act as the client in secure communications and must properly support modern encryption standards.

The results provide insight into how Chrome protects users against common cryptographic vulnerabilities.

---

## Objective
- Evaluate the SSL/TLS capabilities of Google Chrome
- Identify supported encryption protocols
- Review supported cipher suites
- Verify protection against known cryptographic vulnerabilities

---

### Step 1: Access SSL Labs

1. Open a web browser.
2. Navigate to the SSL Labs website: **https://www.ssllabs.com**

![SS1](../Screenshots/SS1.png)

3. Click on **projects**

![SS16](../Screenshots/SS16.png)

5. Click on **SSL Client Test**

![SS20](../Screenshots/SS20.png)

## 1. Protocol Support

Chrome supports the latest secure TLS protocols and disables legacy protocols.

| Protocol | Supported |
|---|---|
| TLS 1.3 | Yes |
| TLS 1.2 | Yes |

---

## 2. Vulnerability Protection

![SS21](../Screenshots/SS21.png)

The scan confirms Chrome is protected against several major TLS-related attacks.

| Vulnerability | Status |
|---|---|
| CVE-2020-0601 (CurveBall) | Not Vulnerable |
| Logjam Attack | Not Vulnerable |
| FREAK Attack | Not Vulnerable |
| POODLE Attack | Not Vulnerable |

---

## 3. Cipher Suites

![SS22](../Screenshots/SS22.png)


Chrome prioritizes **modern cipher suites that provide forward secrecy and strong encryption**.

### Strong Cipher Suites

| Cipher Suite | Encryption | Security Feature |
|---|---|---|
| TLS_AES_128_GCM_SHA256 | 128-bit | Forward Secrecy |
| TLS_AES_256_GCM_SHA384 | 256-bit | Forward Secrecy |
| TLS_CHACHA20_POLY1305_SHA256 | 256-bit | Forward Secrecy |
| TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256 | 128-bit | Forward Secrecy |
| TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256 | 128-bit | Forward Secrecy |

### Legacy / Weak Cipher Suites

Some weaker suites remain for backward compatibility.

| Cipher Suite | Status |
|---|---|
| TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA | Weak |
| TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA | Weak |
| TLS_RSA_WITH_AES_128_GCM_SHA256 | Weak |
| TLS_RSA_WITH_AES_256_GCM_SHA384 | Weak |
| TLS_RSA_WITH_AES_128_CBC_SHA | Weak |
| TLS_RSA_WITH_AES_256_CBC_SHA | Weak |

---

## Protocol Features

| Feature | Supported |
|---|---|
| Server Name Indication (SNI) | Yes |
| Secure Renegotiation | Yes |
| TLS Compression | No |
| Session Tickets | Yes |
| OCSP Stapling | Yes |
| Application Layer Protocol Negotiation (ALPN) | Yes |

These features improve performance and security during TLS connections.

---

# Security Analysis

### Strengths

Google Chrome demonstrates strong SSL/TLS security because it:

- Supports **TLS 1.3 and TLS 1.2**
- Supports **forward secrecy**
- Protects against major TLS vulnerabilities
- Blocks insecure mixed content
 
### Minor Weaknesses

Some weaker cipher suites remain supported for compatibility with older servers. These are rarely used because modern servers prioritize stronger cipher suites.

# Conclusion

The SSL Labs Client Test shows that **Google Chrome provides strong cryptographic security for HTTPS communications**.

Key security benefits include:

- support for modern TLS protocols
- protection against major cryptographic attacks
