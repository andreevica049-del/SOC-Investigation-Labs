# SOC Investigation Labs — Cybersecurity Portfolio

### Practical SOC Analyst Tier 1 | SIEM | Threat Hunting | Incident Investigation

**Completed by:** Andrii Hurskykh  
**Date:** September 2026  
**Field:** Cybersecurity / Security Operations Center (SOC)  
**Lab Platform:** TryHackMe

---

## Project Overview

This repository contains five cybersecurity laboratory reports covering security monitoring, log analysis, threat detection, and incident investigation across Windows, Linux, and network environments.

The laboratories explore practical Security Operations Center (SOC) workflows using Wazuh-related operating system security concepts, Splunk SIEM, Elastic Stack (ELK), Windows Event Viewer, Sysmon, and Linux command-line tools.

The investigations focus on detecting suspicious authentication activity, examining malicious processes, identifying network reconnaissance, investigating potential security incidents, and interpreting indicators of compromise (IOCs).

These labs provide practical exposure to techniques relevant to SOC Analyst Tier 1 and entry-level cybersecurity roles.

## Laboratory Reports

### 1. Linux Logging for SOC — Incident Investigation

**Platform:** Linux  
**Tools:** Linux authentication logs, auditd, Bash, SSH  
**Focus:** SSH authentication monitoring and Linux security investigation

This laboratory focuses on investigating suspicious activity using Linux authentication, system, and audit logs.

**Key Investigation Areas:**
- SSH brute-force and repeated authentication failures.
- Successful SSH authentication following failed attempts.
- Suspicious sudo activity and privilege escalation.
- Unauthorized user account creation.
- Analysis of suspicious process execution using auditd.
- Investigation of Bash command history.
- Reconstruction of attacker activity and identification of IOCs.

**Skills:** Linux Log Analysis, SSH Security, Privilege Escalation Investigation, Threat Hunting, Incident Reporting.

**Report:** [Linux Logging PDF](Linux%20Logging.pdf)

### 2. Windows Logging for SOC — Incident Investigation

**Platform:** Windows  
**Tools:** Windows Event Viewer, Sysmon, PowerShell  
**Focus:** Windows authentication monitoring and incident investigation

This laboratory investigates suspicious Windows authentication events and endpoint activity to reconstruct potential attacker behavior.

**Key Investigation Areas:**
- Failed Windows logins (Event ID 4625).
- Successful RDP authentication (Event ID 4624).
- Correlation of authentication sessions.
- Unauthorized account creation (Event ID 4720).
- Privileged group modifications (Event ID 4732).
- Suspicious process and network activity using Sysmon.
- PowerShell command history analysis.
- Detection of persistence and command-and-control indicators.

**Skills:** Windows Event Log Analysis, Sysmon, RDP Investigation, PowerShell Analysis, Incident Timeline Reconstruction.

**Report:** [Windows Logging PDF](Windows%20Logging.pdf)

### 3. Windows Threat Detection 1 — Incident Investigation

**Platform:** Windows  
**Tools:** Windows Security Logs, Sysmon, Windows Event Viewer  
**Focus:** Initial Access detection and endpoint threat investigation

This laboratory investigates several Initial Access techniques and suspicious Windows endpoint activities.

**Key Investigation Areas:**
- RDP brute-force attacks and successful remote authentication.
- Phishing-related malicious shortcut (LNK) execution.
- Suspicious file downloads and payload execution.
- Process creation and network communication analysis.
- Investigation of malicious activity originating from USB devices.
- Detection of potential malware propagation.
- Identification of suspicious network indicators.

**Skills:** Initial Access Investigation, Phishing Analysis, Malware Detection, Endpoint Monitoring, Threat Hunting.

**Report:** [Windows Threat Detection PDF](Windows%20Threat%20Detection.pdf)

### 4. Network Security Essentials — SOC Investigation

**Platform:** Splunk Enterprise  
**Tools:** Splunk SIEM, Search Processing Language (SPL)  
**Focus:** Network security monitoring and threat hunting

This laboratory demonstrates a structured approach to investigating network security events using Splunk SIEM.

