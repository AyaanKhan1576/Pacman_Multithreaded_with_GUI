# Multithreaded Pac-Man Game

## Overview
This project is a multithreaded implementation of the classic Pac-Man game using OpenGL and pthreads for concurrent processing. The game features Pac-Man navigating a maze, collecting pellets, and avoiding ghosts. The ghosts follow different movement patterns, some random and some tracking Pac-Man. The game ends when Pac-Man loses all lives or collects all pellets.

## Features
- **Multithreading:** Uses pthreads to handle different aspects of the game, such as game logic, rendering, and ghost movement.
- **Real-time Rendering:** Implements OpenGL for rendering the game board, characters, and score display.
- **Ghost AI:** Each ghost has a unique movement pattern, including vertical/horizontal movement and chasing Pac-Man.
- **Power Pellets:** Collecting power pellets turns ghosts vulnerable, allowing Pac-Man to defeat them.
- **Collision Detection:** Detects collisions between Pac-Man and ghosts to update the game state accordingly.
- **Score System:** Players earn points by collecting pellets and defeating vulnerable ghosts.
- **Win/Loss Conditions:** The game ends when all pellets are collected (win) or when Pac-Man loses all lives (game over).
- **Keyboard Controls:** Arrow keys allow Pac-Man to move up, down, left, or right.

## Controls
- **Arrow Keys:** Move Pac-Man in the desired direction.

## Dependencies
- OpenGL (GLUT)
- pthreads
- C standard libraries (stdio.h, stdlib.h, math.h, etc.)

## How to Compile and Run
1. Install necessary dependencies (OpenGL, GLUT, and pthreads).
2. Compile the program using:
   ```sh
   gcc pacman.c -o pacman -lGL -lGLU -lglut -lpthread -lm
   ```
3. Run the executable:
   ```sh
   ./pacman
   ```

## Future Improvements
- Improve ghost AI to mimic original game behavior.
- Add sound effects and animations.
- Implement a menu and difficulty levels.
- Optimize multithreading for better performance.

## Author
Developed by Ayaan Khan as part of Operating Systems Final Project.

