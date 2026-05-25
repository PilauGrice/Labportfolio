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

1. **APT Package Manager Keyring Error Verification**
   - System diagnostic logs tracking authentication blocks during repository indexing initialization
   - ![APT Keyring Error](images/2026-05-20-180258.jpg)

2. **Keyserver Cryptographic Token Import Validation**
   - Terminal stdout validating successful keyring signature injection
   - ![Keyserver Token Import](images/2026-05-20-180737.png)

3. **Successful Compilation of stable maltego_4.11**
   - Package unpacking trace verifying absolute library installation parameters
   - ![Maltego Compilation](images/2026-05-20-180923.jpg)

4. **Java Virtual Machine Environment Runtime Verification**
   - Console trace verifying active memory heap configuration boundaries at `/usr/lib/jvm/java-11-openjdk-amd64`
   - ![JVM Environment](images/2026-05-20-183420.jpg)

---

## Exercise 2.2: Maltego Open-Source Transform Analytics

### Target: Clotet / Funicular Films

A multi-tier open intelligence exploration loop was targeted at personal identifiers (Aina Clotet, Marc Clotet) to expand initial names into corporate entities and infrastructure assets.

### Intelligence Gathering Pipeline

#### Phase 1: Initial Name Phrase Configuration
- ![Initial Name Phrase](images/2026-05-20-190853.jpg) - Tracking baseline website naming configurations and public text hits

#### Phase 2: Hierarchical Entity Mapping
- ![Hierarchical Entity Tree](images/2026-05-20-192449.jpg) - Sorting primary links into a structured organizational parent framework tree

#### Phase 3: Cross-Reference Mapping
- ![Cross-Reference Mapping](images/2026-05-20-193625.jpg) - Identifying media and public news asset anchors linked to core target profiles

#### Phase 4: Relationship Interconnection
- ![Relationship Interconnection](images/2026-05-20-193916.jpg) - Tracking shared infrastructure links bridging distinct entity groups

#### Phase 5: Master Structural Verification
- ![Master Structural Verification](images/2026-05-20-194016.jpg) - Full-canvas layout tracking complete threat mapping without direct server interaction

### High-Value Intelligence Extractions

#### Domain & Email Harvesting
- ![Apex Domain Extraction](images/2026-05-20-194951.jpg) - High-Value Apex Domain Extraction Pass
  - Communication channels: `esther@paperstreet.es`, `aina@funicularfilms.com`
  - Core destination links: `www.marc-clotet.com`

#### URL Parsing & Schema Resolution
- ![URL Parsing](images/2026-05-20-195129.jpg) - Programmatically transforming plain text elements into distinct web schema properties

#### Target Scope Boundary Locking
- ![Target Scope Locking](images/2026-05-20-195353.png) - Macro-zoom validation confirming strict target focus parameters

### Social Engineering Surface Mapping
- ![Passive Communication Endpoint](images/2026-05-20-200019.jpg) - Extracting public personnel account schemas: `mo@un.com`, `t@ru.com`

### External Relationship Dependencies
- ![Media Framework Dependencies](images/2026-05-20-200320.jpg) - Tracing external links referencing third-party production nodes (`www.formulatv.com`)

### Geographic & Infrastructure Intelligence
- ![Geographic Asset Anchoring](images/2026-05-20-201446.jpg) - Harvesting regional infrastructure endpoints: Spanish telecommunication markers (`+34 91...`)

### Historical Timeline Analysis
- ![Wayback Machine Timeline](images/2026-05-20-201510.jpg) - Scraping archive snapshots from 2008 to 2014 to isolate legacy directory structures

### Final Intelligence Canvas
- ![Decade-Scale OSINT Canvas](images/2026-05-20-201630.jpg) - Completed multi-target decade-scale OSINT canvas covering ten years of data transitions

### Inbound Web Entity Mapping (Funicular Films)
- ![Inbound Entity Mapping](images/2026-05-20-202149.jpg) - Mapping core external dependencies: `wikipedia.org`, `variety.com`, `linkedin.com`
- ![Sub-Layer Content Mapping](images/2026-05-20-203338.png) - Separating core routes into Home and About Us metadata blocks
- ![Funicular Films Extraction](images/2026-05-20-203528.jpg) - Final corporate mapping tracking stakeholders: Marc Clotet, Aina Clotet, Marta Baldo, Jan Andreu; Regional offices: Barcelona, Sweden

---

## Exercise 2.3: Pure Command-Line Terminal Reconnaissance

To validate Maltego's automated outputs, low-level shell diagnostics were executed against `hackthissite.org` using standard query utilities.

### WHOIS Domain Registration Analysis

```bash
whois hackthissite.org
```

**Results** - ![WHOIS Domain Info](images/2026-05-20-211734.jpg)
- Domain creation index: 2003
- Primary DNS routing arrays: Porkbun / buddyns

### DNS Zone Resolution

```bash
dig hackthissite.org
```

**Results** - ![DNS Zone Info](images/2026-05-20-211840.png)
- Perimeter load-balancing arrays: `137.74.187.100` through `137.74.187.104`

### RIR Netblock Allocation

```bash
whois 137.74.187.100
```

**Results** - ![RIR Netblock](images/2026-05-20-212100.jpg)
- RIPE NCC allocated `/16` network notation: `137.74.0.0/16`

### Upstream Service Provider Architecture

**Results** - ![Service Provider Architecture](images/2026-05-20-212244.jpg)
- Physical hosting footprint: OVH facility block in Berlin, Germany (DE)

---

## Key Takeaways

✅ Automated OSINT tools can rapidly map complex organizational structures  
✅ Historical data provides context for infrastructure evolution  
✅ Multiple intelligence vectors converge to build comprehensive profiles  
✅ CLI tools validate and supplement automated reconnaissance output  
✅ Public registries expose significant infrastructure metadata

**[← Back to Home](index.md)** | **[Next: Unit 3 →](unit3.md)**
