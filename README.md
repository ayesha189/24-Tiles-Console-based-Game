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
