# Cybersecurity Lab Portfolio - Evidence & Analysis Log

**Portfolio Date**: May 2026 | **Author**: PilauGrice | **Last Updated**: 2026-05-25

---

## Table of Contents

1. [Unit 2: Footprinting & Passive Reconnaissance (OSINT)](#unit-2-footprinting--passive-reconnaissance-osint)
2. [Unit 3: Active Reconnaissance & Local Subnet Diagnostics](#unit-3-active-reconnaissance--local-subnet-diagnostics)
3. [Unit 4: Controlled Exploitation & Automated Auditing](#unit-4-controlled-exploitation--automated-auditing)
4. [Formal Laboratory Question Responses](#formal-laboratory-question-responses)

---

# Unit 2: Footprinting & Passive Reconnaissance (OSINT)

This module evaluates open-source threat intelligence data compilation using automated node graph linkages (Maltego) and low-level CLI lookup systems targeting public DNS and network registries.

## Exercise 2.1: Package Architecture Setup & Registry Troubleshooting

During initial deployment of Maltego on the Kali Linux platform, an upstream signature error was flagged by the Advanced Package Tool due to a missing repository cryptographic token key (`ED65462EC8D5E4C5`).

The security blockage was bypass-remediated by manually injecting the certified 2025 Kali keyserver token using an advanced keyserver request string:
`sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys ED65462EC8D5E4C5`

#### Figure 1.1: APT Package Manager Keyring Error Verification
![Figure 1.1](images/2026-05-20-180258.png)
*Caption: Diagnostic logs tracking authentication blocks during repository indexing initialization.*

#### Figure 1.2: Keyserver Cryptographic Token Import
![Figure 1.2](images/2026-05-20-180737.png)
*Caption: Terminal stdout validating successful keyring signature injection.*

#### Figure 1.3: Maltego 4.11 Compilation
![Figure 1.3](images/2026-05-20-180923.jpg)
*Caption: Package unpacking trace verifying absolute library installation parameters.*

#### Figure 1.4: JVM Environment Verification
![Figure 1.4](images/2026-05-20-183420.jpg)
*Caption: Console trace verifying active memory heap configuration boundaries at `/usr/lib/jvm/java-11-openjdk-amd64`.*

---

## Exercise 2.2: Maltego Open-Source Transform Analytics (Target: Funicular Films)

A multi-tier open intelligence exploration loop was targeted at personal identifiers (Aina Clotet, Marc Clotet) to expand initial names into corporate entities and infrastructure assets.

#### Figure 1.5: Phase 1 — Initial Name Phrase Configuration
![Figure 1.5](images/2026-05-20-190853.jpg)
*Caption: Tracking baseline website naming configurations and public text hits.*

#### Figure 1.6: Phase 2 — Hierarchical Entity Mapping
![Figure 1.6](images/2026-05-20-192449.jpg)
*Caption: Sorting primary links into a structured organizational parent framework tree.*

#### Figure 1.7: Phase 3 — Cross-Reference Mapping
![Figure 1.7](images/2026-05-20-193625.jpg)
*Caption: Identifying media and public news asset anchors linked to the core target profiles.*

#### Figure 1.8: Phase 4 — Relationship Interconnection
![Figure 1.8](images/2026-05-20-193916.jpg)
*Caption: Tracking shared infrastructure links bridging distinct entity groups.*

#### Figure 1.9: Phase 5 — Master Structural Verification
![Figure 1.9](images/2026-05-20-194016.jpg)
*Caption: Full-canvas layout tracking complete threat mapping without direct server interaction.*

#### Figure 1.10: Apex Domain Harvesting
![Figure 1.10](images/2026-05-20-194951.jpg)
*Caption: Unmasking structural organization properties and core destination links (`www.marc-clotet.com`).*

#### Figure 1.11: URL Parsing & Schema Resolution
![Figure 1.11](images/2026-05-20-195129.jpg)
*Caption: Programmatically transforming plain text elements into distinct web schema properties.*

#### Figure 1.12: Target Scope Boundary Locking
![Figure 1.12](images/2026-05-20-195353.png)
*Caption: Macro-zoom validation confirming strict target focus parameters on the canvas layout.*

#### Figure 1.13: Social Engineering & Communication Endpoint Mapping
![Figure 1.13](images/2026-05-20-200019.jpg)
*Caption: Extracting public personnel account schemas (`mo@un.com`, `t@ru.com`) to map social engineering attack surfaces.*

#### Figure 1.14: External Relationship Dependencies
![Figure 1.14](images/2026-05-20-200320.jpg)
*Caption: Tracing external links referencing third-party production nodes (`www.formulatv.com`).*

#### Figure 1.15: Geographic Infrastructure Intelligence
![Figure 1.15](images/2026-05-20-201446.jpg)
*Caption: Harvesting regional infrastructure endpoints (`+34 91...` Spanish telecommunication markers).*

#### Figure 1.16: Wayback Machine Historical Analysis Timeline
![Figure 1.16](images/2026-05-20-201510.jpg)
*Caption: Scraping archive snapshots from 2008 to 2014 to isolate legacy directory structures.*

#### Figure 1.17: Final Canvas — Decade-Scale OSINT Canvas
![Figure 1.17](images/2026-05-20-201630.jpg)
*Caption: The finished passive intelligence profile covering ten years of data transitions.*

#### Figure 1.18: Inbound Web Entity Mapping
![Figure 1.18](images/2026-05-20-202149.jpg)
*Caption: Mapping core external dependencies spanning `wikipedia.org`, `variety.com`, and `linkedin.com`.*

#### Figure 1.19: Sub-Layer Content Structure Mapping Tree
![Figure 1.19](images/2026-05-20-203338.png)
*Caption: Separating core routes into Home and About Us metadata blocks.*

#### Figure 1.20: Final Extraction — Funicular Films Mapping Canvas
![Figure 1.20](images/2026-05-20-203528.jpg)
*Caption: Final corporate mapping tracking stakeholders (Marc Clotet, Aina Clotet, Marta Baldó, Jan Andreu) and regional offices (Barcelona, Sweden) up to the recent May 2026 Cannes Film Festival releases.*

---

## Exercise 2.3: Pure Command-Line Terminal Reconnaissance

To validate Maltego's automated outputs, low-level shell diagnostics were executed against `hackthissite.org` using standard query utilities.

#### Figure 1.21: WHOIS Analysis Output
![Figure 1.21](images/2026-05-20-211734.jpg)
*Caption: Running `whois` commands to extract creation indices (2003) and primary DNS routing arrays (Porkbun / buddyns).*

#### Figure 1.22: DNS Information Zone Resolution
![Figure 1.22](images/2026-05-20-211840.png)
*Caption: Executing `dig` to unmask perimeter load-balancing arrays spanning `137.74.187.100` through `.104`.*

#### Figure 1.23: RIR Netblock Allocation Check
![Figure 1.23](images/2026-05-20-212100.jpg)
*Caption: Tracing network ranges to a RIPE NCC allocated /16 network notation structure (`137.74.0.0/16`).*

#### Figure 1.24: Upstream Service Provider Architecture Map
![Figure 1.24](images/2026-05-20-212244.jpg)
*Caption: Isolating physical hosting footprints down to an OVH facility block in Berlin, Germany (DE).*

---

# Unit 3: Active Reconnaissance & Local Subnet Diagnostics

This phase covers setting up local testing infrastructure, profiling sandboxed machines, and testing low-level link parameters.

## Exercise 3.1: Machine Baseline Profiling

#### Figure 2.1: Ubuntu Gateway Node Interface Profile
![Figure 2.1](images/2026-05-20-213617.jpg)
*Caption: Verifying an Ubuntu 26.04 LTS (Resolute Raccoon) environment running a Linux 7.0.0-14 generic kernel structure.*

#### Figure 2.2: Local Kali Linux Attack Platform Verification
![Figure 2.2](images/2026-05-20-213659.png)
*Caption: Verifying a rolling Kali Linux build operating over a Debian 5.16.0 framework.*

#### Figure 2.3: Metasploitable Threat Target Baseline Check
![Figure 2.3](images/2026-05-20-213843.png)
*Caption: Running `uname -a` against Metasploitable to unmask an outdated 32-bit Linux 2.6.24-16 server structure. Standard `os-release` files returned faults.*

#### Figure 2.4: Legacy Release Bypass via Alternative Paths
![Figure 2.4](images/2026-05-20-213952.png)
*Caption: Executing `cat /etc/lsb-release` to bypass system faults and identify the target host as end-of-life Ubuntu 8.04 (Hardy).*

---

## Exercise 3.2: Subnet Interface Mapping

#### Figure 2.5: Deprecated ifconfig Subsystem Error
![Figure 2.5](images/2026-05-20-214025.png)
*Caption: System path shell error during interface query execution due to missing legacy utilities.*

#### Figure 2.6: Local Mirror Net-tools Installation Stream
![Figure 2.6](images/2026-05-20-214042.png)
*Caption: Updating dependencies via `sudo apt install net-tools` to safely restore network interface mapping analysis components.*

#### Figure 2.7: Ubuntu Gateway Configuration Summary
![Figure 2.7](images/2026-05-20-214110.png)
*Caption: Verifying localized gateway interface `ens4` address space parameters at `192.168.122.71`.*

#### Figure 2.8: Kali Linux Attacker Local Config
![Figure 2.8](images/2026-05-20-214152.png)
*Caption: Verifying local attack platform interface `eth0` address parameters at `192.168.122.148`.*

#### Figure 2.9: Metasploitable Target Config
![Figure 2.9](images/2026-05-20-214210.png)
*Caption: Verifying target vulnerability host interface `eth0` address parameters at `192.168.122.108`.*

---

## Exercise 3.3: Link MTU Testing

#### Figure 2.10: Active ICMP Sizing Fragmentation Boundary Test
![Figure 2.10](images/2026-05-20-214443.png)
*Caption: Running `ping -M do -s 1472 192.168.122.108` to enforce the Don't Fragment bit. The 1472-byte payload, combined with the 20-byte IP header and 8-byte ICMP header, validates a 1500-byte frame MTU limit with 0% packet loss.*

---

## Exercise 3.4: Port Scanning & Banner Grabbing

#### Figure 2.11: Nmap Stealth SYN Port Sweep Baseline
![Figure 2.11](images/2026-05-20-214530.jpg)
*Caption: Executing `sudo nmap -sS -Pn 192.168.122.108` to discover 23 open ports, including ports 21 (ftp), 23 (telnet), 1524 (ingreslock), 6667 (irc), and 5900 (vnc).*

#### Figure 2.12: Manual Interactive Socket Banner Grabbing
![Figure 2.12](images/2026-05-20-214757.png)
*Caption: Connecting via `nc -nv 192.168.122.108 21` to force clear-text application identification banners directly from the raw socket.*

#### Figure 2.13: Automated Version Signature Fingerprinting Scan
![Figure 2.13](images/2026-05-20-214948.jpg)
*Caption: Running targeted scanning flags (`-sV`) to programmatically isolate the listening application engine version as `vsftpd 2.3.4`.*

---

# Unit 4: Controlled Exploitation & Automated Auditing

This phase documents targeted vulnerability verification through system exploitation and automated enterprise compliance mapping.

## Exercise 4.1: Weaponized Framework Staging & Privileged System Extraction

#### Figure 3.1: Exploit Module Target Parameter Configuration Staging
![Figure 3.1](images/2026-05-20-215243.png)
*Caption: Selecting `exploit/unix/ftp/vsftpd_234_backdoor` and mapping destination boundaries using `set rhosts 192.168.122.108`.*

#### Figure 3.2: Exploit Parameter Options Verification Panel
![Figure 3.2](images/2026-05-20-220544.jpg)
*Caption: Running `show options` to verify parameter matching configurations prior to execution.*

#### Figure 3.3: Backdoor Exploitation Stream & Root Command Shell Injection
![Figure 3.3](images/2026-05-20-215400.png)
*Caption: Activating the exploit mechanism to trigger the system backdoor on Port 6200. Running `whoami` and `hostname` confirms root administrative ingestion.*

#### Figure 3.4: Core User Account Database Exfiltration (`/etc/passwd`)
![Figure 3.4](images/2026-05-20-215536.jpg)
*Caption: Reading the global account index payload (`cat /etc/passwd`) to extract plain-text user index profiles (msfadmin, postgres, tomcat55).*

#### Figure 3.5: Cryptographic Shadow Password Hash Exfiltration (`/etc/shadow`)
![Figure 3.5](images/2026-05-20-215550.jpg)
*Caption: Extracting protected cryptographic structures (`cat /etc/shadow`), lifting protected local administrative password hashes for downstream cracking reviews.*

#### Figure 3.6: Multi-Command Session Stability Check
![Figure 3.6](images/2026-05-20-215737.png)
*Caption: Executing inline validation flags (`whoami && hostname`) within the spawned shell to verify session stability across active tasks.*

#### Figure 3.7: Inter-Asset Network Routing Validation Trace
![Figure 3.7](images/2026-05-20-215902.png)
*Caption: Pinging back to the gateway from inside the compromised shell to test routing path metrics.*

#### Figure 3.8: Lateral Workspace Profile Index Logs
![Figure 3.8](images/2026-05-20-220744.png)
*Caption: Profiling processes, directory structures, and environment parameters across secondary systems.*

---

## Exercise 4.2: Automated Vulnerability Auditing (Tenable Nessus)

#### Figure 4.1: Debian Package Extraction and Local Cryptographic Integrity Check
![Figure 4.1](images/2026-05-21-202131.jpg)
*Caption: Running `sudo dpkg -i Nessus.deb` to unpack binaries. The log records successful OpenSSL FIPS Known-Answer Tests across AES, SHA, and RSA components.*

#### Figure 4.2: Package Manager Directory Tracking Path Error
![Figure 4.2](images/2026-05-20-220309.png)
*Caption: Installer error indicating a missing binary path due to initializing the session outside the active target Downloads stack.*

#### Figure 4.3: Workspace Path Remediation Verification
![Figure 4.3](images/2026-05-20-220410.png)
*Caption: Updating terminal context via `cd Downloads/` and running `ls` to verify the unextracted zip archive presence.*

#### Figure 4.4: Web Administration GUI Database Initialization Alert
![Figure 4.4](images/2026-05-21-203718.png)
*Caption: Browser view showing the background compilation lock during local signature database indexing.*

#### Figure 4.5: Air-Gapped Offline Licensing Registration Portal
![Figure 4.5](images/2026-05-21-203904.png)
*Caption: Bypassing isolated network blocks by feeding the registration engine a challenge string.*

#### Figure 4.6: Scanner Scope Scoping Definition Panel
![Figure 4.6](images/2026-05-21-205443.png)
*Caption: Restricting active targets explicitly to `192.168.122.108` to enforce ethical authorization boundaries.*

#### Figure 4.7: Real-Time Vulnerability Ingestion Processing Progress Dashboard
![Figure 4.7](images/2026-05-21-205402.png)
*Caption: Tracking live vulnerability discoveries at early completion stages.*

#### Figure 4.8: Nessus Live Severity Finding Index Table
![Figure 4.8](images/2026-05-21-210009.jpg)
*Caption: Prioritized vulnerability table tracking manual verification targets, including UnrealIRCd (10.0) and VNC Default Passwords (10.0).*

#### Figure 4.9: Folder Management Active Multi-Scan Tracking Panel
![Figure 4.9](images/2026-05-21-210419.png)
*Caption: Side-by-side execution monitoring tracking the Common Ports profile and the All Ports profile concurrently.*

#### Figure 4.10: Finalized Common Ports Policy Summary Dashboard
![Figure 4.10](images/2026-05-21-210736.jpg)
*Caption: The scan finished processing in 13 minutes and 4 seconds, identifying 70 total vulnerabilities via an uncredentialed network sweep profile.*

#### Figure 4.11: Finalized All Ports Policy Summary Dashboard
![Figure 4.11](images/2026-05-21-215434.jpg)
*Caption: Expanding the scan scope to all 65,535 ports increased processing duration to 17:41 but successfully uncovered 1 additional Critical vulnerability and 1 additional Medium vulnerability, raising the total threat footprint to 71 vulnerabilities.*

---

# Formal Laboratory Question Responses

## Core Framework Definitions

### CVE (Common Vulnerabilities and Exposures)

CVE acts as a standardized data dictionary that assigns unique tracking identifiers (e.g., CVE-2011-2523) to publicly disclosed security flaws. Its importance lies in providing a universal naming convention across independent security tools, vendor advisors, and remediation logs. This cross-platform consistency ensures that security operations teams can track, discuss, and remediate technical vulnerabilities without translation ambiguities.

### CVSS (Common Vulnerability Scoring System)

CVSS is an open framework that generates a quantitative numerical severity score ranging from 0.0 to 10.0 based on a vulnerability's underlying technical characteristics (attack vector constraints, authentication requirements, data confidentiality impacts). This scoring system allows enterprise security teams to prioritize high-risk critical flaws first, optimizing patch management workloads.

## Post-Exploitation Technical Analysis

### FTP Version Criticality

The specific application version banner (`vsftpd 2.3.4`) was critical because it is tied directly to a documented supply-chain compromise event. In July 2011, the master source archive for this version was altered to include a malicious command delivery mechanism. When an authentication attempt passes specific parameter characters containing a smiley face (`:)`), the daemon instantly forks process execution and opens an unauthenticated listening shell on Port 6200 with complete root administrative privileges. 

### `/etc/passwd` vs `/etc/shadow`

`/etc/passwd` serves as a globally readable system configuration file that indexes basic account metadata, including usernames, local user ID mappings (UID), group ID assignments (GID), and default shell binaries. Conversely, `/etc/shadow` is a highly restricted system storage file accessible only by root administrative accounts. This file contains the actual cryptographic salted password hashes for local users, keeping sensitive authentication records isolated from standard application processes.

### System Compromise Assessment

Successful extraction of both `/etc/passwd` and `/etc/shadow` files demonstrates absolute system compromise. Read access to `/etc/shadow` indicates that the attacker has bypassed all built-in operating system security boundaries and obtained administrative root control. This level of access exposes sensitive system assets to data theft, lateral movement across connected enterprise subnets, and local system credential cracking via offline brute-force tools, requiring an immediate system isolation and remediation response.

---

**Laboratory Completion Date**: May 25, 2026 | **Portfolio Version**: 1.0

*End of Document*
