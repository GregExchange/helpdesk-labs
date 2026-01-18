# Active Directory & GPO Basics – Help Desk Lab

## Scenario
User account requires management within a domain environment.

## Environment
- OS: Windows Server (conceptual or VM)
- Tools: Active Directory Users & Computers, Group Policy Management

## Tasks Performed
1. Created a user account in AD.
2. Reset and unlocked user password.
3. Moved user to correct OU.
4. Reviewed applied Group Policies.

## Concepts Demonstrated
- Active Directory structure
- Organizational Units (OU)
- Group Policy Objects (GPO)
- Account lifecycle management

## Skills Demonstrated
- AD fundamentals
- GPO awareness
- Enterprise user support

## Outcome
User account properly managed within domain policies.
# Lab 10 – Active Directory & GPO Basics

## Scenario
User account requires management within a domain environment.

## Objective
Create and manage domain users and groups, apply a Group Policy, and verify enforcement on a domain-joined client.

## Environment
- Domain Controller: Windows Server 2022 (DC01)
- Domain: helpdesk.local
- Client: Windows 11 Pro
- Tools: ADUC, Group Policy Management

## Steps Performed
1. Created OU structure
2. Created domain user and security group
3. Added user to group
4. Created and linked a GPO
5. Joined client to domain
6. Applied and verified GPO using gpupdate/gpresult

## Outcome
User account was successfully managed within Active Directory and policies were enforced.

## Skills Demonstrated
- Active Directory user & group management
- OU design
- Group Policy creation and enforcement
- Domain join troubleshooting
