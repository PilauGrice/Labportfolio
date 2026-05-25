# Unit 4: Controlled Exploitation, Post-Exploitation & Automated Auditing

## Overview

This phase documents targeted vulnerability verification through system exploitation and automated enterprise compliance mapping.

---

## Exercise 4.1: Weaponized Framework Staging & Privileged System Extraction

### Intelligence Foundation

Using version data collected from nmap (`vsftpd 2.3.4`), the Metasploit console was loaded to execute a prebuilt backdoor verification routine targeting the unpatched FTP engine.

### Supply-Chain Compromise Context

In July 2011, the master source archive for vsftpd 2.3.4 was altered to include a malicious command delivery mechanism. When an authentication attempt passes specific parameter characters containing a smiley face (`':)'`), the daemon instantly forks process execution and opens an unauthenticated listening shell on **Port 6200** with complete root administrative privileges.

### Exploitation Workflow

#### Stage 1: Module Configuration

**Screenshots: 2026-05-20 215243.png through 215346.png**

```
msf> use exploit/unix/ftp/vsftpd_234_backdoor
msf> set rhosts 192.168.122.108
```

**Actions**:
- Select exploit module: `exploit/unix/ftp/vsftpd_234_backdoor`
- Map destination boundaries using `set rhosts 192.168.122.108`

#### Stage 2: Parameter Verification

**Screenshot: 2026-05-20 220544.jpg**

```
msf> show options
```

**Configuration Check**:
- Verifying parameter matching configurations prior to execution
- Confirm all required options are set correctly

#### Stage 3: Exploit Injection & Shell Extraction

**Screenshots: 2026-05-20 215400.png, 215452.png, 215504.png, 215514.png**

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

**Verification**: Running `whoami` and `hostname` confirms **root administrative ingestion**

### Post-Exploitation Data Exfiltration

#### System Account Database Extraction

**Screenshot: 2026-05-20 215536.jpg**

```bash
cat /etc/passwd
```

**Extracted Users**:
- msfadmin
- postgres
- tomcat55
- (and others)

**File Purpose**: Global readable system configuration containing usernames, UID/GID mappings, home directories, and default shell binaries

#### Cryptographic Hash Database Extraction

**Screenshot: 2026-05-20 215550.jpg**

```bash
cat /etc/shadow
```

**Critical Finding**: Successfully lifted protected local administrative **password hashes** for downstream cracking reviews

**File Purpose**: Highly restricted system storage containing salted cryptographic hashes, account expiration flags, and security settings (accessible only by root)

### Session Stability & Verification

#### Multi-Command Access Continuity

**Screenshot: 2026-05-20 215737.png**

```bash
whoami && hostname
```

**Result**: Successful execution confirms session stability across active tasks

#### Network Routing Verification

**Screenshot: 2026-05-20 215902.png**

```bash
ping 192.168.122.71
```

**Result**: Running ping checks from compromised shell back to gateway validates routing path metrics and lateral movement capability

#### Lateral Asset Footprinting

**Screenshots: 2026-05-20 220744.png through 223554.jpg**

**Actions Performed**:
- Profiling processes across secondary systems
- Mapping directory structures
- Harvesting environment parameters
- Identifying lateral movement targets

---

## Exercise 4.2: Automated Vulnerability Auditing (Tenable Nessus)

To compare targeted manual testing with automated auditing, the Tenable Nessus Expert scanner engine was compiled on the Kali Linux platform.

### Installation & Integrity Verification

#### Package Extraction

**Screenshot: 2026-05-21 202131.jpg**

```bash
sudo dpkg -i Nessus.deb
```

**Cryptographic Integrity Checks**:
- OpenSSL FIPS Known-Answer Tests across:
  - **AES** (Advanced Encryption Standard)
  - **SHA** (Secure Hash Algorithm)
  - **RSA** (Rivest-Shamir-Adleman)

#### Dependency Resolution

**Screenshot: 2026-05-20 220309.png**
- Initial package manager directory tracking path error
- Missing binary path due to terminal session initialized outside Downloads stack

