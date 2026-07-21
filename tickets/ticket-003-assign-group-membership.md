# Ticket #003 - Assign Users to Security Groups

## Request
Assign employees to the appropriate department security groups based on their roles.

## Environment
Windows Server Active Directory Domain Controller

Domain:
lab.local

## Actions Taken
Assigned users to security groups:

Accounting:
- Added Accounting users to Accounting-Users

IT Department:
- Added IT users to IT-Admins

HR Department:
- Added HR users to HR-Users

Sales Department:
- Added Sales users to Sales-Users

Help Desk:
- Added support users to HelpDesk

## Verification
Verified group membership using:

- Security Group Members tab
- User Member Of tab

## Result
Users were successfully assigned to the appropriate security groups.

## Status
Completed
