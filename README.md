# SOC Endpoint Investigation Playbook

This repository contains a SOC-style playbook designed to guide the
investigation of common suspicious activities on Windows endpoints.

The playbook covers multiple scenarios, including authentication
abuse and suspicious PowerShell execution, based on real-world SOC
workflows and simulated incidents.


## Scenarios Covered
- **Suspicious PowerShell Execution:** Investigation of Base64 encoded commands.
- **Authentication Abuse:** Detection and analysis of Brute Force attempts (Event ID 4625).

## Tech Stack
- **Telemetry:** Microsoft Sysmon
- **Analysis:** Windows Event Viewer (XML Analysis)
- **Documentation:** Markdown & VS Code