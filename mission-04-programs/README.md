# Mission 4 — How programs run

## 1. Task / objective
Run a simple Python program and compare how compilers and interpreters translate and execute code.

## 2. Work completed
I created `hello.py` with a one-line `print` statement and ran it using Python 3, which printed `"Hello from Python"` right in the terminal.

| Point | Compiler | Interpreter |
|---|---|---|
| When translation and execution happen | Translates the entire program into machine code before running | Reads and runs instructions one line at a time while the program executes |
| Typical output | A separate executable file | Direct output on the screen, with no separate file created |
| One example | C, C++ | Python |
| One advantage | Runs faster once compiled since all the translation is done upfront | Easier to test and debug because errors show up right away without a build step |

A compiler translates the whole program into machine code before anything runs, which is why languages like C need a separate build step first. Python is interpreted, so when I ran `hello.py`, it read and executed the line on the spot. No extra file got created, and the output appeared immediately.

## 3. Commands/tools used
`python3 hello.py`

## 4. My understanding
Running `hello.py` showed me how quick it is to test code in an interpreted language since I didn't have to compile anything first. It also made the difference between compilers and interpreters much clearer, especially why C requires an extra build step before you can actually run the program.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence/files
`hello.py`

## 8. Commit details
"Compare compilers and interpreters" (pushed to `main`).