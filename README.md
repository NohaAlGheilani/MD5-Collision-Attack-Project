# MD5-Collision-Attack-Project

## Overview
This repository contains the practical and theoretical work for the **Advanced Cryptography (CSSY4102)** course project on **MD5 Collision Attacks**.  
The project demonstrates how MD5, once widely used for digital signatures, SSL certificates, and file integrity checks, is now considered broken due to its vulnerability to collision attacks.

---

## Author
- Noha Mohammed Al‑Gheilani (ID: 2021493026)  

---

## Contents

### 1. MD5 Fundamentals
- How MD5 works (padding, compression, chaining)  
- Avalanche effect and design principles  

### 2. Vulnerabilities
- Historical timeline of MD5 weaknesses  
- Real-world incidents (e.g., Flame malware, CVE-2024-4765)  

### 3. Collision Attack Techniques
- Plain collisions vs. chosen-prefix collisions  
- Tools used: md5collgen  
- Practical demonstrations of binary and executable collisions  

### 4. Experimental Lab Tasks
- Task 1: Generating two files with the same MD5 hash  
- Task 2: Demonstrating MD5’s append property  
- Task 3: Creating two executables with identical MD5 hashes  
- Task 4: Crafting benign and malicious programs with the same MD5 hash  

### 5. Findings
- Collision preservation under concatenation  
- Security implications for code signing and authentication  
- Necessity of migration to secure alternatives (SHA-256, SHA-3)  

---

## Key Results
- Successfully generated colliding files in less than 5 seconds using `md5collgen`.  
- Demonstrated append property: collisions persist even after concatenation.  
- Built two distinct executables with identical MD5 hashes.  
- Created benign vs. malicious programs sharing the same MD5 fingerprint.  

---

## Security Implications
- Digital signatures can be forged using MD5 collisions.  
- Software updates and certificates relying on MD5 are vulnerable.  
- Immediate migration to SHA-256 or SHA-3 is strongly recommended.  

---

## Tools & Environment
- md5collgen (Marc Stevens’ collision generator)  
- Linux utilities: `md5sum`, `diff`, `hexdump`, `cat`, `head`, `tail`  
- C programming for executable demonstrations  
- Hex editors for binary manipulation  

---

## Recommended Alternatives
- SHA-256: Strong collision resistance, widely adopted.  
- SHA-3 (Keccak): Sponge construction, avoids MD5’s structural weaknesses.  

---

## This project is for academic and educational purposes only.  
Do not use MD5 in production systems.  

---

## References
- Ronald Rivest (1991) – MD5 Design  
- Xiaoyun Wang (2004) – Practical Collision Attack  
- Marc Stevens – md5collgen tool  
- NIST & IETF – MD5 deprecation standards  
