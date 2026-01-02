# Assembly Hexadecimal Sequence Processor

## Project Overview

This project is a **16-bit x86 Assembly application** developed as a seminar project.  
It runs in a **DOS environment** and processes a user-provided sequence of hexadecimal characters, offering multiple operations through a text-based menu.

The application demonstrates:
- Modular assembly programming
- User input validation
- Data processing at byte and word level
- Low-level bit manipulation
- Menu-driven UI logic

---

##  Technologies Used

- **x86 Assembly (16-bit)**
- **TASM (Turbo Assembler)**
- **TLINK (Turbo Linker)**
- **DOS / DOSBox environment**

---

## Project Structure

- Proiect_Seminar/
- main.asm — Program entry point
- ui.asm — User interface and menu logic
- printer.asm — Printing routines
- converter.asm — Hexadecimal → binary conversion
- sorter.asm — Sorting routines
- rotator.asm — Bit/byte rotation logic
- byte_searcher.asm — Byte analysis (counting 1 bits)
- exception.asm — General exception handling
- FILE_EXCEPTION.asm — File-related exceptions
- BUILD.BAT — Build automation script
- LINKFILE.LNK — Linker configuration
- *.OBJ — Compiled object files
- MAIN.EXE — Final executable
- *.MAP — Memory maps
- hexa.txt — Example input file




---

## ▶️ Application Features

After starting the program, the user is prompted to input:

- An **even number of hexadecimal characters**
- Minimum **16 hex characters**
- Spaces are allowed

### Available Menu Options

1. **Print the sequence**
2. **Sort the sequence**
3. **Calculate word C**
4. **Rotate the elements of the sequence**
5. **Find the byte with the highest number of `1` bits**  
   - The byte must contain **at least 4 bits set to `1`**
   - If not found, the user can:
     - Enter a new sequence
     - Return to the main menu

---

## ⚙️ Build Instructions

### Prerequisites

- Turbo Assembler (**TASM**)
- Turbo Linker (**TLINK**)
- DOS or **DOSBox**

### Build Steps

1. Open a DOS/DOSBox terminal
2. Navigate to the project directory
3. Run:

```bat
BUILD.BAT
If the build is successful, MAIN.EXE will be generated.
