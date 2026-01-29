# Suspicious Activity – SOC Playbook

## Objective

To provide a standardized investigation procedure for common suspicious activities on Windows endpoints.

## Scope

This procedures manual applies to alerts related to:

- Authentication abuse
- Suspicious PowerShell execution

## Data Sources

- Windows Security Event Logs
- Sysmon Operational Logs

---

## General Investigation Workflow

1. Analyze alerts in chronological order
2. Identify the affected endpoint and user
3. Validate the alert's legitimacy
4. Collect relevant logs
5. Determine the type and severity of the incident

---

## Scenario 1 – Brute Force Authentication

### Trigger

Multiple failed logon attempts for the same user within a short period of time.

### Investigation Steps

1. Analyze events ID 4625 in chronological order
2. Identify the target user account
3. Verify if there were successful logins (ID 4624)
4. Assess the period and frequency of attempts
5. Check for account lockout events (Event ID 4740)


### Decision

- Only a few failures → Brute force attempt failed
- Multiple failed attempts followed by success → Possible compromise

### Escalation Criteria

- Successful login after multiple failures
- Target privileged account

---

## Scenario 2 – Suspicious PowerShell Execution

### Trigger

Suspicious PowerShell execution detected via Sysmon.

### Investigation Steps

1. Analyze Sysmon event ID 1
2. Identify the parent process
3. Analyze command-line arguments
4. Decode encoded or obfuscated content, if present

### Decision

- Legitimate administrative activity → Close as benign
- Obfuscated or malicious behavior → Escalate the incident

### Escalation Criteria

- Malicious payload identified
- Persistence mechanisms detected

---

## Documentation & Closing

- Incident summary
- Timeline of events
- Findings and results
- Final classification (TP / FP)
- Resolution actions (e.g., password reset, host isolation)
