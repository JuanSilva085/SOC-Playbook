# Suspicious PowerShell Execution – Example

## Incident Type
Suspicious PowerShell Activity

## Detection
Suspicious PowerShell execution identified through Sysmon logs.

## Evidence
- Sysmon Event ID 1 – Process creation

## Analysis
PowerShell was executed with uncommon parameters, which may indicate malicious or unauthorized activity.

## Conclusion
The activity was classified as suspicious and requires further monitoring.

## Recommended Action
- Review executed command
- Monitor host activity
- Escalate if additional indicators are observed
