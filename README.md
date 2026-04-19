# TIC-TAC-TOE GAME

Welcome to the Tic-Tac-Toe project. This program is developed in C++ and supports multiple game modes along with an automated judge mode for testing.

## 1. System Requirements
- **Compiler:** `g++` version >= 15.2.0 (supporting C++20 standard).
- **Operating System:** Windows.

## 2. Compilation
Open your terminal in the project directory and use one of the following commands:

* **Basic command:** `g++ -std=c++20 game.cpp -o game.exe`
* **With warnings (Recommended):** `g++ -std=c++20 -Wall -Wextra game.cpp -o game.exe`
* **Debug build:** `g++ -std=c++20 -Wall -Wextra -g game.cpp -o game.exe`

*(If using VS Code, you can configure `tasks.json` and press `Ctrl + Shift + B` to compile).*

## 3. Usage

### 3.1. Interactive Mode (Default)
Run `game.exe` to start. The menu will prompt you to select:
- Board size (maximum 12x12).
- Winning condition (number of consecutive pieces).
- Game mode: PvP (Player vs Player), PvE (Player vs Bot), EvE (Bot vs Bot).
- Bot difficulty: Easy / Medium / Hard.

### 3.2. Judge Mode
Used for automated testing:
`game.exe --judge --input input1.txt`

## 4. Command Line Options
| Option | Description |
| :--- | :--- |
| `--judge`, `-j` | Enable judge mode (disables UI). |
| `--input`, `-i` | Path to the input file (required with `--judge`). |
| `--log`, `-l` | Path to the log file (default: `log.txt`). |
| `--help`, `-h` | Display help instructions. |

## 5. Examples
- **Standard gameplay:** `game.exe`
- **Run with test case:** `game.exe -j -i input1.txt`
- **Run with test case and output log:** `game.exe -j -i input2.txt -l out.txt`

---
*Note on Computational Complexity:*
- **Compilation:** The time complexity of compilation is $O(N)$, where $N$ is the number of lines of source code.
- **Git Operations:** When you `git push` this file to GitHub, Git calculates the delta between versions with a complexity of $O(M)$, where $M$ is the size of the changes, ensuring high performance for standard project updates.
