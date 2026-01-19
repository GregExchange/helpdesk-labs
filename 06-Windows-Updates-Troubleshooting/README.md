# Lab 06 – Windows Update Troubleshooting (Windows 11 Pro)

## Overview
This lab documents troubleshooting a Windows 11 Pro system where Windows Updates were failing or stuck. The issue was resolved by resetting Windows Update components and verifying successful update functionality.

---

## Scenario
User reports Windows Updates are failing, stuck, or will not install.

---

## Objective
Restore Windows Update functionality by diagnosing update issues, resetting update components, and confirming updates can successfully install.

---

## Environment
- **OS:** Windows 11 Pro  
- **Account Type:** Local Administrator  
- **Tools Used:**
  - Windows Update Settings
  - Windows Update Troubleshooter
  - Services
  - Command Prompt

---

## Troubleshooting Summary
- Verified Windows Update status and reviewed Update history  
- Ran Windows Update Troubleshooter  
- Restarted update-related services (Windows Update, BITS, Cryptographic Services)  
- Reset Windows Update components by renaming `SoftwareDistribution` and `catroot2`  
- Rebooted the system  
- Verified updates could check, download, and install successfully  

---

## Commands Used
```bat
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
```

## Root Cause
Corrupted or stuck Windows Update components prevented updates from installing.  
Windows Update initially failed due to VM network configuration preventing internet access. Issue was resolved by correcting the VM’s network adapter settings.

## Notes
This lab was completed in a virtualized environment. Network configuration limitations in the VM initially prevented Windows Update from accessing Microsoft update services.
