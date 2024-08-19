
# Wi-Fi Security Protocols: WEP, WPA, and WPA2

## Table of Contents
- [Introduction](#introduction)
- [WEP (Wired Equivalent Privacy)](#wep-wired-equivalent-privacy)
- [WPA (Wi-Fi Protected Access)](#wpa-wi-fi-protected-access)
- [WPA2 (Wi-Fi Protected Access II)](#wpa2-wi-fi-protected-access-ii)
- [Comparison of Protocols](#comparison-of-protocols)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction
This repository contains a detailed report on the evolution and technical aspects of Wi-Fi security protocols, specifically focusing on WEP, WPA, and WPA2. These protocols are crucial in protecting wireless networks from unauthorized access and ensuring data security. The detailed report is in [Report](./Report-Research-9931061-Justified.pdf) 

## WEP (Wired Equivalent Privacy)
WEP was the first security protocol introduced in 1999 as part of the original IEEE 802.11 standard. It was designed to provide the same level of security as wired networks by encrypting data transmitted over the wireless network. However, WEP has several vulnerabilities:

- **Weak encryption**: Uses RC4 stream cipher with 40-bit or 104-bit keys, which are easily crackable.
- **IV (Initialization Vector) issues**: The 24-bit IV used in WEP is too short, leading to frequent reuse and making the protocol vulnerable to attacks like the FMS attack.
- **Lack of integrity checks**: WEP does not provide proper data integrity checks, making it susceptible to bit-flipping attacks.

Due to these flaws, WEP was deprecated in 2004.

## WPA (Wi-Fi Protected Access)
WPA was introduced in 2003 as an interim solution to address the shortcomings of WEP. WPA implemented several key improvements:

- **TKIP (Temporal Key Integrity Protocol)**: Enhanced encryption by dynamically changing keys with each packet, reducing the risk of attacks like key reuse.
- **Message Integrity Check (MIC)**: Added a new integrity check mechanism to prevent data tampering.
- **Backward compatibility**: WPA was designed to be compatible with older WEP hardware through software updates.

Despite these enhancements, WPA was still vulnerable to certain attacks, particularly with the RC4 cipher, leading to the development of WPA2.

## WPA2 (Wi-Fi Protected Access II)
WPA2, introduced in 2004, is the most widely used Wi-Fi security protocol today. It includes significant advancements over its predecessors:

- **AES (Advanced Encryption Standard)**: Replaces RC4 with AES, a more secure and robust encryption method.
- **CCMP (Counter Mode with Cipher Block Chaining Message Authentication Code Protocol)**: Provides strong data confidentiality, integrity, and origin authentication.
- **Strong encryption**: Uses 128-bit keys, making it much harder to crack.
- **Enterprise and Personal modes**: Supports both individual users (WPA2-Personal) and enterprise environments (WPA2-Enterprise) with authentication through a RADIUS server.

WPA2 remains the standard for Wi-Fi security, though WPA3 has been introduced to address emerging threats.

## Comparison of Protocols
| Feature           | WEP                    | WPA                    | WPA2                  |
|-------------------|------------------------|------------------------|-----------------------|
| Encryption        | RC4 (40/104-bit)       | RC4 with TKIP          | AES (128-bit)         |
| Integrity         | CRC-32                 | MIC                    | CCMP                  |
| Vulnerabilities   | IV reuse, weak keys    | TKIP weaknesses        | KRACK (fixes available)|
| Deployment Date   | 1999                   | 2003                   | 2004                  |
| Status            | Deprecated             | Superseded by WPA2     | Current Standard      |

## Conclusion
Understanding the evolution of Wi-Fi security protocols is essential for anyone working with wireless networks. While WEP, WPA, and WPA2 have served as critical components in securing Wi-Fi communications, it’s important to recognize their limitations and the ongoing need for stronger security measures, as seen with the introduction of WPA3.

## References
- [IEEE 802.11 Standards](https://www.ieee.org/)
- [Wi-Fi Alliance](https://www.wi-fi.org/)
- Research papers and articles on wireless security protocols.
