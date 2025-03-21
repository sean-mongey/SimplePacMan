# Simple Pacman

A minimalist implementation of the classic Pac-Man game using HTML, CSS, and JavaScript.

## Overview

This project is a browser-based version of Pac-Man with a simple maze, basic ghost AI, and scoring. The game features:
- A grid-based maze with walls and dots.
- A controllable Pac-Man that consumes dots.
- A ghost that actively chases Pac-Man using Manhattan distance.
- Basic start and restart controls.

## How It Works

- **HTML:** Sets up the canvas for the game and adds Start/Restart buttons.
- **CSS:** Styles the canvas, buttons, and overall page layout.
- **JavaScript:** Contains the game logic including:
  - Initializing the maze board from a predefined pattern.
  - Drawing the game board, Pac-Man, ghost, and score.
  - Handling user input via arrow keys.
  - Game loop and state updates (movement, collision detection, dot consumption, etc.).
  - Simple ghost AI that computes moves based on Manhattan distance to Pac-Man.

## Getting Started

1. **Prerequisites:**  
   All you need is a modern web browser (Chrome, Firefox, Safari, etc.).

2. **Running the Game:**  
   - Open the HTML file (e.g., `index.html`) in your web browser.
   - You will see the title screen with "Simple Pacman" displayed.
   - Click the **Start Game** button to begin playing.
   - Use the arrow keys to control Pac-Man's movement.
   - To restart the game at any time, click the **Restart Game** button.

3. **Game Controls:**  
   - **Arrow Up:** Move Pac-Man up.
   - **Arrow Down:** Move Pac-Man down.
   - **Arrow Left:** Move Pac-Man left.
   - **Arrow Right:** Move Pac-Man right.

## Game Mechanics

- **Maze Layout:**  
  The maze is defined by a 2D array (`mazePattern`) where:
  - `0` represents walls (drawn as blue blocks).
  - `1` represents dots (small white circles).
  - Other values are used to mark dots that have been eaten.

- **Pac-Man:**  
  Starts at the top-left area of the maze and moves according to arrow key inputs. As Pac-Man moves, he consumes dots which increase the score.

- **Ghost:**  
  The ghost starts at the bottom-right area of the maze. Its movement is determined by evaluating all possible moves that decrease the Manhattan distance to Pac-Man and randomly selecting one among the best options.

- **Game Loop:**  
  The game updates every 200 milliseconds:
  - The board is redrawn.
  - Pac-Man and the ghost positions are updated.
  - Collision detection is performed: if Pac-Man and the ghost collide, the game ends.

## Future Improvements

- Enhance ghost AI for more complex behavior.
- Add multiple levels or increasing difficulty.
- Include sound effects and animations.
- Improve user interface and add score persistence.

## License

This project is open source and available for modification and distribution under the terms of your chosen license.

## Acknowledgments

Inspired by the classic arcade game Pac-Man.
