# Mission 3 — Understand the operating system

## 1. Task / objective
Explore the operating system, running processes, storage, paths, permissions, and describe what an OS actually does.

## 2. Work completed

### Task 3.1 — Explore the OS
| Information explored | What it tells you | My observation |
|---|---|---|
| OS / system details | Which OS and version is running | macOS, version 27.2.1 |
| Current account identity | Which user account is active | My account (redacted) |
| Available and used storage | How much disk space is free and used | Main disk is 460Gi total, 13Gi used, and 311Gi available |
| System activity snapshot | Running processes, CPU, and memory load | 926 processes total with 3 running, CPU at 4.5% user, 9.45% system, and 86.48% idle |

### Task 3.2 — Processes
A process is just a program currently running on the computer with its own memory and resources. The PID (Process Identifier) is a unique number the OS gives each running process so it can track and manage them separately. Two examples from my snapshot are the shell process running my Terminal session and background system processes like `WindowServer`, which handles the screen and display.
## 3. Commands/Tools Used
sw_vers, whoami, df -h, top -l1, pwd, cd, ls -la

## 4. My Understanding
[In your own words: what the operating system's job is — e.g. managing
hardware resources, running processes, controlling file access/permissions,
and acting as the layer between you and the hardware]

## 5. Difficulties Faced
[Any trouble you had with this mission, or "None" if it went smoothly]

## 6. How I Resolved Them
[Your fix, or "N/A"]

## 7. Evidence/Files
Terminal output from sw_vers, df -h, top -l1, and ls -la commands

## 8. Commit Details
See git log