**Screenshot: 2026-05-20 220410.png & 220524.png**

```bash
cd Downloads/
ls
sudo dpkg -i Nessus.deb
```

**Solution**: Updated terminal context and verified archive presence before re-running installation

### Web Administration Interface Setup

#### GUI Database Initialization

**Screenshot: 2026-05-21 203718.png**

```
https://192.168.122.148:8834/
```

**Status**: Browser view showing background compilation lock during local signature database indexing

#### Air-Gapped Offline Licensing

**Screenshot: 2026-05-21 203904.png**

**Challenge**: Bypassing isolated network blocks by feeding registration engine a challenge string

```bash
nessuscli fetch --challenge
```

**Workaround**: Generated challenge string for air-gapped offline licensing registration portal

### Scanner Configuration & Scope Definition

#### Target Scope Restriction

**Screenshot: 2026-05-21 205443.png**

```
Target: 192.168.122.108
```

**Action**: Restricting active targets explicitly to enforce authorization boundaries

#### Real-Time Vulnerability Processing

**Screenshots: 2026-05-21 205402.png and 205917.png**

**Status**: Tracking live vulnerability discoveries at early completion stages

### Vulnerability Assessment Results

#### Live Severity Finding Index

**Screenshot: 2026-05-21 210009.jpg**

**Prioritized Vulnerabilities**:
| Vulnerability | CVSS Score | Status |
|---|---|---|
| UnrealIRCd | 10.0 (Critical) | Verified |
| VNC Default Password | 10.0 (Critical) | Verified |
| Samba Badlock | 7.5 (High) | Verified |

---

## Comparative Analysis Matrix: Scanning Policy Trade-offs

Two separate assessment sweeps were executed against the target machine to evaluate scanning policy trade-offs.

### Multi-Scan Tracking Panel

**Screenshot: 2026-05-21 210419.png**

**Configuration**: Side-by-side execution monitoring tracking:
- Common Ports profile (concurrent)
- All Ports profile (concurrent)

### Common Ports Policy Results

**Screenshot: 2026-05-21 210736.jpg**

| Metric | Value |
|--------|-------|
| Duration | 13 minutes 4 seconds |
| Total Vulnerabilities | 70 |
| Critical | 10 |
| High | 6 |
| Medium | 25 |
| Low | 9 |
| Failed Auth | 1 |
| Profile Type | Uncredentialed network sweep |

### All Ports Policy Results

**Screenshot: 2026-05-21 215434.jpg**

| Metric | Value | Change |
|--------|-------|--------|
| Duration | 17 minutes 41 seconds | +35.4% |
| Total Vulnerabilities | 71 | +1 |
| Critical | 11 | +1 |
| High | 6 | — |
| Medium | 26 | +1 |
| Low | 9 | — |
| Failed Auth | 1 | — |

### Key Findings

**Trade-Off Analysis**:
- Expanding scan scope to all 65,535 ports increased processing duration by **35.4%**
- Successfully uncovered **1 additional Critical vulnerability**
- Successfully uncovered **1 additional Medium vulnerability**
- Total threat footprint raised from **70 to 71 vulnerabilities**

**Recommendations**:
- For time-constrained assessments: Common Ports profile acceptable (13 min)
- For comprehensive coverage: All Ports profile justified (18 min, +1 Critical find)
- ROI: ~5 minutes additional scan time yields 1-2 additional vulnerabilities

---

## Key Takeaways

✅ Supply-chain compromises enable trivial privilege escalation  
✅ Successful exploitation grants immediate root access  
✅ Post-exploitation: Access to `/etc/shadow` indicates complete system compromise  
✅ Lateral movement feasible from compromised host  
✅ Automated tools complement manual exploitation findings  
✅ Scanning policy selection balances thoroughness vs. time constraints  
✅ CVSS scoring prioritizes remediation efforts

---

**[← Back: Unit 3](unit3.md)** | **[Home](index.md)** | **[Next: Responses →](responses.md)**
