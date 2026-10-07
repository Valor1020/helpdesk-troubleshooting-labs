# Help Desk & IT Support Troubleshooting Labs

Hands-on IT support labs documenting troubleshooting methodology, incident diagnosis, remediation, verification, and technical documentation across Windows, Linux, networking, and help desk environments.

These labs were created in a virtualized homelab environment to develop practical skills applicable to **Help Desk, Service Desk, Desktop Support, and IT Support** roles.

> **Portfolio Note:** These are hands-on simulated/homelab incidents created for technical training and portfolio development. They do not represent production incidents or real end-user environments.

---

## Incident Portfolio

### [INC-001 — Linux DNS Resolution Failure](./INC-001-DNS-Resolution-Failure)

**Environment:** Ubuntu Linux  
**Focus:** DNS troubleshooting, network configuration, connectivity testing

Investigated a Linux workstation that retained network connectivity but could not resolve domain names. Diagnostic testing isolated the failure to DNS configuration, and normal name resolution was restored and verified.

**Skills demonstrated:**
- Linux networking
- DNS troubleshooting
- `resolvectl`
- `nmcli`
- `ip addr`
- `ip route`
- `ping`
- Network configuration verification

---

### [INC-002 — Windows DNS Resolution Failure](./INC-002-Windows-DNS-Resolution-Failure)

**Environment:** Windows 11  
**Focus:** Windows networking, DNS diagnosis, PowerShell

Investigated a Windows 11 workstation that could reach external IP addresses but could not resolve domain names. Testing separated basic IP connectivity from DNS functionality before configuration was corrected and verified.

**Skills demonstrated:**
- Windows 11 troubleshooting
- TCP/IP fundamentals
- DNS troubleshooting
- `ipconfig`
- `ping`
- `nslookup`
- PowerShell
- `Get-DnsClientServerAddress`
- Post-remediation verification

---

### [INC-003 — Windows 11 Boot Recovery](./INC-003-Windows-11-Boot-Recovery)

**Environment:** Windows 11 / VMware Workstation  
**Focus:** Windows Recovery Environment, boot troubleshooting, system integrity

Recovered a Windows 11 virtual machine that failed to boot normally and entered Automatic Repair. Troubleshooting progressed through WinRE diagnostics, partition identification, filesystem and system-file verification, servicing investigation, Safe Mode isolation, Event Viewer analysis, and repeated normal-boot verification.

The system was successfully restored, but the available evidence did not establish a defensible root cause.

**Skills demonstrated:**
- Windows Recovery Environment
- DiskPart
- CHKDSK
- Offline SFC
- DISM
- BCDEdit
- Safe Mode
- Event Viewer
- Boot troubleshooting
- Evidence-based root cause analysis

---

### [INC-004 — DHCP Failure After Network Driver Update](./INC-004-Spiceworks-DHCP-Driver-Failure)

**Environment:** Windows 11 / VMware Workstation / Spiceworks Cloud Help Desk  
**Focus:** Help desk ticket lifecycle, DHCP/APIPA troubleshooting, driver remediation

Managed a simulated help desk incident from initial user report through diagnosis, remediation, verification, documentation, and closure.

Testing identified an APIPA address after DHCP lease acquisition failed. Isolation testing and change investigation ultimately identified a recently installed Realtek Ethernet driver update as the cause. Rolling back the affected driver restored DHCP and normal network connectivity.

**Skills demonstrated:**
- Spiceworks Cloud Help Desk
- Ticket lifecycle management
- End-user communication
- Incident triage
- DHCP troubleshooting
- APIPA identification
- TCP/IP troubleshooting
- Windows Services
- Device Manager
- Driver rollback
- Known-good substitution testing
- Root cause analysis
- Technical documentation

---

## Troubleshooting Methodology

My labs follow a structured troubleshooting process:

```text
Gather Information
        ↓
Determine Scope
        ↓
Establish a Baseline
        ↓
Form a Hypothesis
        ↓
Test the Hypothesis
        ↓
Isolate the Failure
        ↓
Implement the Least-Disruptive Fix
        ↓
Verify Full Functionality
        ↓
Document Findings and Resolution
```

The objective is not simply to make a problem disappear. Each troubleshooting step should answer a question, eliminate or strengthen a hypothesis, and produce evidence supporting the next decision.

---

## Core Technologies

| Area | Technologies & Tools |
|---|---|
| **Operating Systems** | Windows 11, Ubuntu Linux |
| **Virtualization** | VMware Workstation |
| **Networking** | TCP/IP, DNS, DHCP, APIPA, IPv4 |
| **Windows Tools** | Command Prompt, PowerShell, Device Manager, Services, Event Viewer, WinRE |
| **Recovery Tools** | DiskPart, CHKDSK, SFC, DISM, BCDEdit |
| **Linux Tools** | `ip`, `ping`, `resolvectl`, `nmcli` |
| **Help Desk** | Spiceworks Cloud Help Desk |
| **Documentation** | Incident documentation, troubleshooting notes, root cause analysis, verification |

---

## Troubleshooting Philosophy

**Understand first. Memorize second. Apply always.**

I approach troubleshooting by understanding what each test proves before running it. Commands and tools are useful only when their results help narrow the problem.

A successful technical resolution should answer three questions:

1. **What failed?**
2. **What evidence supports the diagnosis?**
3. **How was normal functionality verified after remediation?**

When the available evidence does not establish a definitive root cause, I document the root cause as undetermined rather than assigning an unsupported explanation.

---

## Current Development

This repository will continue to expand with additional hands-on IT support labs involving:

- Active Directory
- Windows Server
- User and group administration
- Permissions and access troubleshooting
- Microsoft 365 concepts
- PowerShell
- DHCP and DNS services
- Ticketing workflows
- Remote support scenarios
- Hardware and peripheral troubleshooting
- Network troubleshooting

---

## About This Repository

This portfolio documents my progression toward professional IT support and cybersecurity roles by converting technical study into practical troubleshooting experience.

Each incident is designed to demonstrate not only **what commands or tools were used**, but **why they were selected, what the results established, and how the resolution was verified**.
