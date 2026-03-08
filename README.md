# Sudoku Game Using iGraphics Library

This project is a **Sudoku Game** developed using the **iGraphics** library in **C++**. The game allows users to play Sudoku on a graphical interface, featuring different game levels and a clean user interface. It also includes features such as background sound and level selection.

## Features

- **Graphical User Interface**: Built using the **iGraphics** library, providing a rich visual experience.
- **Multiple Game Levels**: Includes Easy, Medium, and Hard levels for users to choose from.
- **Sound Effects**: Background music and sound effects to enhance gameplay.
- **Sudoku Solver**: Automatically solves the puzzle for users to compare their solution.
- **Interactive Design**: Allows users to interact with the grid and enter numbers easily.

## Video Demonstration

Watch the game in action by clicking the link below:
[Game Video Visualization](https://youtu.be/B1JGbQ2kJfk?si=J_yJpdN5U2SpDEWb)

## Setup and Installation

### Prerequisites
1. **C++ Compiler**: Make sure you have a C++ compiler installed (e.g., MinGW for Windows, or GCC for Linux/Mac).
2. **iGraphics Library**: You need to have the **iGraphics** library installed on your system. Follow the [installation guide](https://github.com/igra/igraphics) for iGraphics setup.

### Steps to Run the Game

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Usha0070/L-1-T-1-Term-Project-Sudoku-Game-Using-i-Graphics.git

Navigate to the project directory:

cd L-1-T-1-Term-Project-Sudoku-Game-Using-i-Graphics

Compile the project:

If you are using MinGW on Windows, you can compile the program using the following command:

g++ -o sudoku_game iMain.cpp -lgraphics

Run the game:

After compiling, you can run the game with the following command:

./sudoku_game
Project Structure
SUDOKU-GAME-USING-i-graphics-LIBRARY-main/
├── iMain.cpp          # Main C++ file with game logic
├── iGraphics.h        # iGraphics library header
├── README.md          # Project documentation
├── templates/          # Sudoku puzzle templates
│   ├── 1.txt
│   ├── 2.txt
│   └── 3.txt
├── pictures/          # Game assets (images)
│   ├── About_us.bmp
│   ├── Game_level.bmp
│   └── ...
├── sound/             # Sound files
│   ├── bg.wav
│   └── ...
└── README.md          # This file
Contributing

If you want to contribute to this project, feel free to fork it and submit a pull request. Contributions are always welcome!

License

This project is open-source and available under the MIT License
