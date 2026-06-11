# Software Installation Ticket Example

## Overview

This document provides a sample help desk ticket for a software installation request. Software installation tickets should confirm approval, licensing, system requirements, installation source, testing, and documentation.

## Ticket Information

| Field | Details |
|---|---|
| Ticket Number | HD-1006 |
| Request Type | Service Request |
| Category | Software |
| Priority | Low / Medium |
| Status | Resolved |
| User | Samantha Wilson |
| Department | Human Resources |
| Device | LAPTOP-HR-007 |
| Software | Approved PDF Editor |
| Support Role | Help Desk Technician |

## Issue Summary

User requested installation of approved PDF editing software.

## User Impact

The user needed the software to edit onboarding forms and HR documents.

## Initial User Request

```text
User requested approved PDF editor installation for HR onboarding documents.
Manager approval was included in the ticket.
```

## Approval and License Check

Before installation, confirm:

- Software is approved by IT
- Manager approval is provided, if required
- License is available
- Device meets system requirements
- Installation source is trusted
- User is authorized to use the application

## Troubleshooting / Fulfillment Questions

- What software do you need installed?
- What device should it be installed on?
- Is this software already approved?
- Is a license assigned?
- Is there a business reason?
- Is this needed urgently?
- Are you onsite or remote?
- Should installation be done during a specific time?

## Steps Performed

```text
1. Reviewed software installation request.
2. Confirmed manager approval was attached to the ticket.
3. Verified software was listed as approved.
4. Confirmed available license assignment.
5. Checked device name and operating system.
6. Checked disk space and confirmed enough free space.
7. Downloaded installer from approved company source.
8. Installed software using admin credentials through approved process.
9. Activated license under the user's account.
10. Opened software and completed launch test.
11. Confirmed user could open and edit a test PDF.
```

## Useful Commands Used

Check system information:

```cmd
systeminfo
```

Check disk space:

```cmd
wmic logicaldisk get size,freespace,caption
```

Open installed programs:

```cmd
appwiz.cpl
```

Example MSI installation command:

```cmd
msiexec /i software.msi
```

Example silent install command:

```cmd
msiexec /i software.msi /quiet /norestart
```

## Findings

```text
The device met the software requirements and had enough disk space.
The software was approved and a license was available.
No installation errors occurred.
```

## Resolution

```text
Installed approved PDF editing software and activated assigned license.
Confirmed the user could launch the software and edit a test PDF.
```

## Verification

The user confirmed:

- Software opened successfully
- License was activated
- Test PDF opened
- Edit and save functions worked
- Desktop shortcut was available, if needed

## Final Ticket Note

```text
Reviewed software installation request for approved PDF editor.
Confirmed manager approval, license availability, and device compatibility.
Installed software from approved company source using standard installation process.
Activated license under user's account.
Tested application launch and confirmed PDF editing worked successfully.
User verified software is working.
Ticket resolved.
```

## Escalation Criteria

Escalate if:

- Software is not approved
- License is unavailable
- Admin rights are required outside standard process
- Security tools block installer
- Installation fails repeatedly
- Application requires advanced configuration
- Software may create compliance or security concerns

## Security Best Practices

- Install only approved software.
- Use trusted installation sources.
- Do not give users local admin rights unless approved.
- Confirm license compliance.
- Avoid unknown third-party download sites.
- Document software name and version.
- Escalate blocked or suspicious installers.

## Skills Demonstrated

- Software installation support
- License and approval review
- Windows application setup
- System requirement checks
- Security-aware support
- Ticket documentation
