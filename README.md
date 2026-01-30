# SOC Analyst Lab – Endpoint Investigation Playbook (Windows)

## Overview
This project simulates the daily activities of a **SOC Level 1 Analyst**, focusing on the monitoring, investigation, and documentation of security incidents in **Windows endpoints**.  
The playbooks were created to standardize the investigation process, support initial incident response, and document findings based on real-world SOC workflows.

## Objectives
- Simulate SOC Level 1 investigation routines
- Analyze Windows security events and Sysmon logs
- Identify suspicious or malicious activity
- Document incidents and response procedures
- Create structured playbooks for repeatable investigations

## Scope
The playbooks focus on **endpoint security monitoring** in Windows environments, covering common attack patterns observed in SOC operations.

## Scenarios Covered
- **Brute Force Authentication Attempts**
  - Analysis of repeated failed login attempts
  - Identification of account lockouts
  - Correlation of Windows Security Event IDs (4625, 4740)

- **Suspicious PowerShell Execution**
  - Detection of abnormal PowerShell activity
  - Analysis of Sysmon Event ID 1
  - Identification of potential malicious command execution

## Tools and Technologies
- Windows Event Viewer
- Sysmon
- Windows Security Logs
- Markdown for documentation

## Investigation Workflow
1. Alert or suspicious event identification
2. Log collection and validation
3. Event correlation and timeline analysis
4. Impact assessment
5. Initial containment or recommended action
6. Incident documentation

## Deliverables
- SOC investigation playbooks
- Incident analysis documentation
- Structured investigation workflows
- Evidence-based conclusions


