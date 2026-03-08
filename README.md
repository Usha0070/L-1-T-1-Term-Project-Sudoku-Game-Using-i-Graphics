# Sudoku King 🎮

A graphical Sudoku game built in **C++** using the **iGraphics** library (OpenGL/GLUT) — developed as a Level 1 Term 1 project at BUET.

## 🎬 Video Demonstration

[![Sudoku King Demo](https://img.shields.io/badge/YouTube-Demo%20Video-red?style=for-the-badge&logo=youtube)](https://youtu.be/B1JGbQ2kJfk?si=s6hhklzZRwyJfgS_)

> **Watch the full demo:** https://youtu.be/B1JGbQ2kJfk?si=s6hhklzZRwyJfgS_

---

## 📌 About

Sudoku King is a fully graphical desktop Sudoku game with multiple difficulty levels, a live scoring system, mistake tracking, a persistent leaderboard, and background music — all rendered using OpenGL/GLUT via the iGraphics library.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🖥️ Graphical UI | Full game interface built on OpenGL/GLUT via iGraphics |
| 🎯 Difficulty Levels | Easy, Medium, and Hard puzzles |
| 🏆 Score System | +10 for correct placements, -5 for mistakes |
| ⏱️ Timer & Mistake Counter | Track time elapsed and errors made |
| 📋 Leaderboard | Top scores per level saved to `game_result.txt` |
| 🎵 Sound Effects | Background music and click/keyboard sounds (toggle On/Off) |
| ⌨️ Dual Input | Enter digits via keyboard (1–9) or the on-screen number panel |
| 🔼 Arrow Navigation | Move between grid cells using arrow keys |

---

## 🗂 Project Structure

```
SUDOKU-KING/
├── iMain.cpp               # Main source file — all game logic
├── iGraphics.h             # iGraphics library header (OpenGL/GLUT wrapper)
├── stb_image.h             # Image loading library
├── glut32.dll              # GLUT runtime DLL (must stay in project root)
├── game_result.txt         # Leaderboard and score data
├── Name.txt                # Temporary player name storage
├── templates/              # Sudoku puzzle templates
│   ├── 1.txt               # Easy puzzle
│   ├── 2.txt               # Medium puzzle
│   └── 3.txt               # Hard puzzle
├── pictures/               # All image assets (.bmp)
│   ├── digits/             # Pre-set digit images (1–9)
│   ├── userdigit/          # User-entered digit images
│   ├── level/              # Level indicator images
│   └── *.bmp               # Background and UI images
├── sound/                  # Sound files
│   ├── bg.wav              # Main menu background music
│   ├── playbg.wav          # In-game background music
│   ├── mouse-click.wav     # Mouse click sound
│   └── keyboard.wav        # Keyboard sound
├── .vscode/                # VS Code build configuration
│   ├── tasks.json
│   ├── c_cpp_properties.json
│   └── settings.json
└── README.md
```

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Language | C++ |
| Graphics | OpenGL, GLUT |
| Library | iGraphics (OpenGL/GLUT wrapper) |
| Image Loading | stb_image.h |
| Audio | Windows Multimedia (winmm) |
| IDE | Visual Studio Code |
| Compiler | MinGW GCC (32-bit) |

---

## ⚙️ Prerequisites

- **MinGW** (GCC for Windows, 32-bit) — installed at `C:\MinGW`
  - Download from [winlibs.com](https://winlibs.com) (MSVCRT, 32-bit)
  - Add `C:\MinGW\bin` to your system **PATH**
- **Required `.lib` files** — place in `C:\MinGW\lib\`:
  - `glut32.lib`
  - `glaux.lib`
  - `libglut32.a`
- **Visual Studio Code** with the **C/C++ Extension** by Microsoft

---

## 🚀 Setup & Installation

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

## 🎮 How to Play

1. Launch the game and enter your name on the login screen
2. From the main menu, select your preferred difficulty under **Level**
3. Click **Play Game** to start
4. Click a cell on the grid to select it, then:
   - Type a digit (**1–9**) using the keyboard, **or**
   - Click a number from the on-screen panel
5. Use **arrow keys** to navigate between cells
6. Press **Erase** to clear a selected cell
7. Click **Exit** to save your score and return to the menu

---

## 👨‍💻 Author

**Md. Usha Khan**
Bangladesh University of Engineering & Technology (BUET)
Student ID: 2205065 | Session: 2022–2023
Supervisor: Mustari Sadia, Lecturer, BUET

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
