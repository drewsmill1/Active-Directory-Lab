# Ticket #005 - Reset User Password

## Request
Reset a user's Active Directory password after the user reported being unable to access their account.

## Environment
Windows Server Active Directory Domain Controller

Domain:
lab.local

## Actions Taken
Performed password reset:

- Located user account in Active Directory Users and Computers.
- Selected Reset Password.
- Created a temporary password.
- Enabled "User must change password at next logon."

## Verification
Confirmed the password reset was successfully applied to the user account.

## Result
User account credentials were successfully updated.

## Status
Completed
