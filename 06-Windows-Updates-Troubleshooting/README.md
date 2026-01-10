# Windows Update Troubleshooting – Help Desk Lab

## Scenario
Windows updates failing to install.

## Environment
- OS: Windows 11
- Tools: Settings, Services, Troubleshooter

## Troubleshooting Steps
1. Checked update history.
2. Ran Windows Update troubleshooter.
3. Restarted Windows Update service.
4. Rechecked updates.

## Root Cause
Update service temporarily stalled.

## Resolution
Restarted services and resumed updates.

## Skills Demonstrated
- OS maintenance
- Service troubleshooting

## Outcome
Updates installed successfully.
# Lab 06 – Windows Update Troubleshooting

## Scenario
User reports Windows Updates are failing or stuck and updates will not install.

## Objective
Diagnose Windows Update issues and restore update functionality by resetting update components.

## Environment
- OS: Windows 11 Home
- Tools Used: Windows Update Settings, Troubleshooter, Services, Command Prompt

## Troubleshooting Steps
1. Checked Windows Update status and update history
2. Ran Windows Update troubleshooter
3. Restarted update-related services (Windows Update, BITS, Cryptographic Services)
4. Reset update components by renaming SoftwareDistribution and catroot2
5. Rebooted system and verified updates could check/download/install
6. Confirmed results in Update history

## Commands Used
```cmd
net stop wuauserv
net stop bits
net stop cryptsvc
net stop msiserver
ren C:\Windows\SoftwareDistribution SoftwareDistribution.old
ren C:\Windows\System32\catroot2 catroot2.old
net start wuauserv
net start bits
net start cryptsvc
net start msiserver
