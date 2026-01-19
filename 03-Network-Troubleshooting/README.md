# Network Troubleshooting – Help Desk Lab

## Scenario
User reports no internet connectivity.

# Lab 03 – Network Troubleshooting

## Scenario
User reported no internet connectivity on Windows 11.

## Objective
Diagnose and restore network connectivity.

## Environment
- OS: Windows 11 Home
- Network: Wi-Fi
- Tools Used: Command Prompt, Network Connections

## Troubleshooting Steps
1. Verified network status
2. Checked IP configuration
3. Tested connectivity with ping
4. Reset network adapter
5. Flushed DNS cache
6. Renewed IP address
7. Verified internet access

## Commands Used
```cmd
ipconfig /all
ping 8.8.8.8
ping google.com
ipconfig /release
ipconfig /renew
ipconfig /flushdns
```

## Root Cause
Corrupted or stuck Windows Update components prevented updates from installing.  
Windows Update initially failed due to VM network configuration preventing internet access. Issue was resolved by correcting the VM’s network adapter settings.

## Notes
This lab was completed in a virtualized environment. Network configuration limitations in the VM initially prevented Windows Update from accessing Microsoft update services.

