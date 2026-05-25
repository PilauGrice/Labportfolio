# Cybersecurity Lab Portfolio - Complete Edition

**Portfolio Date**: May 2026 | **Author**: PilauGrice | **Last Updated**: 2026-05-25

---

## Table of Contents

1. [Overview](#overview)
2. [Unit 2: Footprinting & Passive Reconnaissance (OSINT)](#unit-2-footprinting--passive-reconnaissance-osint)
3. [Unit 3: Active Reconnaissance & Local Subnet Diagnostics](#unit-3-active-reconnaissance--local-subnet-diagnostics)
4. [Unit 4: Controlled Exploitation & Automated Auditing](#unit-4-controlled-exploitation--automated-auditing)
5. [Formal Laboratory Question Responses](#formal-laboratory-question-responses)

---

## Overview

This portfolio documents a comprehensive cybersecurity laboratory focused on open-source threat intelligence (OSINT), passive reconnaissance, active reconnaissance, and controlled exploitation techniques.

### Learning Objectives

- Master OSINT methodologies using automated node graph linkages (Maltego)
- Execute CLI-based DNS and network registry lookups
- Conduct subnet diagnostics and active reconnaissance
- Perform controlled vulnerability exploitation and post-exploitation analysis
- Execute automated vulnerability auditing with enterprise-grade tools

### Key Technologies

- **Reconnaissance**: Maltego, whois, dig, nmap
- **Exploitation**: Metasploit Framework, Nessus
- **Target Platforms**: Kali Linux, Ubuntu, Metasploitable
- **Analysis**: CVSS/CVE frameworks, vulnerability scoring

---

# Unit 2: Footprinting & Passive Reconnaissance (OSINT)

## Overview

This module evaluates open-source threat intelligence data compilation using automated node graph linkages (Maltego) and low-level CLI lookup systems targeting public DNS and network registries.

---

## Exercise 2.1: Package Architecture Setup & Registry Troubleshooting

### Problem Statement

During initial deployment of Maltego on the Kali Linux platform, an upstream signature error was flagged by the Advanced Package Tool due to a missing repository cryptographic token key: `ED65462EC8D5E4C5`

### Solution

The security blockage was remediated by manually injecting the certified 2025 Kali keyserver token:

```bash
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys ED65462EC8D5E4C5
```

### Key Milestones

1. **APT Package Manager Keyring Error Verification** - ![APT Keyring Error](images/2026-05-20-180258.png)
2. **Keyserver Cryptographic Token Import** - ![Keyserver Token](images/2026-05-20-180737.png)
3. **Maltego 4.11 Compilation** - ![Maltego Compilation](images/2026-05-20-180923.jpg)
4. **JVM Environment Verification** - ![JVM Environment](images/2026-05-20-183420.jpg)

---

## Exercise 2.2: Maltego Open-Source Transform Analytics

### Target: Clotet / Funicular Films

#### Intelligence Gathering Phases

- ![Phase 2](images/2026-05-20-192449.png) - Hierarchical Entity Mapping
- ![Phase 3](images/2026-05-20-193625.png) - Cross-Reference Mapping
- ![Phase 4](images/2026-05-20-193916.png) - Relationship Interconnection
- ![Phase 5](images/2026-05-20-194016.png) - Master Structural Verification

#### High-Value Extractions

- ![Domain Harvesting](images/2026-05-20-194951.png) - Apex Domain Extraction
- ![URL Parsing](images/2026-05-20-195129.png) - Schema Resolution
- ![Scope Locking](images/2026-05-20-195353.png) - Target Boundary Locking
- ![Social Engineering](images/2026-05-20-200019.png) - Communication Endpoint Mapping
- ![External Dependencies](images/2026-05-20-200320.png) - Relationship Dependencies
- ![Geographic Intelligence](images/2026-05-20-201446.png) - Regional Infrastructure
- ![Historical Analysis](images/2026-05-20-201510.png) - Wayback Machine Timeline
- ![Final Canvas](images/2026-05-20-201630.png) - Decade-Scale OSINT Canvas
- ![Entity Mapping](images/2026-05-20-202149.png) - Inbound Web Entities
- ![Content Mapping](images/2026-05-20-203338.png) - Sub-Layer Structure
- ![Final Extraction](images/2026-05-20-203528.png) - Funicular Films Mapping

---

## Exercise 2.3: Pure Command-Line Terminal Reconnaissance

### WHOIS Analysis - ![WHOIS](images/2026-05-20-211734.png)
### DNS Resolution - ![DNS](images/2026-05-20-211840.png)
### RIR Netblock - ![Netblock](images/2026-05-20-212100.png)
### Service Provider - ![Provider](images/2026-05-20-212244.png)

---

# Unit 3: Active Reconnaissance & Local Subnet Diagnostics

## Exercise 3.1: Machine Baseline Profiling

- ![Ubuntu Gateway](images/2026-05-20-213617.png)
- ![Kali Linux](images/2026-05-20-213659.png)
- ![Metasploitable](images/2026-05-20-213843.png)
- ![Legacy Bypass](images/2026-05-20-213952.png)

## Exercise 3.2: Subnet Interface Mapping

- ![ifconfig Error](images/2026-05-20-214025.png)
- ![Net-tools Install](images/2026-05-20-214042.png)
- ![Ubuntu Gateway Config](images/2026-05-20-214110.png)
- ![Kali Config](images/2026-05-20-214152.png)
- ![Metasploitable Config](images/2026-05-20-214210.png)

## Exercise 3.3: Link MTU Testing

- ![MTU Test](images/2026-05-20-214443.png)

## Exercise 3.4: Port Scanning & Banner Grabbing

- ![Nmap Sweep](images/2026-05-20-214530.png)
- ![Banner Grabbing](images/2026-05-20-214757.png)
- ![Version Fingerprinting](images/2026-05-20-214948.png)

---

# Unit 4: Controlled Exploitation & Automated Auditing

## Exercise 4.1: Metasploit Exploitation

- ![Exploit Configuration](images/2026-05-20-215243.png)
- ![Parameter Verification](images/2026-05-20-220544.png)
- ![Exploitation](images/2026-05-20-215400.png)
- ![Passwd Extraction](images/2026-05-20-215536.png)
- ![Shadow Extraction](images/2026-05-20-215550.png)
- ![Session Stability](images/2026-05-20-215737.png)
- ![Network Routing](images/2026-05-20-215902.png)
- ![Lateral Movement](images/2026-05-20-220744.png)

## Exercise 4.2: Nessus Vulnerability Audit

- ![Nessus Installation](images/2026-05-21-202131.png)
- ![Dependency Error](images/2026-05-20-220309.png)
- ![Path Remediation](images/2026-05-20-220410.png)
- ![Web Interface](images/2026-05-21-203718.png)
- ![Licensing Portal](images/2026-05-21-203904.png)
- ![Scope Definition](images/2026-05-21-205443.png)
- ![Scan Progress](images/2026-05-21-205402.png)
- ![Vulnerability Results](images/2026-05-21-210009.png)
- ![Multi-Scan Tracking](images/2026-05-21-210419.png)
- ![Common Ports Results](images/2026-05-21-210736.png)
- ![All Ports Results](images/2026-05-21-215434.png)

---

# Formal Laboratory Question Responses

## Core Framework Definitions

### CVE (Common Vulnerabilities and Exposures)

CVE assigns unique tracking identifiers to publicly disclosed security flaws, providing universal naming convention across security tools and remediation logs.

**Importance**:
- Standardization of vulnerability references
- Precise communication across departments
- Automation of scanning tool correlation
- Longitudinal monitoring across asset inventory
- Compliance with regulatory requirements

### CVSS (Common Vulnerability Scoring System)

CVSS generates quantitative severity scores (0.0-10.0) based on technical characteristics of vulnerabilities.

**Score Tiers**:
| Range | Severity | Priority |
|---|---|---|
| 9.0-10.0 | Critical | Patch immediately |
| 7.0-8.9 | High | Within 1-2 weeks |
| 4.0-6.9 | Medium | Within 30 days |
| 0.1-3.9 | Low | Regular cycle |

## Post-Exploitation Analysis

### FTP Version Criticality

vsftpd 2.3.4 was compromised in July 2011 with a supply-chain attack enabling immediate root access via smiley face trigger (`:)`) in authentication attempts.

### /etc/passwd vs /etc/shadow

| Aspect | /etc/passwd | /etc/shadow |
|--------|---|---|
| **Permissions** | World-readable (644) | Root-only (600) |
| **Contents** | Metadata only | Password hashes |
| **Risk** | Low | **CRITICAL** |

### System Compromise Assessment

Successful extraction of both files demonstrates **absolute system compromise**:
- Root administrative access obtained
- Offline password cracking enabled
- Lateral movement feasible
- Full data access capability
- Requires immediate isolation and remediation

---

## Vulnerability Chain Summary

```
Passive OSINT → Active Reconnaissance → Service Enumeration → 
Exploit Selection → Root Access → Credential Harvesting → 
Offline Cracking → Lateral Movement → Persistence
```

## Key Takeaways

✅ Version intelligence enables targeted exploitation  
✅ File permissions are critical security boundaries  
✅ Supply-chain attacks pose insidious threats  
✅ Defense in depth is essential  
✅ Incident response planning must be pre-planned  

---

**Laboratory Completion Date**: May 25, 2026 | **Portfolio Version**: 1.0

*End of Document*
