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

### Task 3.3 — Paths
A path is the address of a file or folder on the system. An absolute path starts from the root (e.g. `/Users/abc/digital-detective-8053`) and always points to the same place no matter where you currently are. A relative path (e.g. `../mission-03-operating-system`) depends on your current folder, so it means something different depending on where you run it from.

### Task 3.4 — Permissions
Running `ls -la` showed permission strings like `drwxr-xr-x` next to each file and folder. The first character shows the type (`d` for directory, `-` for a regular file), and the next 9 characters are read/write/execute permissions, grouped in threes for the owner, the group, and everyone else.

## 3. Commands/Tools Used
sw_vers, whoami, df -h, top -l1, pwd, cd, ls -la

## 4. My Understanding
The operating system manages the computer's hardware resources — CPU, memory, and storage — and acts as the middleman between the hardware and the programs I run. It keeps track of every running process through its PID, controls who can read, write, or execute each file through permissions, and manages the file system so paths resolve correctly whether absolute or relative.

## 5. Difficulties Faced
None major — this mission mostly involved reading and interpreting output from built-in commands like `top`, `df`, and `ls -la`.

## 6. How I Resolved Them
N/A

## 7. Evidence/Files
Terminal output from sw_vers, df -h, top -l1, and ls -la commands

## 8. Commit Details
See git log