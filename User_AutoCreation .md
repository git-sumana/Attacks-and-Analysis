# Incident Report: Automatic Creation of Local User Account

## Description
Triggered when Sophos Endpoint reports the automatic creation of a local user account, which may indicate first-time login or unusual user activity.

## Observations
1. We have observed the automatic creation of a local user account on the system.
2. This can happen during a first-time login, especially in corporate environments with domain or remote access setups. However, it may also signal unusual or suspicious activity, such as unauthorized user creation by malware or a misconfigured system.

## Recommendations
1. Kindly verify the newly created local account is expected—such as part of a first-time login by a known user or if it was created without approval.
2. Examine system logs, Sophos alerts, and event viewer data to determine when, how, and by whom the account was created.
3. Use Sophos Endpoint to perform a full malware scan to rule out any malicious activity that may have triggered the account creation.

## Risk Factors
1. **Unauthorized Access**: If the account was created by an attacker, it could be used to gain unauthorized access to the system and sensitive data.
2. **Privilege Escalation**: The new account might be used to escalate privileges, allowing the attacker to perform administrative actions.
3. **Persistence**: Attackers could use the account to maintain persistent access to the system, making it harder to detect and remove them.
4. **Data Exfiltration**: The account could be used to exfiltrate data from the system, leading to potential data breaches.
5. **System Misconfiguration**: If the account creation is due to a misconfiguration, it could indicate broader issues with system security settings that need to be addressed.
