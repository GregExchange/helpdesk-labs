# User Login & Account Issues – Help Desk Lab

## Scenario
User is unable to log in to their Windows 11 computer.

## Environment
- OS: Windows 11
- Account Type: Local User
- Tools: Settings, Computer Management, Event Viewer

## Troubleshooting Steps
1. Logged in as administrator.
2. Opened Computer Management → Local Users and Groups.
3. Checked if account was disabled or locked.
4. Reset user password.
5. Verified account status.
6. Tested login.

## Root Cause
Account lockout due to repeated incorrect password attempts.

## Resolution
Reset password and confirmed account was enabled.

## Skills Demonstrated
- User account management
- Password reset
- Windows troubleshooting

## Outcome
User successfully logged in.
# Lab 01 – User Login & Account Issues

## Scenario
User was unable to log in to their Windows 11 computer.

## Environment
- OS: Windows 11 Home
- Account Type: Local User
- Tools: Command Prompt

## Issue Identified
User account was disabled.

## Troubleshooting Steps
1. Verified user existence using `net user`
2. Created user account
3. Disabled account to simulate issue
4. Re-enabled account using Command Prompt

## Commands Used
```cmd
net user
net user jdoe Password123 /add
net user jdoe /active:no
net user jdoe /active:yes
## Issue Encountered
User account name contained a space, causing initial command failure.

## Resolution
Used quotation marks around the username to properly execute the command.

Example:
```cmd
net user "John Doe" /active:no
### Issue Encountered
User account did not appear on Windows 11 sign-in screen.

### Root Cause
Windows hides local accounts that have never logged in.

### Resolution
Manually logged in using "Other user" and initialized profile.
### Behavior Observed
When a user account is disabled, Windows removes it from the sign-in screen.

### Reason
Disabled accounts are hidden by design for security purposes.

### Verification Method
Used `net user "John Doe"` to confirm account active status.

### Resolution
Re-enabled account using:
```cmd
net user "John Doe" /active:yes
