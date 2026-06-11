# Printer Issue Ticket Example

## Overview

This document provides a sample help desk ticket for a printer issue. Printer problems are common in office support environments and may involve print queues, printer drivers, print spooler services, network connectivity, or printer hardware.

## Ticket Information

| Field | Details |
|---|---|
| Ticket Number | HD-1002 |
| Request Type | Incident |
| Category | Printer / Hardware |
| Priority | Medium |
| Status | Resolved |
| User | Aisha Brown |
| Department | Accounting |
| Device | DESKTOP-ACC-022 |
| Printer | Printer-Accounting-Floor2 |
| Support Role | Desktop Support Technician |

## Issue Summary

User was unable to print to the department network printer.

## User Impact

The user could not print invoices and accounting documents required for daily work.

## Initial User Report

```text
User reported that documents were stuck in the print queue and the printer showed as offline in Windows.
```

## Troubleshooting Questions

- What printer are you trying to print to?
- Can other users print to the same printer?
- Is the printer showing any error message?
- Is the printer powered on?
- Are documents stuck in the queue?
- Can you print from another application?
- Did this start today or after a change?

## Troubleshooting Steps Performed

```text
1. Confirmed the affected printer name with the user.
2. Checked printer status in Windows Printers & Scanners.
3. Confirmed printer showed offline on the user's workstation.
4. Verified the physical printer was powered on and had paper.
5. Confirmed no paper jam or toner error was shown on the printer panel.
6. Checked the print queue and found multiple stuck jobs.
7. Cleared stuck print jobs.
8. Restarted the Windows Print Spooler service.
9. Printed a test page successfully.
10. Asked user to print original document again.
```

## Useful Commands Used

Restart print spooler:

```cmd
net stop spooler
net start spooler
```

Open printer settings:

```cmd
control printers
```

Test printer by name or IP address:

```cmd
ping printer-name
ping printer-ip-address
```

## Findings

```text
The printer hardware was online and available.
The issue was caused by stuck jobs in the local Windows print queue.
Restarting the Print Spooler service cleared the issue.
```

## Resolution

```text
Cleared the print queue and restarted the Print Spooler service.
Confirmed successful print test from the user's workstation.
```

## Verification

The user confirmed:

- Test page printed successfully
- Original document printed successfully
- Printer no longer showed offline
- No further print errors appeared

## Final Ticket Note

```text
User reported network printer showing offline and documents stuck in queue.
Verified printer was powered on, connected, and had no physical error.
Checked Windows print queue and found stuck print jobs.
Cleared queue and restarted Print Spooler service.
Printed test page successfully.
User confirmed original document printed normally.
Ticket resolved.
```

## Escalation Criteria

Escalate if:

- Multiple users cannot print
- Printer is unreachable by IP address
- Print server is unavailable
- Printer has a hardware error
- Driver needs admin deployment
- Printer requires vendor maintenance
- Printer is not visible on the network

## Skills Demonstrated

- Printer troubleshooting
- Print queue management
- Print Spooler support
- Network printer testing
- Windows device support
- Ticket documentation
