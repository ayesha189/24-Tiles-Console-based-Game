# 24-Tiles-Console-based-Game
# 🟩 24-Tile Console Game

<div align="left">
  <h3>A Classic 2D Array-Based Tile Puzzle Game Built in C++</h3>
  
  ![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
  ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
  ![Console](https://img.shields.io/badge/Console-Game-brightgreen?style=for-the-badge)
  
  <p>A console-based 24-tile puzzle game implemented using 2D arrays. Players slide tiles to arrange numbers in order, tracking moves and time, built as part of a C++ learning and game development project.</p>
</div>


## ✨ Features

### 🎮 Gameplay
- **Classic Tile Puzzle**
  - 4x6 grid (24 tiles)
  - Slide tiles using coordinates to reach target order
- **Move Validation**
  - Only adjacent tiles can be swapped
- **Performance Tracking**
  - Move counter
  - Timer for each game session

### 🎨 Visual Experience
- **Console Display**
  - Tiles arranged in a 4x6 grid
  - Clean layout for easy readability
- **Responsive Interface**
  - Clear instructions and feedback
  - Highlights invalid moves

### 💾 Score System
- **Persistent Score Tracking**
  - Saves best move counts and completion times
  - Records stored in `tilegame.txt`
  - View your best performances anytime

---

## 🚀 Getting Started

### Prerequisites
- **Windows OS** (uses Windows-specific libraries: `<conio.h>`, `<windows.h>`)
- **Visual Studio** or **VS Code** with C++ compiler

---

### Option 1: Visual Studio (Recommended for Beginners)

1. **Download and Install Visual Studio**
   - Download [Visual Studio Community](https://visualstudio.microsoft.com/downloads/) (free)
   - During installation, select "Desktop development with C++"

2. **Clone or Download the Repository**
   ```bash
   git clone https://github.com/ayesha189/24-Tile-ConsoleGame
Or download as ZIP and extract

Open in Visual Studio

Launch Visual Studio

Click "Create a new project"

Search for "Empty Project" (C++)

Name your project and click "Create"

Add the Game File

In Solution Explorer, right-click on "Source Files"

Select Add → Existing Item

Browse and select tilegame.cpp

Build and Run

Press Ctrl + F5 (or click "Local Windows Debugger")

The game will launch in a console window

Make sure tilegame.txt is in the same directory as your executable

Option 2: VS Code (For Advanced Users)
Install Required Tools

Download and install VS Code

Install MinGW-w64 or MSYS2 for GCC compiler

Add MinGW bin folder to your system PATH

Install VS Code Extensions

Open VS Code

Install C/C++ extension by Microsoft

Install Code Runner extension (optional, for quick runs)

Clone the Repository

git clone https://github.com/ayesha189/24-Tile-ConsoleGame
cd 24-Tile-Console-Game
Open Folder in VS Code

Open VS Code

File → Open Folder → Select the project folder

Compile and Run

Method A: Using Terminal

Open integrated terminal (Ctrl + `)

Compile:

g++ "tilegame.cpp" -o tilegame
Run:

tilegame.exe
Method B: Using Code Runner

Open tilegame.cpp

Right-click in editor → "Run Code"

Or press Ctrl + Alt + N

Create tasks.json (Optional - For Build Task)

Press Ctrl + Shift + P

Type "Tasks: Configure Default Build Task"

Select "C/C++: g++.exe build active file"

Press Ctrl + Shift + B to build anytime

📝 Important Notes
Ensure tilegame.txt is in the same directory as your executable

The game requires a Windows environment due to platform-specific libraries

For the best experience, run in a full-screen console window

🎯 How to Play
Game Controls
Start the Game

The 4x6 grid will appear with shuffled tiles

Making Moves

Enter row and column of the tile to move (0-indexed)

Enter row and column of the adjacent tile to swap

Only adjacent swaps (horizontal/vertical) are allowed

Winning

Arrange the tiles in ascending order (1-24)

Fewer moves = higher efficiency

Example Move
Enter first tile position:
Row: 1
Column: 2

Enter second tile position (adjacent):
Row: 1
Column: 3

✅ Valid swap! Board updated...
📁 Project Structure
24-Tile-ConsoleGame/
│
├── tilegame.cpp         # Main game logic and implementation
├── tilegame.txt         # Score tracking and game data storage
└── README.md            # Project documentation (this file)
Code Organization
tilegame.cpp: Complete game including:

2D array board management

Move validation logic

Timer system

File I/O for persistent scores

tilegame.txt: Stores best performances

🛠️ Technologies Used
<p align="left"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" width="50" height="50" alt="C++"/> <img src="https://upload.wikimedia.org/wikipedia/commons/5/5f/Windows_logo_-_2012.svg" width="50" height="50" alt="Windows"/> </p>
Language: C++

Graphics: Console-based 2D grid

I/O: <iostream>, <fstream>

Platform: Windows-specific headers (<conio.h>, <windows.h>)

Data Structures: 2D arrays for board representation

🎓 Learning Outcomes
This project demonstrates proficiency in:

✅ C++ Fundamentals

Object-oriented concepts and 2D array manipulation

Standard Template Library (STL) usage

✅ Game Development

Console-based game loop and user input handling

Move validation and timer management

✅ Software Engineering

File I/O for persistent data storage

Modular code structure

Console UI/UX design principles

✅ Problem Solving

Puzzle-solving algorithms

Grid-based logic

Strategic thinking under move constraints

🔮 Future Enhancements
Planned Features
 Cross-platform support (Linux/Mac compatibility)

 Undo move / hint system

 Animated tile sliding

 Enhanced leaderboard with player names and times

 Different puzzle sizes (5x5, 6x6)

 Power-ups or special tiles

Technical Improvements
 Refactor code into classes (Board, Game, ScoreManager)

 Add unit tests for core logic

 Optimize for larger boards

 Configuration file for game settings

👥 Team
<ul> <li>Ayesha Rauf (23f-0807)</li> <li>Aqsa Ishaq (23f-0839)</li> </ul>
📝 License
This project is created for educational purposes as part of a university course assignment.

📧 Contact
Ayesha Rauf: [https://github.com/ayesha189]

Project Link: [https://github.com/ayesha189/24-Tile-ConsoleGame]

🙏 Acknowledgments
Inspired by classic tile puzzle games

Thanks to instructors for project guidance

C++ community for tutorials and resources

⭐ Show Your Support
If you found this project helpful or interesting, please consider giving it a ⭐!
