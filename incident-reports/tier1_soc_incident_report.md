# Security Incident Report — Tier-1 SOC Investigation

## Incident Overview

This report documents a Tier-1 SOC investigation conducted following the detection of suspicious activity on a Windows endpoint monitored by SOAR platform.

The incident involved abnormal PowerShell execution behavior and a registry-based persistence attempt, identified through endpoint telemetry and correlated SIEM alerts.

---

## Detection Summary

- Detection Source: SOAR platform
- Affected Host: Windows 10 Endpoint
- Alert Types:
  - Suspicious PowerShell execution
  - Encoded command usage
  - Registry modification for persistence
- Severity Level: High

Alerts were mapped to relevant MITRE ATT&CK techniques based on observed behavior.

---

## Investigation Actions

The following investigative steps were performed:

1. Reviewed SIEM alert metadata and timestamps
2. Analyzed command-line execution details
3. Validated process lineage and parent-child relationships
4. Examined registry modification events
5. Correlated multiple alerts to confirm incident scope

All findings were validated using endpoint telemetry rather than assumptions.

---

## MITRE ATT&CK Mapping

- T1059.001 — Command and Scripting Interpreter: PowerShell
- T1547.001 — Registry Run Keys / Startup Folder

These techniques indicate potential execution and persistence behavior.

---

## Assessment and Escalation Decision

Based on the confirmed presence of encoded PowerShell execution and persistence-related registry modifications, the incident met escalation criteria beyond Tier-1 triage.

The incident was classified as a confirmed security event requiring further DFIR analysis.

---

## Conclusion

This investigation demonstrates proper Tier-1 SOC procedures, including alert validation, evidence-based analysis, MITRE mapping, and disciplined escalation decision-making.

All actions were documented following professional SOC reporting standards.
