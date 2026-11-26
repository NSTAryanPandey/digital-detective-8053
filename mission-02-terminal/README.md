# Mission 2 — Become comfortable with the Terminal

## 1. Task / objective
Practise basic terminal commands, safe file management, flags and pipes, and understand how package managers work.

## 2. Work completed

### Task 2.1 — Basic operations
| Operation | Command | What I observed |
|---|---|---|
| Current-directory display | `pwd` | Showed the full path to the folder I was currently in. |
| Directory listing | `ls` | Listed the visible files and folders in my current directory. |
| Detailed listing | `ls -la` | Showed permissions, owner, file size, and dates for every item, including hidden files. |
| Change directory | `cd ..` / `cd digital-detective-8053` | Moved up one folder and then back in. I ran `pwd` each time to make sure I was in the right place. |
| Create directory | `mkdir terminal-practice` | Created a new empty folder named `terminal-practice`. |
| Create empty file | `touch notes.txt` | Created `notes.txt` with 0 bytes. |
| Copy file | `cp notes.txt notes_backup.txt` | Made a duplicate copy while leaving `notes.txt` unchanged. |
| Move/rename file | `mv notes_backup.txt notes_backup_renamed.txt` | Renamed the backup file, and the original `notes.txt` stayed intact. |
| Display file contents | `cat notes.txt` | Printed the file's contents, which came out empty since I hadn't added any text yet. |

### Task 2.2 — Safe file changes
- **Overwriting vs. appending (`>` vs. `>>`):** Using `>` replaces everything already inside a file, so the old content gets wiped. Using `>>` just adds new text at the end without deleting what's already there.
- **Copying vs. moving (`cp` vs. `mv`):** Copying keeps both the original and the duplicate, while moving shifts or renames the file so you only end up with one.
- **Why `pwd` is useful:** It lets me double-check my exact folder location before running any command that changes or deletes files.
- **Why `ls -la` is useful:** It shows hidden files, permissions, and exact file sizes that a normal `ls` command misses.

### Task 2.3 — Flags and pipes
When I ran `ls -la` and `ls -lh` inside `terminal-practice`, both showed the exact same files, except `-h` displayed sizes in a readable format like `0B` instead of raw bytes. Then I ran `ls -la | head -5` to pipe that detailed listing into `head`, which cut the output down to just the first 5 lines. Basically, the pipe (`|`) takes whatever the command on the left outputs and sends it straight to the command on the right as input.

### Task 2.4 — Package managers
Homebrew is installed on my system (version 7.0.12). A package manager handles installing, updating, and removing software from the command line so I don't have to manually download and set up each tool. It also takes care of dependencies automatically, which saves time and keeps tools from breaking each other.

## 3. Commands/tools used
`pwd`, `ls`, `ls -la`, `ls -lh`, `cd`, `mkdir`, `touch`, `cp`, `mv`, `cat`, `head`, `brew --version`

## 4. My understanding
This mission helped me get way more comfortable navigating folders and handling files directly in the terminal instead of relying on Finder. I also understood how flags change a command's output and how pipes let me connect simple commands together. Checking `pwd` and `ls` before making edits is a good habit so I don't accidentally mess up files in the wrong folder.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence/files
`terminal-practice/` folder with `notes.txt` and `notes_backup_renamed.txt`.

## 8. Commit details
"Complete Terminal and file management mission" (pushed to `main`).