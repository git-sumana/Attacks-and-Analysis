## Description
Triggered when Sophos Endpoint reports the automatic creation of a local user account, which may indicate first-time login or unusual user activity.

## Observations:
1. We have observed the automatic creation of a local user account on the system.
2. This can happen during a first-time login, especially in corporate environments with domain or remote access setups. However, it may also signal unusual or suspicious activity, such as unauthorized user creation by malware or a misconfigured system.

## Recommendations:
1. Kindly verify the newly created local account is expected—such as part of a first-time login by a known user or if it was created without approval.
2. Examine system logs, Sophos alerts, and event viewer data to determine when, how, and by whom the account was created.
3. Use Sophos Endpoint to perform a full malware scan to rule out any malicious activity that may have triggered the account creation.

## Risk Factors:
1. **Potential Data Breach**: Unauthorized account creation can lead to unauthorized access and potential data breaches.
2. **Service Disruption**: Malicious activity may disrupt normal operations and services.
3. **Reputation Damage**: Security incidents can harm the organization's reputation if not addressed promptly.
4. **Financial Loss**: Addressing security breaches and disruptions can incur significant costs.
5. **Regulatory Non-Compliance**: Failing to protect against such threats may result in non-compliance with data protection regulations.
