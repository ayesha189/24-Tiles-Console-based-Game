# 24-Tiles – Console-Based Sliding Puzzle Game

<div align="center">

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

## 🎯 How to Play

### Game Controls
1. **Start the Game**
   - Choose difficulty: Easy (8x8) or Hard (10x10)
   
2. **Making Moves**
   - Enter row and column of the first candy (0-indexed)
   - Enter row and column of the adjacent candy to swap
   - Only adjacent swaps (horizontal/vertical) are allowed
   
3. **Scoring**
   - Match 3 candies: Base points
   - Match 4+ candies: Bonus points
   - Complete moves before time runs out!

### Example Move
```
Enter first candy position:
Row: 2
Column: 3

Enter second candy position (adjacent):
Row: 2
Column: 4

✅ Valid swap! Checking for matches...
```

---

## 📁 Project Structure

```
Candy-Crush-Console-Game/
│
├── candy crush.cpp         # Main game logic and implementation
├── candycrush.txt          # Score tracking and game data storage
└── README.md               # Project documentation (this file)
```

### Code Organization
- **candy crush.cpp**: Complete game implementation including:
  - Match detection algorithms
  - Board management and rendering
  - Swap validation logic
  - ANSI color codes for display
  - User input handling
  - Timer system
- **candycrush.txt**: Persistent data storage for:
  - High scores tracking
  - Game statistics
  - Player records

---

## 🛠️ Technologies Used

<p align="left">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" width="50" height="50" alt="C++"/>
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/5f/Windows_logo_-_2012.svg" width="50" height="50" alt="Windows"/>
</p>

- **Language**: C++ (Standard Library)
- **Graphics**: ANSI Escape Codes for colored output
- **I/O**: `<iostream>`, `<fstream>` for console and file operations
- **Platform**: Windows-specific headers (`<conio.h>`, `<windows.h>`)
- **Data Structures**: 2D arrays for board representation

---

## 🎓 Learning Outcomes

This project demonstrates proficiency in:

✅ **C++ Fundamentals**
- Object-oriented programming concepts
- 2D array manipulation and algorithms
- Standard Template Library (STL) usage

✅ **Game Development**
- Game loop design and implementation
- User input handling and validation
- Score tracking and leaderboard systems

✅ **Software Engineering**
- File I/O for persistent data storage
- Modular code structure and functions
- Console UI/UX design principles

✅ **Problem Solving**
- Match-3 algorithm implementation
- Grid-based game logic
- Timer and event management

---

## 🔮 Future Enhancements

### Planned Features
- [ ] **Cross-platform support** (Linux/Mac compatibility)
- [ ] **Gravity system** - candies fall down after matches
- [ ] **Special candies** - striped, wrapped, color bombs
- [ ] **Cascade scoring** - chain reaction bonuses
- [ ] **Power-ups** - shuffle, hint, extra time
- [ ] **Sound effects** - match sounds, background music
- [ ] **Animations** - smoother transitions
- [ ] **Enhanced leaderboard** - player names, dates, statistics
- [ ] **Save/Load game** - resume gameplay
- [ ] **Combo multipliers** - consecutive match bonuses


### Technical Improvements
- [ ] Refactor code into classes (Board, Game, UI, ScoreManager)
- [ ] Add unit tests for core game logic
- [ ] Implement design patterns (Singleton, Factory)
- [ ] Optimize performance for larger boards
- [ ] Add configuration file for game settings

---




---

## 👥 Team

<table>
  <tr>
    <td align="center">
      <img src="" width="100px;" alt="Ayesha Rauf"/>
      <br />
      <sub><b>Nimrah</b></sub>
      <br />
      <sub>23F-0807</sub>
      <br />
      <sub>Core Logic & UI</sub>
    </td>
    <td align="center">
      <img src="" width="100px;" alt="Aqsa Ishaq"/>
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

This project is created for educational purposes as part of a university course assignment.

---

## 📧 Contact

**Ayesha rauf** - [@NIMRAH-S](https://github.com/NIMRAH-S)

**Project Link**: [https://github.com/NIMRAH-S/Candy-Crush-Console-Game](https://github.com/NIMRAH-S/Candy-Crush-Console-Game)

---

## 🙏 Acknowledgments

- Inspired by the original Candy Crush Saga game
- Thanks to our instructors for project guidance
- C++ community for documentation and resources
- ANSI color code references for console styling

---

## ⭐ Show Your Support

If you found this project helpful or interesting, please consider giving it a ⭐!

---

<div align="center">
  <p>Made with ❤️ and C++</p>
  <p>© 2024 Candy Crush Console Game Team</p>
</div>

