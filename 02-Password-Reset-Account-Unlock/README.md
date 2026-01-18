# Lab 02 – Password Reset & Account Unlock

## Scenario
User forgot their password and could not log into their Windows 11 computer.

## Objective
Reset a forgotten password and restore user access.

## Environment
- OS: Windows 11 Home
- Tools Used: Command Prompt

## Troubleshooting Steps
1. Verified user account existence
2. Simulated login failure
3. Reset password using net user
4. Re-enabled account if locked
5. Verified successful login

## Commands Used
```cmd
net user
net user JohnDoe NewP@ssw0rd123
net user JohnDoe /active:yes
