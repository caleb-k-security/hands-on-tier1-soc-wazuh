# Security Incident Report — Tier-1 SOC Investigation

## Incident Overview

This report documents the simulation and validation of automated SOC response workflows built within a SOAR platform.

Instead of investigating a single live incident, this project focused on building, testing, and validating automated response playbooks that activate following SIEM alert ingestion.

Each workflow was tested using simulated high-severity alerts to ensure correct decision-making and controlled automated response.

## Automation Triggers

The SOAR platform received simulated SIEM alerts via webhook integrations representing:

- Suspicious outbound IP activity
- Multiple failed login attempts indicating possible account compromise
- High-confidence phishing email indicators

Each alert was processed through validation logic before any automated action occurred.

## Workflow Validation Steps

The following validation steps were performed during testing:

1. Confirmed webhook ingestion of alert data
2. Verified conditional logic execution
3. Observed simulated containment actions
4. Validated audit logging and SOC notification steps
5. Ensured automation only triggered under high-risk conditions


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

This project demonstrates how SOC investigations can evolve into structured SOAR automation while maintaining oversight, logging, and risk validation.

The workflows reflect real SOC automation practices where actions are controlled, auditable, and based on defined thresholds rather than blind execution.

