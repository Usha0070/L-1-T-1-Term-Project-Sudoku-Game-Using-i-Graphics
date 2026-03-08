# Sudoku King 🎮

A Sudoku game developed in **C++** using the **iGraphics** library (an OpenGL/GLUT wrapper). The game features a full graphical interface with multiple difficulty levels, a scoring system, a leaderboard, and background music.

---

## Features

- **Graphical User Interface** — Built using the iGraphics library on top of OpenGL/GLUT
- **Multiple Difficulty Levels** — Easy, Medium, and Hard puzzles to choose from
- **Score System** — Earn +10 points for correct placements, lose -5 for mistakes
- **Mistake Counter & Timer** — Track errors and time elapsed during gameplay
- **Leaderboard** — Top scores per level saved and displayed from `game_result.txt`
- **Sound Effects** — Background music and click/keyboard sounds (toggle On/Off in-game)
- **Keyboard & Mouse Input** — Enter digits via keyboard (1–9) or the on-screen number panel
- **Arrow Key Navigation** — Move between grid cells using arrow keys

---

## Project Structure

```
SUDOKU-KING/
├── iMain.cpp               # Main C++ source file with all game logic
├── iGraphics.h             # iGraphics library header (OpenGL/GLUT wrapper)
├── stb_image.h             # Image loading library (required by iGraphics)
├── glut32.dll              # GLUT runtime DLL (must be in project root)
├── game_result.txt         # Stores player scores and leaderboard data
├── Name.txt                # Temporary player name file
├── templates/              # Sudoku puzzle templates
│   ├── 1.txt               # Easy puzzle
│   ├── 2.txt               # Medium puzzle
│   └── 3.txt               # Hard puzzle
├── pictures/               # All game image assets (.bmp)
│   ├── digits/             # Digit images (1.bmp – 9.bmp)
│   ├── userdigit/          # User-entered digit images
│   ├── level/              # Level indicator images
│   └── *.bmp               # Background and UI images
├── sound/                  # Sound files (not included due to size)
│   ├── bg.wav              # Background music
│   ├── playbg.wav          # In-game background music
│   ├── mouse-click.wav     # Mouse click sound effect
│   └── keyboard.wav        # Keyboard sound effect
├── .vscode/                # VS Code build configuration
│   ├── tasks.json
│   ├── c_cpp_properties.json
│   └── settings.json
└── README.md
```

---

## Prerequisites

1. **MinGW** (GCC for Windows) — installed at `C:\MinGW`
   - Download from [winlibs.com](https://winlibs.com) (MSVCRT, 32-bit)
   - Add `C:\MinGW\bin` to your system **PATH**
2. **Required `.lib` files** — place in `C:\MinGW\lib\`:
   - `glut32.lib`
   - `glaux.lib`
   - `libglut32.a`
3. **Visual Studio Code** with the **C/C++ Extension** by Microsoft

---

## Setup & Installation

### 1. Clone the repository

```bash
git clone https://github.com/Usha0070/L-1-T-1-Term-Project-Sudoku-Game-Using-i-Graphics.git
cd L-1-T-1-Term-Project-Sudoku-Game-Using-i-Graphics
```

### 2. Open in VS Code

```bash
code .
```

### 3. Build & Run

Press **`Ctrl + Shift + B`** — this triggers the pre-configured **Build & Run** task in `.vscode/tasks.json`, which compiles and launches the game automatically.

**Or compile manually from terminal:**

```bash
gcc iMain.cpp -o SudokuKing -lopengl32 -lglu32 -lglut32 -lglaux -lstdc++ -lwinmm -w
./SudokuKing
```

> ⚠️ Make sure `glut32.dll` is in the **same folder** as the compiled `.exe` before running.

---

## How to Play

1. Launch the game and enter your name on the login screen
2. From the main menu, optionally set your preferred difficulty under **Level**
3. Click **Play Game** to start
4. Click a cell on the grid to select it, then:
   - Type a digit (1–9) using the keyboard, **or**
   - Click a number from the on-screen panel
5. Use **arrow keys** to navigate between cells
6. Press the **Erase** button to clear a selected cell
7. Click **Exit** to save your score and return to the menu

---

## Video Demonstration

*https://youtu.be/B1JGbQ2kJfk?si=s6hhklzZRwyJfgS_*

---

## Author

**Md. Usha Khan**
Bangladesh University of Engineering & Technology (BUET)
Student ID: 2205065 | Session: 2022–2023
Supervisor: Mustari Sadia, Lecturer, BUET

---

## License

This project is open-source and available under the [MIT License](LICENSE).
