
**Description:**
A(n) Office 365 login to the account with ID "xyz", "username" occurred from two different locations (i.e., "Mumbai, Maharashtra, India" and "Taipei, Taipei City, Taiwan"). It is impossible to travel between these two locations with a distance deviation of 3130.48 miles that would require 539.0 seconds with a travel speed of 20908.57 miles/hour. Microsoft Entra ID reported a suspicious alert with the following details - Threat Name of "Anonymous IP address".

**Observations:**
1. We have observed successful login on user from two different geolocations within a short time frame.
2. First login was from (Mumbai, India) IP and second successful login on same user from (Taipei, Taiwan) IP.
3. For the same user, Microsoft Entra ID reported a suspicious alert with the following details - Threat Name of "Anonymous IP address".

**Recommendations:**
1. Kindly verify the legitimacy of the login by reaching out to the user to confirm whether they performed the login or used a VPN/remote access service.
2. If the activity is unknown to the user, reset the user's credentials and, if necessary, disable the account temporarily.
3. Ensure that Multi-Factor Authentication (MFA) is enabled on O365 for the user account to reduce the risk of unauthorized access, especially from unusual locations [1](https://support.microsoft.com/en-us/office/set-up-your-microsoft-365-sign-in-for-multi-factor-authentication-ace1d096-61e5-449b-a875-58eb3d74de14) [2](https://learn.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide).

**Risk Factors:**
1. Potential unauthorized access due to login from unusual locations.
2. Increased risk of account compromise if the user did not perform the logins.
3. Use of anonymous IP addresses indicating possible malicious intent.
