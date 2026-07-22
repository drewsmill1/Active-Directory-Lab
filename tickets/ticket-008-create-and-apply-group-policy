# Ticket #008 - Create and Apply Group Policy

## Request
Create and apply a Group Policy Object (GPO) to the Workstations Organizational Unit to demonstrate centralized management of domain-joined computers.

## Environment
Windows Server Active Directory Domain Controller

Domain:
lab.local

## Actions Taken
Performed Group Policy configuration:

- Opened Group Policy Management on the Domain Controller.
- Created a new Group Policy Object named **Workstation Security Policy**.
- Linked the Group Policy Object to the **Workstations** Organizational Unit.
- Configured computer security settings within the Group Policy.
- Forced a Group Policy update on the workstation using `gpupdate /force`.
- Verified the policy was successfully applied using `gpresult /r`.

## Verification
Confirmed the **Workstation Security Policy** appeared under **Applied Group Policy Objects** in the Computer Settings section of the `gpresult /r` output.

## Result
The Group Policy Object was successfully created, linked to the Workstations Organizational Unit, and applied to the domain-joined workstation.

## Status
Completed
