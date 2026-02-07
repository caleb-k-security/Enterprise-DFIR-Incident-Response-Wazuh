# Enterprise DFIR Investigation and Incident Response Using Wazuh SIEM and Endpoint Forensics

## Project Overview
This project demonstrates an enterprise-style Digital Forensics and Incident Response (DFIR) investigation conducted within a Security Operations Center (SOC) environment. The objective was to detect, investigate, and escalate a simulated endpoint attack using SIEM telemetry, endpoint visibility, and forensic evidence handling practices aligned with real-world SOC workflows.

The investigation follows a structured SOC lifecycle: baseline validation, alert detection, incident escalation, forensic acquisition, memory analysis, and professional incident documentation.

---

## Objectives
- Validate SOC telemetry and endpoint visibility before incident simulation
- Detect suspicious PowerShell execution and persistence mechanisms
- Correlate alerts using Wazuh SIEM and Sysmon telemetry
- Apply DFIR best practices for evidence preservation and integrity
- Perform memory forensics using Volatility 3
- Document findings in a professional incident response ticket

---

## Environment Architecture
- **Attacker Simulator:** Kali Linux
- **Victim Endpoint:** Windows 10 with Sysmon
- **SIEM / SOC Platform:** Wazuh SIEM
- **Forensic Analysis:** Volatility 3, WinPmem
- **Analyst Role:** SOC Analyst / DFIR Investigator

---

## Investigation Workflow
1. Baseline validation (Sysmon, Wazuh agent, log flow verification)
2. Controlled attack simulation (encoded PowerShell execution)
3. Persistence simulation (registry run key modification)
4. Alert detection and MITRE ATT&CK mapping
5. Incident escalation decision
6. Memory acquisition and integrity hashing
7. Targeted disk artifact collection
8. Memory forensic analysis using Volatility 3
9. Evidence correlation and incident documentation

---

## Key Skills Demonstrated
- SOC alert triage and escalation
- Endpoint telemetry analysis (Sysmon)
- SIEM correlation and investigation (Wazuh)
- DFIR methodology and chain of custody
- Memory acquisition and analysis
- MITRE ATT&CK mapping
- Professional incident reporting

---

## Disclaimer
All activities performed in this project were conducted in an isolated lab environment for educational and defensive security purposes only. No real malware was used, and no production systems were affected.

---

## Author
**Caleb Kimani**  
SOC Analyst (Tier-1) | DFIR Foundations
