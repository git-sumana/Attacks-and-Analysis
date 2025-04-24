# Incident Report: Email Reported by User as Junk

## Description
Office 365 Security & Compliance reported a suspicious alert with the following details - Threat Name of "Email reported by user as junk", Alert Entity List of Users. The description of the event states that "This alert is triggered when any email message is reported as junk by users."

## Observations
1. User Involved: manually marked an email as “Not Junk”.
2. The email was originally flagged as junk or spam by Microsoft 365 filtering.
3. It may be possible that a phishing email was misclassified by the user, which could lead to future threats if not reviewed.

## Recommendations
1. Check if it was part of a known phishing campaign.
2. Confirm if the user correctly marked the message as not junk. If incorrect, consider notifying the user and providing guidance.
3. Confirm if the sender is trusted and the domain is legitimate.

## Risk Factors
1. **Phishing Threats**: If the email is a phishing attempt, it could lead to credential theft or other malicious activities.
2. **User Misclassification**: Incorrectly marking phishing emails as not junk can lead to similar future emails bypassing spam filters.
3. **Security Breach**: If the sender is not trusted, it could result in a security breach or data compromise.
4. **Increased Vulnerability**: Allowing potentially harmful emails to reach users increases the risk of successful phishing attacks.
