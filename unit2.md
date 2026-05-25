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
   - *Screenshot: 2026-05-20 180258.jpg*

2. **Keyserver Cryptographic Token Import Validation**
   - Terminal stdout validating successful keyring signature injection
   - *Screenshot: 2026-05-20 180737.png*

3. **Successful Compilation of stable maltego_4.11**
   - Package unpacking trace verifying absolute library installation parameters
   - *Screenshot: 2026-05-20 180923.jpg*

4. **Java Virtual Machine Environment Runtime Verification**
   - Console trace verifying active memory heap configuration boundaries at `/usr/lib/jvm/java-11-openjdk-amd64`
   - *Screenshot: 2026-05-20 183420.jpg*

---

## Exercise 2.2: Maltego Open-Source Transform Analytics

### Target: Clotet / Funicular Films

A multi-tier open intelligence exploration loop was targeted at personal identifiers (Aina Clotet, Marc Clotet) to expand initial names into corporate entities and infrastructure assets.

### Intelligence Gathering Pipeline

#### Phase 1: Initial Name Phrase Configuration
- **Screenshot: 2026-05-20 190853.jpg** - Initial Name Phrase Phase-I Radial Link Configuration Array
  - Tracking baseline website naming configurations and public text hits

#### Phase 2: Hierarchical Entity Mapping
- **Screenshot: 2026-05-20 192449.jpg** - Hierarchical Entity Tree Pivot Structural Mapping
  - Sorting primary links into a structured organizational parent framework tree

#### Phase 3: Cross-Reference Mapping
- **Screenshot: 2026-05-20 193625.jpg** - Peripheral Web Platform Cross-Reference Mapping Loop
  - Identifying media and public news asset anchors linked to core target profiles

#### Phase 4: Relationship Interconnection
- **Screenshot: 2026-05-20 193916.jpg** - Global Relationship Interconnection Overview Canvas
  - Tracking shared infrastructure links bridging distinct entity groups

#### Phase 5: Master Structural Verification
- **Screenshot: 2026-05-20 194016.jpg** - Master Structural Verification Intelligence Map
  - Full-canvas layout tracking complete threat mapping without direct server interaction

### High-Value Intelligence Extractions

#### Domain & Email Harvesting
- **Screenshot: 2026-05-20 194951.jpg** - High-Value Apex Domain Extraction Pass
  - Communication channels: `esther@paperstreet.es`, `aina@funicularfilms.com`
  - Core destination links: `www.marc-clotet.com`

#### URL Parsing & Schema Resolution
- **Screenshot: 2026-05-20 195129.jpg** - URL Parsing and Application Layer Object Resolution
  - Programmatically transforming plain text elements into distinct web schema properties

#### Target Scope Boundary Locking
- **Screenshot: 2026-05-20 195353.png** - Target Scope Asset Tracking and Boundary Locking
  - Macro-zoom validation confirming strict target focus parameters on the canvas layout

### Social Engineering Surface Mapping

- **Screenshot: 2026-05-20 200019.jpg** - Passive Communication Endpoint Harvesting
  - Extracting public personnel account schemas: `mo@un.com`, `t@ru.com`
  - Mapping social engineering attack surfaces

### External Relationship Dependencies

- **Screenshot: 2026-05-20 200320.jpg** - Media Framework Relationship Dependency Check
  - Tracing external links referencing third-party production nodes (`www.formulatv.com`)

### Geographic & Infrastructure Intelligence

- **Screenshot: 2026-05-20 201446.jpg** - Geographic Asset Anchoring and Phone Registry Scraping
  - Harvesting regional infrastructure endpoints: Spanish telecommunication markers (`+34 91...`)

### Historical Timeline Analysis

- **Screenshot: 2026-05-20 201510.jpg** - Wayback Machine Historical Timeline Fan Grid Allocation
  - Scraping archive snapshots from 2008 to 2014 to isolate legacy directory structures

### Final Intelligence Canvas

- **Screenshot: 2026-05-20 201630.jpg** - Completed Multi-Target Decade-Scale OSINT Canvas
  - The finished passive intelligence profile covering ten years of data transitions

### Inbound Web Entity Mapping (Funicular Films)

- **Screenshot: 2026-05-20 202149.jpg** - Inbound Web Entity Relationship Mapping (Funicular Films Hub)
  - Mapping core external dependencies: `wikipedia.org`, `variety.com`, `linkedin.com`

- **Screenshot: 2026-05-20 203338.png** - Sub-Layer Content Mapping Tree
  - Separating core routes into Home and About Us metadata blocks

- **Screenshot: 2026-05-20 203528.jpg** - Master Funicular Films Structural Extraction Layout
  - Final corporate mapping tracking stakeholders: Marc Clotet, Aina Clotet, Marta Baldo, Jan Andreu
  - Regional offices: Barcelona, Sweden
  - Timeline: Up to May 2026 Cannes Film Festival releases

---

## Exercise 2.3: Pure Command-Line Terminal Reconnaissance

To validate Maltego's automated outputs, low-level shell diagnostics were executed against `hackthissite.org` using standard query utilities.

### WHOIS Domain Registration Analysis

```bash
whois hackthissite.org
```

**Results** - *Screenshot: 2026-05-20 211734.jpg*
- Domain creation index: 2003
- Primary DNS routing arrays: Porkbun / buddyns

### DNS Zone Resolution

```bash
dig hackthissite.org
```

**Results** - *Screenshot: 2026-05-20 211840.png*
- Perimeter load-balancing arrays: `137.74.187.100` through `137.74.187.104`

### RIR Netblock Allocation

```bash
whois 137.74.187.100
```

**Results** - *Screenshot: 2026-05-20 212100.jpg*
- RIPE NCC allocated `/16` network notation: `137.74.0.0/16`

### Upstream Service Provider Architecture

**Results** - *Screenshot: 2026-05-20 212244.jpg*
- Physical hosting footprint: OVH facility block in Berlin, Germany (DE)

---

## Key Takeaways

✅ Automated OSINT tools can rapidly map complex organizational structures  
✅ Historical data provides context for infrastructure evolution  
✅ Multiple intelligence vectors converge to build comprehensive profiles  
✅ CLI tools validate and supplement automated reconnaissance output  
✅ Public registries expose significant infrastructure metadata

**[← Back to Home](index.md)** | **[Next: Unit 3 →](unit3.md)**