**Key Investigation Areas:**
- Initial SIEM log visibility and source identification.
- Filtering network events by sourcetype.
- Investigation of blocked firewall connections.
- Analysis of VPN authentication activity.
- Detection of potentially suspicious service account logins.
- Investigation of IDS alerts involving possible C2 beaconing and data exfiltration.
- Correlation of firewall, VPN, and IDS evidence.

**Skills:** Splunk SPL, SIEM Investigation, Firewall Log Analysis, VPN Monitoring, IDS Alert Analysis, Threat Correlation.

**Report:** [Network Security Essentials PDF](Network%20Security%20Essentials.pdf)

### 5. Network Discovery Detection — SOC Investigation

**Platform:** Elastic Stack (ELK)  
**Tools:** Elasticsearch, Kibana, Linux CLI, awk  
**Focus:** Network reconnaissance and host discovery detection

This laboratory focuses on detecting potential network reconnaissance activity through SIEM analysis and command-line log examination.

**Key Investigation Areas:**
- Network log exploration using Kibana.
- Identification of unusual network traffic patterns.
- ICMP traffic filtering and host discovery analysis.
- Detection of repeated probing against multiple IP addresses.
- Raw log analysis using Linux command-line tools.
- Identification of possible automated network scanning.
- Mapping observed behavior to MITRE ATT&CK techniques.

**Skills:** Elastic SIEM, Kibana, Network Traffic Analysis, ICMP Monitoring, Log Forensics, Reconnaissance Detection.

**Report:** [Network Discovery Detection PDF](Network%20Discovery.pdf)

---

## Technologies and Skills

| Category | Technologies / Skills |
|---|---|
| SIEM Platforms | Splunk Enterprise, Elastic Stack (ELK) |
| Operating Systems | Windows, Linux |
| Log Analysis | Windows Event Logs, Sysmon, Linux auth logs, auditd |
| Network Security | TCP/IP, SSH, RDP, ICMP, VPN, Firewall Logs |
| Threat Detection | Authentication attacks, phishing, malicious execution, network reconnaissance |
| Investigation | Security event correlation, IOC identification, incident timelines |
| Frameworks | MITRE ATT&CK |
| Scripting & Queries | PowerShell, Linux CLI, Splunk SPL |

## SOC Investigation Methodology

The laboratory reports follow a structured investigation approach:

1. **Log Collection and Visibility** — Identify available security data and log sources.
2. **Event Filtering** — Narrow the investigation to relevant authentication, endpoint, or network activity.
3. **Suspicious Activity Identification** — Examine events that may indicate malicious behavior.
4. **Event Correlation** — Compare related security events, timestamps, accounts, processes, and network indicators.
5. **Threat Assessment** — Evaluate potential risks and map observed activity to relevant attack techniques.
6. **Incident Documentation** — Record findings, supporting evidence, conclusions, and recommended mitigation measures.

## Learning Outcomes

These laboratories cover foundational SOC investigation activities, including:

- Analyzing security alerts from multiple operating systems.
- Investigating suspicious Windows and Linux authentication activity.
- Using SIEM tools to search and filter security logs.
- Detecting potential network reconnaissance and Initial Access activity.
- Examining endpoint processes and suspicious network connections.
- Recognizing indicators of compromise.
- Documenting investigation findings in structured technical reports.

## Additional Cybersecurity Project

**Bachelor's Thesis: Detecting Suspicious Logins in Windows and Linux Using Wazuh**

A separate cybersecurity project focused on deploying Wazuh in a controlled Windows and Linux laboratory environment, collecting authentication events, and evaluating suspicious login detection.

The thesis complements these SOC investigation exercises by examining SIEM implementation, Windows authentication events, Linux SSH logs, and Wazuh alert analysis.

## Acknowledgments

The laboratory exercises are based on TryHackMe cybersecurity training environments.

The investigation report materials were adapted from the [SOC Investigation Labs repository by Majd Mashaleh](https://github.com/MajdMashaleh/SOC-Investigation-Labs).

Original training content and third-party materials remain the property of their respective authors.

---

**Andrii Hurskykh**  
Information Technology Student  
Metropolia University of Applied Sciences  
Helsinki, Finland

**Career Interests:** SOC Analyst Tier 1 | Junior Cybersecurity Analyst | Security Operations | Threat Detection
