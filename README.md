# SOC Lab Project 01: Windows Endpoint Monitoring with Sysmon, Wireshark, and Process Monitor

## Project Overview

This project demonstrates a Security Operations Center (SOC) investigation by monitoring Windows endpoint activity using Sysmon, Event Viewer, Process Monitor (ProcMon), and Wireshark.

A Windows 11 virtual machine was configured to generate endpoint telemetry. A PowerShell command (`Test-NetConnection google.com -Port 443`) was executed to simulate network activity. The resulting endpoint logs and network traffic were collected, analyzed, and correlated to demonstrate a typical SOC investigation workflow.

---

## Objectives

- Configure Sysmon for enhanced endpoint logging.
- Monitor Windows process creation.
- Capture outbound HTTPS network traffic.
- Analyze process activity using ProcMon.
- Correlate endpoint logs with packet captures.
- Produce a professional SOC investigation report.

---

## Lab Environment

| Component | Technology |
|----------|------------|
| Operating System | Windows 11 |
| Hypervisor | Oracle VirtualBox |
| Endpoint Monitoring | Sysmon |
| Log Analysis | Windows Event Viewer |
| Packet Capture | Wireshark |
| Process Monitoring | Process Monitor (ProcMon) |
| Command Shell | Windows PowerShell |

---

## Investigation Workflow

1. Configure Sysmon.
2. Launch Windows PowerShell.
3. Execute:
     Test-NetConnection google.com -Port 443
   4. Observe Process Creation (Event ID 1).
5. Observe Network Connection (Event ID 3).
6. Capture HTTPS traffic using Wireshark.
7. Monitor process activity using ProcMon.
8. Correlate collected evidence.

---

## Evidence Collected

- Sysmon Event ID 1 (Process Creation)
- Sysmon Event ID 3 (Network Connection)
- PowerShell command output
- Wireshark HTTPS packet capture
- Process Monitor process activity
- Investigation screenshots
- SOC Investigation Report

---

## MITRE ATT&CK Mapping

| Tactic | Technique | ID |
|---------|-----------|----|
| Execution | PowerShell | T1059.001 |
| Command and Control | Application Layer Protocol | T1071 |
| Discovery | System Network Configuration Discovery | T1016 |

---

## Skills Demonstrated

- Windows Endpoint Monitoring
- Event Log Analysis
- Sysmon
- Wireshark
- Process Monitor
- PowerShell
- Network Traffic Analysis
- Incident Investigation
- Log Correlation
- Technical Documentation

---

## Key Takeaways

This project demonstrates how multiple monitoring tools can be used together to reconstruct endpoint activity and validate network communication, following a workflow commonly performed by Security Operations Center (SOC) analysts.

---

## Author

Akinwunmi Ifedayo

Aspiring SOC Analyst | Computer Engineer | Cybersecurity Enthusiast
