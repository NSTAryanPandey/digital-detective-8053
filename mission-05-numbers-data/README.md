# Mission 5: Numbers and Data

## 1. Mission Title
Numbers and Data — Binary, Hexadecimal, and Encoding

## 2. Task/Objective
Practise converting numbers between decimal, binary, and hexadecimal by hand, verify the results using Python, build a simple converter script, and understand how computers encode text as numbers.

## 3. Work Completed
- Hand-converted 7 numbers between decimal, binary, and hexadecimal.
- Verified each hand calculation in Python using `bin()`, `int()`, and `hex()`.
- Built `number_converter.py`, which takes a decimal number as input and prints its binary and hex values.
- Tested the converter program with 3 different inputs (`42`, `100`, and `225`).
- Checked how text characters map to numeric ASCII values (for example, `'A'` is `65` in decimal, or `01000001` in binary) so computers can store text as numbers.

## 4. Hand Calculations
- **13 to binary:**
  13 ÷ 2 = 6 remainder 1
  6 ÷ 2 = 3 remainder 0
  3 ÷ 2 = 1 remainder 1
  1 ÷ 2 = 0 remainder 1
  Reading the remainders from bottom to top gives `1101`.

- **25 to binary:**
  25 ÷ 2 = 12 remainder 1
  12 ÷ 2 = 6 remainder 0
  6 ÷ 2 = 3 remainder 0
  3 ÷ 2 = 1 remainder 1
  1 ÷ 2 = 0 remainder 1
  Reading the remainders from bottom to top gives `11001`.

- **1010 (binary) to decimal:**
  (1 × 2³) + (0 × 2²) + (1 × 2¹) + (0 × 2⁰) = 8 + 0 + 2 + 0 = `10`

- **1101 (binary) to decimal:**
  (1 × 2³) + (1 × 2²) + (0 × 2¹) + (1 × 2⁰) = 8 + 4 + 0 + 1 = `13`

- **A (hex) to decimal:**
  In hexadecimal, digits go from 0–9 and then A–F, so `A` equals `10` in decimal.

- **1F (hex) to decimal:**
  Since `F` equals 15 in decimal: (1 × 16¹) + (15 × 16⁰) = 16 + 15 = `31`

- **1111 (binary) to hex:**
  First convert `1111` to decimal: 8 + 4 + 2 + 1 = 15. In hex, 15 is `F` (and since 4 binary bits map to 1 hex digit, `1111` is directly `F`).

## 5. Python Verification
| Expression | Result |
|---|---|
| `bin(13)` | `0b1101` |
| `bin(25)` | `0b11001` |
| `int('1010', 2)` | `10` |
| `int('1101', 2)` | `13` |
| `int('A', 16)` | `10` |
| `int('1F', 16)` | `31` |
| `hex(int('1111', 2))` | `0xf` |

## 6. Converter Program Results
| Input | Binary | Hexadecimal |
|---|---|---|
| 42 | 101010 | 2a |
| 100 | 1100100 | 64 |
| 225 | 11100001 | e1 |

## 7. My Understanding
Computers use binary (1s and 0s) because their hardware runs on electrical circuits that only have two states: on or off. Long binary numbers are hard for humans to read without making mistakes, so hexadecimal is used as a shorter way to write them. Each hex digit represents exactly 4 binary bits, which makes converting back and forth really clean, and it's why hex shows up in things like color codes and memory addresses. For text, computers can't store letters directly, so encoding standards like ASCII assign every character a number (like `65` for `'A'` or `97` for `'a'`), which then gets stored in binary.

## 8. Difficulties Faced
I accidentally pasted all my Python commands into the terminal at once, so the interactive shell got stuck showing `...` instead of running them.

## 9. How I Resolved Them
I pressed `Ctrl+C` to exit the multiline prompt and then entered each command one line at a time.

## 10. Evidence/Files
`number_converter.py` in this folder, along with the terminal output above.

## 11. Commit Details
See `git log`.