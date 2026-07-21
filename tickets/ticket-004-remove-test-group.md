# Ticket #004 - Remove Temporary Security Group

## Request
Remove an unused temporary security group from Active Directory.

## Environment
Windows Server Active Directory Domain Controller

Domain:
lab.local

## Actions Taken
Created a temporary test group:

- Temp-Project

After confirming the group was no longer needed:

- Removed the test group from Active Directory.

## Verification
Confirmed the group no longer appeared in Active Directory Users and Computers.

## Result
Temporary security group was successfully removed.

## Status
Completed
