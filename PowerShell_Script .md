# Incident Report: Suspicious PowerShell Script Execution

## Description
A suspicious PowerShell script was executed on the host by the user. This detection was triggered by a rule with the following description: "Detects technique used by MAZE ransomware to enumerate directories using PowerShell."

## Observations
1. We have observed PowerShell scripts related to Microsoft Defender for Endpoint on the above-mentioned host.
2. Based on its file path and naming convention, `filename` is likely a utility script used during the deployment and configuration of the MDE agent on Windows servers managed by Azure Defender for Servers.
3. Event ID 4104 in the Windows event log indicates PowerShell Script Block Logging. It logs the execution of PowerShell script blocks.

## Recommendations
1. Kindly check the legitimacy of these PowerShell script executions on the server mentioned above.
2. If the script is legitimate for Azure Defender for the mentioned server, kindly let us know so that we can whitelist this activity on Stellar Cyber.
3. In case of unknown scripts on these servers, isolate the host from the network, quarantine the scripts, disable PowerShell execution, and check for the entry points of them.

## Risk Factors
1. If the script runs with system-level privileges, it can be leveraged by attackers to gain elevated access.
2. An attacker could alter the script to disable or weaken security agent behavior.
