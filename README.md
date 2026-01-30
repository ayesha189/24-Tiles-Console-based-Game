# 24-Tiles – Console-Based Sliding Puzzle Game

<div align="left">

![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Console](https://img.shields.io/badge/Console-Game-brightgreen?style=for-the-badge)

**A classic 4×6 sliding tile puzzle game built in C++ with move & time tracking and persistent high-score saving.**

</div>

## 📖 About

**24-Tiles** is a console-based implementation of the classic sliding puzzle (similar to the 15-puzzle but larger). The goal is to arrange numbers **1 to 24** in ascending order inside a **4×6 grid** by sliding adjacent tiles into the empty space.

Features include:
- Move validation (only horizontal/vertical adjacent swaps)
- Real-time move counter
- Game timer
- Persistent best-score saving (moves + time) in `tilegame.txt`
- Clean, readable console UI with clear feedback

This project was developed as a university C++ programming assignment.

## ✨ Features

- **4×6 grid** (24 numbered tiles + 1 empty space)
- Coordinate-based input (0-indexed row & column)
- Validates only **adjacent** moves (up, down, left, right)
- Tracks **total moves** and **elapsed time**
- Saves best performance (fewest moves + fastest time) persistently
- Friendly messages, error handling & win/lose feedback
- Simple, distraction-free console interface

## 🖥️ Requirements

- **Operating System**: Windows (uses `<conio.h>` and `<windows.h>`)
- **Compiler**: MSVC (Visual Studio) or MinGW-w64 (g++)
- Recommended IDE: Visual Studio 2022 Community (easiest for beginners)

> Linux/macOS support is planned for a future version.

## 🚀 Quick Start

### Option 1: Visual Studio (Recommended)

1. Download & install [Visual Studio Community](https://visualstudio.microsoft.com/downloads/)  
   → Select **“Desktop development with C++”** workload during installation.

2. Get the code:

   ```bash
   git clone https://github.com/ayesha189/24-Tile-ConsoleGame.git

   Or download as ZIP and extract

3. **Open in Visual Studio**
   - Launch Visual Studio
   - Click **"Create a new project"**
   - Search for **"Empty Project"** (C++)
   - Name your project and click **"Create"**

4. **Add the Game File**
   - In Solution Explorer, right-click on **"Source Files"**
   - Select **Add → Existing Item**
   - Browse and select `candy crush.cpp`

5. **Build and Run**
   - Press **Ctrl + F5** (or click "Local Windows Debugger")
   - The game will launch in a console window
   - Make sure `candycrush.txt` is in the same directory as your executable

---

### Option 2: VS Code (For Advanced Users)

1. **Install Required Tools**
   - Download and install [VS Code](https://code.visualstudio.com/)
   - Install [MinGW-w64](https://www.mingw-w64.org/) or [MSYS2](https://www.msys2.org/) for GCC compiler
   - Add MinGW `bin` folder to your system PATH

2. **Install VS Code Extensions**
   - Open VS Code
   - Install **C/C++** extension by Microsoft
   - Install **Code Runner** extension (optional, for quick runs)

3. **Clone the Repository**
   ```bash
   git clone https://github.com/ayesha189/CandyCrush-ConsoleGame
   cd Candy-Crush-Console-Game
   ```

4. **Open Folder in VS Code**
   - Open VS Code
   - File → Open Folder → Select the project folder

5. **Compile and Run**
   
   **Method A: Using Terminal**
   - Open integrated terminal (Ctrl + `)
   - Compile:
     ```bash
     g++ "candy crush.cpp" -o candy
     ```
   - Run:
     ```bash
     candy.exe
     ```

   **Method B: Using Code Runner**
   - Open `candy crush.cpp`
   - Right-click in editor → **"Run Code"**
   - Or press **Ctrl + Alt + N**

6. **Create tasks.json (Optional - For Build Task)**
   - Press **Ctrl + Shift + P**
   - Type **"Tasks: Configure Default Build Task"**
   - Select **"C/C++: g++.exe build active file"**
   - Press **Ctrl + Shift + B** to build anytime

---

### 📝 Important Notes
- Ensure `candycrush.txt` is in the same directory as your executable
- The game requires a Windows environment due to platform-specific libraries
- For the best experience, run in a full-screen console window

---


## 🎮 How to Play

### Game Controls
1. **Start the Game**
   - The board shuffles automatically
   - Empty space is shown as **0**

2. **Making Moves**
   - Enter row and column of the **tile** you want to move (0-indexed)
   - Enter row and column of the **empty space** (or the tile you want to swap with)
   - Only **adjacent** (horizontal/vertical) moves are allowed

3. **Winning**
   - Arrange tiles in this exact order:
   -1  2  3  4  5  6
   -7  8  9 10 11 12
   -13 14 15 16 17 18
   -19 20 21 22 23 24
- Game ends when layout is correct → shows moves used & time taken


## 📁 Project Structure

24-Tiles-ConsoleGame/
│
├── tilegame.cpp       # Main game logic and implementation
├── tilegame.txt       # High-score storage (auto-created/updated)
└── README.md          # This documentation file


### Code Organization
- **tilegame.cpp**: Complete game including:
  - 2D array board management
  - Move validation & swapping logic
  - Win condition checking
  - Timer using `<ctime>`
  - File I/O for persistent scores
  - Console display formatting

- **tilegame.txt**: Stores best performances (moves + time)

## 🛠️ Technologies Used
<p align="left">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" width="50" height="50" alt="C++"/>
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/5f/Windows_logo_-_2012.svg" width="50" height="50" alt="Windows"/>
</p>

- **Language**: C++ (Standard Library)
- **Graphics**: Console text output (optional ANSI colors if supported)
- **I/O**: `<iostream>`, `<fstream>`
- **Platform**: Windows-specific (`<conio.h>`, `<windows.h>`)
- **Data Structures**: 2D arrays (`int board[4][6]`)

## 🎓 Learning Outcomes
This project demonstrates proficiency in:

✅ **C++ Fundamentals**  
- 2D array manipulation  
- Control structures & functions  
- STL usage (if applied)

✅ **Game Development**  
- Game loop & real-time input handling  
- State tracking (board, moves, time)  
- Win detection logic

✅ **Software Engineering**  
- File I/O for persistent high scores  
- Input validation & error messages  
- Clean console UI/UX

✅ **Problem Solving**  
- Grid-based algorithms  
- Adjacency & movement constraints  
- Puzzle solvability awareness

## 🔮 Future Enhancements
### Planned Features
- [ ] Cross-platform support (Linux/Mac using ncurses)
- [ ] Undo last move
- [ ] Hint system or next-best-move suggestion
- [ ] Solvability checker (parity-based)
- [ ] Multiple sizes (3×3, 5×5, etc.)
- [ ] Move history replay
- [ ] Enhanced visuals (colors, borders)

### Technical Improvements
- [ ] Refactor into classes (`Board`, `Game`, `ScoreManager`)
- [ ] Add unit tests for move validation & win check
- [ ] Implement design patterns (e.g. Singleton for game state)
- [ ] Configuration file for grid size/timer
- [ ] Better shuffling algorithm (guarantee solvability)

## 👥 Team
<table>
  <tr>
    <td align="center">
      <br />
      <sub><b>Ayesha Rauf</b></sub>
      <br />
      <sub>23F-0807</sub>
      <br />
      <sub>Core Logic & Implementation</sub>
    </td>
    <td align="center">
      <br />
      <sub><b>Aqsa Ishaq</b></sub>
      <br />
      <sub>23F-0839</sub>
      <br />
      <sub>Testing & Debugging</sub>
    </td>
  </tr>
</table>
---

## 📝 License

Educational university project — free to use and modify for learning purposes.

---

## 📧 Contact
**Ayesha Rauf** — [@ayesha189](https://github.com/ayesha189)  
**Project Link**: [https://github.com/ayesha189/24-Tile-ConsoleGame](https://github.com/ayesha189/24-Tile-ConsoleGame)

---

## 🙏 Acknowledgments

- Inspired by classic sliding tile puzzles (15-puzzle family)
- Thanks to instructors for guidance
- C++ community resources & tutorials

---

## ⭐ Support

If you found this project useful or inspiring, please consider giving it a ⭐ on GitHub.
