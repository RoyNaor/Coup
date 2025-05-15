# CPP_EX3_25 – Coup Game Implementation

This project is a C++ implementation of the strategic bluffing game **Coup**, developed as part of an academic assignment to practice object-oriented programming concepts such as inheritance, polymorphism, and class design.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

## 🧠 Overview

The game simulates political intrigue where players aim to eliminate others and become the last one standing. Each player assumes a role with unique abilities, and the game progresses through actions like income collection, taxation, coups, and special role abilities.

## 🎮 Features

- Multiple roles with distinct abilities: General, Governor, Judge, Merchant, Spy, Baron.
- Special abilities for each role via polymorphic methods.
- Turn-based actions: `gather`, `tax`, `bribe`, `arrest`, `sanction`, `coup`, `pass`.
- Special handling for complex game logic, including blocking actions and reviving.
- SFML-powered graphical interface for interactive play.

## 🚀 Getting Started

### Prerequisites

- C++17 or later
- SFML library installed
- CMake

### Installation

```bash
git clone https://github.com/BenjaminSaldman/CPP_EX3_25.git
cd CPP_EX3_25
mkdir build && cd build
cmake ..
make
```

## 🕹️ Usage

Run the game from the `bin` directory:

```bash
./CoupGame
```

Follow the in-game UI prompts to play.

## 🗂️ Project Structure

```text
.
├── Game.cpp / Game.hpp       # Game logic and state management
├── Player.cpp / Player.hpp   # Player data and action handling
├── Roles/                   # All role classes (Baron, Governor, etc.)
├── screens.cpp              # GUI screen logic using SFML
├── tests/                   # Doctest-based unit tests
├── assets/                  # Fonts and UI assets
└── Makefile                 # Build configuration
```

## ✅ Testing

Unit tests are written using the [doctest](https://github.com/doctest/doctest) framework.

To run tests:

```bash
cd tests
g++ -std=c++17 -I../ -I../Roles *.cpp -o tests
./tests
```

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit pull requests for improvements or bug fixes.

## 📄 License

This project is licensed under the MIT License.

---

> **Note:** This project was developed as part of an academic assignment. Please respect academic integrity and do not submit this as your own work.
