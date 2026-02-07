# Forensic Methodology Overview

## Purpose
This document outlines the forensic methodology applied during the DFIR investigation to preserve evidence integrity, support analysis, and enable defensible incident conclusions.

The approach follows industry-accepted DFIR principles and prioritizes volatile evidence collection.

---

## Evidence Handling Principles
- Evidence was collected in a controlled lab environment
- Acquisition followed a memory-first, disk-second strategy
- Cryptographic hashing was used to validate integrity
- Chain of custody documentation was maintained throughout the process

---

## Memory Acquisition
- **Tool Used:** WinPmem
- **Acquisition Type:** Live memory capture
- **Rationale:** Memory contains volatile artifacts such as running processes, command-line arguments, network connections, and injected code that may not persist on disk

Memory acquisition was performed prior to any disk-based collection to minimize evidence loss.

---

## Disk Artifact Collection
Targeted disk acquisition was performed to support timeline reconstruction and persistence analysis.

Artifacts collected included:
- Windows registry hives (SYSTEM, SOFTWARE)
- Prefetch files
- Windows event logs (Security, System, Sysmon Operational)

Full disk imaging was not performed due to scope and relevance considerations.

---

## Memory Analysis
- **Framework Used:** Volatility 3
- **Analysis Focus:**
  - Active and recently executed processes
  - Command-line arguments
  - Parent-child process relationships
  - Network activity visible in memory

Findings were correlated with SIEM alerts to increase confidence in incident determination.

---

## Integrity and Documentation
- Cryptographic hashes were generated for acquired artifacts
- Evidence locations and handling steps were documented
- Analysis limitations were recorded transparently

This methodology supports defensible DFIR conclusions aligned with SOC and incident response best practices.
