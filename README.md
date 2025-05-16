# Coup Game Implementation

This project is a C++ implementation of the strategic bluffing game **Coup**, developed as part of an academic assignment to practice object-oriented programming concepts such as inheritance, polymorphism, and class design.

## 🧠 Overview

The game simulates political intrigue where players aim to eliminate others and become the last one standing. Each player assumes a role with unique abilities, and the game progresses through actions like income collection, taxation, coups, and special role abilities.

## ✨ Features

- ✅ Object-Oriented Design with role-specific polymorphic behaviors  
- 🎭 Role Types: Governor, General, Spy, Judge, Baron, Merchant  
- 🪙 Actions: Gather, Tax, Bribe, Sanction, Arrest, Coup  
- 🎯 Target selection with UI prompts  
- ⌨️ Text-based UI using SFML for visual game screen  
- 🧪 Unit testing using Doctest  
- 🧠 Memory safety tested via **Valgrind**  

---

## 🚀 Getting Started

### Requirements

- C++11 or later  
- SFML library  
- `g++` compiler  
- `valgrind` (for memory testing)  
- Linux or Windows with WSL or Ubunto

```bash
git clone https://github.com/RoyNaor/Coup.git
cd Coup
mkdir build && cd build
cmake ..
make
```

## 🕹️ Usage

Run the game from the `bin` directory:

```bash
./CoupGame
```

Run the game's tests:

```bash
make test
```

Run the game's Memory Leak Check (Valgrind):
```bash
valgrind --leak-check=full ./coupGame
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

