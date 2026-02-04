# Incident Report: SSH Unauthorized Login Attempts

## Date Observed
January 04

## Summary
Multiple failed SSH authentication attempts were detected for a non-existent user account, indicating a possible brute-force or credential-stuffing attempt.

## Indicators of Compromise (IOCs)
- Username: testuser
- Service: SSH
- Authentication failures: Multiple
- Source: Localhost (::1) – lab testing environment

## Analysis
The attacker attempted to authenticate using an invalid username. Repeated failures suggest automated or scripted login attempts.

## Impact
No successful unauthorized access was detected.

## Mitigation Recommendations
- Disable password-based SSH authentication
- Enable key-based authentication
- Monitor SSH logs regularly
- Implement fail2ban for brute-force protection
