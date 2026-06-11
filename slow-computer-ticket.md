# Slow Computer Ticket Example

## Overview

This document provides a sample help desk ticket for a slow Windows computer. Slow performance issues are common in desktop support and may be caused by high resource usage, startup apps, low disk space, pending updates, malware, hardware limitations, or user profile issues.

## Ticket Information

| Field | Details |
|---|---|
| Ticket Number | HD-1005 |
| Request Type | Incident |
| Category | Workstation / Performance |
| Priority | Medium |
| Status | Resolved |
| User | Michael Chen |
| Department | Administration |
| Device | DESKTOP-ADM-011 |
| Operating System | Windows 11 |
| Support Role | Desktop Support Technician |

## Issue Summary

User reported that their computer was running slowly after login.

## User Impact

The user experienced delays opening Outlook, Microsoft Teams, browser tabs, and shared documents.

## Initial User Report

```text
User stated the computer was very slow after signing in and applications were taking several minutes to open.
```

## Troubleshooting Questions

- When did the issue start?
- Is the computer slow all day or only after startup?
- Are all applications slow or only one?
- Did the computer recently update?
- Have you restarted recently?
- Are you working with large files?
- Is the issue happening on another device?
- Are other users affected?

## Troubleshooting Steps Performed

```text
1. Confirmed device name and operating system.
2. Checked system uptime in Task Manager.
3. Confirmed computer had not restarted in over 20 days.
4. Reviewed Task Manager for CPU, memory, and disk usage.
5. Found several startup applications using high memory.
6. Checked disk space and confirmed available storage was low.
7. Cleared temporary files using Windows Storage settings.
8. Disabled unnecessary startup applications with user approval.
9. Checked Windows Update and confirmed restart was pending.
10. Restarted the computer.
11. Retested Outlook, Teams, and browser performance.
```

## Useful Commands Used

Check system boot time:

```cmd
systeminfo | find "System Boot Time"
```

Open Task Manager:

```cmd
taskmgr
```

Check disk space:

```cmd
wmic logicaldisk get size,freespace,caption
```

Open Windows Update:

```cmd
control update
```

## Findings

```text
The device had long uptime, low free disk space, multiple high-impact startup apps, and a pending Windows restart.
No signs of a wider network or Microsoft 365 issue were found.
```

## Resolution

```text
Cleared temporary files, disabled unnecessary startup apps, completed pending restart, and confirmed normal application performance after reboot.
```

## Verification

The user confirmed:

- Login was faster
- Outlook opened normally
- Teams launched successfully
- Browser response improved
- No freezing occurred after restart

## Final Ticket Note

```text
User reported slow workstation performance after login.
Checked system uptime and confirmed device had not restarted in over 20 days.
Reviewed Task Manager and found high memory usage from startup applications.
Checked disk space and removed temporary files using Windows Storage settings.
Disabled unnecessary startup apps with user approval.
Completed pending Windows restart.
User confirmed improved performance after reboot.
Ticket resolved.
```

## Escalation Criteria

Escalate if:

- Disk health errors are present
- Malware is detected
- Computer freezes after restart
- User profile appears corrupted
- Hardware upgrade is required
- Multiple users report similar performance issues
- Business-critical application is affected

## Skills Demonstrated

- Windows performance troubleshooting
- Task Manager analysis
- Disk space review
- Startup app management
- Windows Update awareness
- User support documentation
