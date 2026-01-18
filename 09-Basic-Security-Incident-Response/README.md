# Lab 09 – Basic Security Incident Response (Pop-ups + Slow System)

## Scenario
User reported pop-ups and slow performance on a Windows 11 computer.

## Objective
Perform basic incident response: contain the issue, identify suspicious causes, scan/remediate, and verify system recovery.

## Environment
- OS: Windows 11 Home
- Tools Used: Windows Security (Defender), Task Manager, Browser Settings (Edge), Installed Apps

## Actions Taken (IR Workflow)
### 1) Containment
- Disconnected from the network to reduce risk while investigating.

### 2) Identification
- Checked browser extensions and blocked pop-ups/redirects.
- Reviewed startup apps for suspicious items.

### 3) Eradication & Remediation
- Updated Defender protection updates.
- Ran Full scan.
- Reviewed Protection History and removed/quarantined any findings.
- Cleared browser cookies/cache.
- Uninstalled suspicious applications if present.

### 4) Recovery
- Reconnected network and verified normal browsing behavior.
- Confirmed improved performance via Task Manager.

## Evidence
Screenshots in `/screenshots` documenting containment, scans, actions taken, and verification.

## Outcome
System was scanned, suspicious settings/apps were removed or ruled out, and performance returned to normal.

## Skills Demonstrated
- Basic incident response process
- Malware and adware troubleshooting
- Defender scanning and remediation
- Browser hardening
- Documentation and verification
