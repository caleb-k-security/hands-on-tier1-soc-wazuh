# Hands-On Tier-1 SOC Operations Using Wazuh: Detection, Investigation, and Incident Documentation

## Overview

This project demonstrates hands-on Tier-1 Security Operations Center (SOC) activities using the Wazuh SIEM platform. 
It focuses on alert detection, investigation, evidence validation, and professional incident documentation in a controlled lab environment.

The objective is to replicate real-world SOC workflows, emphasizing accuracy, escalation discipline, and evidence-based analysis.

## SOC Role Alignment

This project aligns with Tier-1 SOC analyst responsibilities, including:

- Monitoring and triaging security alerts
- Investigating endpoint and log-based detections
- Validating suspicious activity using telemetry
- Documenting incidents clearly for escalation
- Mapping detections to MITRE ATT&CK techniques

## Lab Environment

- Wazuh Server (Manager, Indexer, Dashboard)
- Windows 10 endpoint with Wazuh Agent and Sysmon
- Kali Linux (attack simulation)
- Isolated virtualized environment (VirtualBox)

The lab was designed to maintain clear separation between attacker, victim, and monitoring components.

## Detection and Investigation Summary

Security alerts were generated through controlled and non-malicious attack simulations, including:

- Suspicious PowerShell execution
- Encoded command usage
- Registry-based persistence techniques

Each alert was investigated by analyzing:
- Process execution details
- Command-line arguments
- Registry modifications
- Event timestamps and host context

## Evidence and Documentation

This repository includes:

- Incident reports documenting investigation findings
- Screenshots of SIEM alerts and telemetry
- A clear investigation methodology
- Supporting lab configuration notes

All evidence is preserved and organized to reflect real SOC documentation standards.

## Skills Demonstrated

- SIEM monitoring and alert triage
- Endpoint log analysis (Windows & Sysmon)
- Incident documentation and reporting
- MITRE ATT&CK mapping
- Evidence validation and investigation workflow
- Professional SOC communication

## Disclaimer

All activities in this project were conducted in a controlled lab environment for educational and defensive security purposes only.
No real-world systems or data were targeted.
