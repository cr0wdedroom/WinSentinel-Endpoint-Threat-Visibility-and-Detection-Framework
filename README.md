# WinSentinel-Endpoint-Threat-Visibility-and-Detection-Framework

WinSentinel is a security monitoring framework that integrates modern Windows telemetry tools to provide real-time visibility, detection, and investigation capabilities for endpoint threats in a simulated enterprise environment.
This project demonstrates applied SOC Analyst skills by combining Sysmon, Sysinternals, Windows Event Logs, Osquery, and Wazuh SIEM to monitor, log, detect, and alert on suspicious activity across a Windows 11 VM — with Kali Linux used for simulating attacker behavior.

🛡️Project Objectives:

Build a robust endpoint logging and detection lab

Simulate real-world attacker behavior (recon, persistence, privilege escalation)

Detect anomalies using custom Sysmon rules, Osquery packs, and Wazuh alerts

Showcase core SOC skills: event correlation, telemetry analysis, and alert triage


## Step 1: Wazuh Manager Active Status
Installed the Wazuh Manager on my Kali Linux virtual machine. The Wazuh Manager acts as the central server that collects, analyzes, and stores security data received from various agents.

Installation Summary:

Installed using the official Wazuh repository.

Followed proper setup steps, ensuring all necessary dependencies were met.

Ensured no broken configuration in ossec.conf by validating with xmllint.

Service Activation:

After installation, I started and enabled the Wazuh Manager service and checked the running status.

![Wazuh Manager Active Status](screenshots/wazuh-manager-active-status.png)

## Step 2: Wazuh Manager Port Listening
Wazuh Manager is listening on Port 55000.

![Wazuh Manager Port Listening](screenshots/wazuh-manager-port-listening.png)
