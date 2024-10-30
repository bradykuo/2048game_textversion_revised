# 2048 文字版遊戲＿改良版

An enhanced text-based version of the classic 2048 game implemented in C++. This version extends the traditional 2048 game with additional diagonal movement capabilities and save/load functionality.

## Features

- Traditional 2048 game mechanics
- Extended movement in 8 directions:
  - Up (T)
  - Down (B)
  - Left (F)
  - Right (H)
  - Upper-left (R)
  - Upper-right (Y)
  - Lower-left (V)
  - Lower-right (N)
- Game state saving and loading
- Score tracking
- File corruption detection and handling
- Cross-platform compatibility (Windows/macOS/Linux)

## Requirements

- C++ compiler (GCC, Clang, or MSVC)
- Terminal/Console that supports ANSI escape codes
- CMake (optional, for building)

### Windows
- MinGW or Visual Studio 2019+ with C++ support
- Windows Terminal (recommended) or CMD

### macOS/Linux
- GCC or Clang
- Terminal emulator

## Building and Running

### On macOS/Linux
```bash
# Clone the repository
git clone https://github.com/bradykuo/2048game_textversion_revised.git
cd 2048game_textversion_revised

# Compile
g++ main.cpp game.cpp -o 2048game

# Run
./2048game
```

### On Windows
```bash
# Using MinGW
g++ main.cpp game.cpp -o 2048game.exe

# Run
2048game.exe
```

## Game Controls

- T: Move Up
- B: Move Down
- F: Move Left
- H: Move Right
- R: Move Upper-left
- Y: Move Upper-right
- V: Move Lower-left
- N: Move Lower-right
- O: Save game
- P: Load game
- ESC: Quit game

## Implementation Details

The game is implemented using C++ with Object-Oriented Programming principles:
- `game` class handling core game mechanics
- Custom exception handling for file corruption
- Cross-platform terminal handling

### Project Structure
```
.
├── main.cpp          # Main game loop and UI
├── game.cpp          # Game logic implementation
├── 2048.h           # Game class definition
└── exception.h      # Custom exception classes
```

## Original Assignment Requirements

This game was developed as part of a programming assignment with the following key requirements:
1. Implement the classic 2048 game with additional diagonal movement
2. Include save/load functionality with file corruption handling
3. Use object-oriented programming principles
4. Implement custom exception handling

## Contributors

- [bradykuo](https://github.com/bradykuo)

## License

This project is available under the MIT License. See the LICENSE file for more details.
