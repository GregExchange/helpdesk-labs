# Lab 04 – Printer Issues (Windows 11 Pro)

## Scenario
User reports documents are not printing and print jobs appear stuck or paused.

## Objective
Restore printer functionality by diagnosing printer status, restarting the Print Spooler, clearing stuck print jobs, and confirming successful printing.

## Environment
- OS: Windows 11 Pro
- Account Type: Local User (Tier 1)
- Account Type: Administrator (Tier 2)
- Tools Used: Settings, Print Queue, Services (Print Spooler)

## Troubleshooting Steps

### Tier 1 – User Actions
1. Verified printer power and connection
2. Confirmed correct printer was selected
3. Identified paused printer / stuck print jobs
4. Attempted test print and confirmed failure

### Tier 2 – Administrator Actions
5. Restarted the Print Spooler service
6. Cleared stuck print queue
7. Verified printer status returned to Ready
8. Printed test document successfully

## Resolution
The issue was caused by a stalled Print Spooler service and stuck print jobs. Restarting the service and clearing the queue restored printing functionality.

## Evidence
Screenshots included:
- Printer queue showing stuck jobs
- Print Spooler service restart
- Printer status restored
- Successful test print
