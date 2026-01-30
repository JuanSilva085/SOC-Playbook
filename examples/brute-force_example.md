# Brute Force Incident – Example

## Incident Type
Brute Force Authentication Attempt

## Detection
The incident was detected through multiple failed login attempts recorded in Windows Security Logs.

## Evidence
- Event ID 4625 – Failed logon attempts
- Event ID 4740 – Account lockout

### Screenshots
![Event 4625 – Failed Logon](/examples/img/4625.png)
--
![Event 4740 – Account Lockout](/examples/img/4740.png)

## Analysis
Multiple failed authentication attempts were observed within a short time window, leading to an account lockout. The pattern is consistent with a brute force attempt rather than normal user behavior.

## Conclusion
The activity was classified as a brute force authentication attempt.

## Recommended Action
- Monitor the affected account
- Enforce password policy review
- Continue monitoring for similar activity
