# PYTHON-ASSIGNMENT-2
ASSIGNMENT GIVEN BY PROFF.CHENNA REDDY SIR

#######################################
Student details:
1. N.NAGA SWETHA - 22001A0541
2. H.GRACE LILLY - 22001A0544
3. B.ANITHA - 22001A0536

**Snake Game Documentation:**

**Overview:**
This code is a simple implementation of the classic "Snake" game using the `turtle` module in Python. The player controls a snake represented by a square-shaped head, and the objective is to eat food represented by a red circle. As the snake eats food, it grows longer, and the player earns points. The game ends if the snake collides with the boundary or with its own body.

**Requirements:**
1. Python: This code requires Python to be installed on the system.
2. `turtle` module: The code uses the `turtle` module for graphics and user input.
3. The game runs on any operating system that supports Python and the `turtle` module.

**Game Elements:**
1. **Snake Head (`head`):** Represents the player-controlled snake's head.
2. **Snake Food (`food`):** Represents the food that the snake needs to eat to grow.
3. **Snake Segments (`segments`):** A list to keep track of the snake's body segments.
4. **Score (`score`):** Integer variable to store the current score.
5. **High Score (`high_score`):** Integer variable to store the highest score achieved during the game.

**Game Functions:**
1. **`go_up()`:** Function to change the snake's direction to "up" when the 'w' key is pressed.
2. **`go_down()`:** Function to change the snake's direction to "down" when the 's' key is pressed.
3. **`go_left()`:** Function to change the snake's direction to "left" when the 'a' key is pressed.
4. **`go_right()`:** Function to change the snake's direction to "right" when the 'd' key is pressed.
5. **`move()`:** Function to move the snake's head in the current direction.

**Keyboard Bindings:**
The `window` listens for specific keyboard inputs and associates them with the corresponding functions:
- 'w': Calls `go_up()`
- 's': Calls `go_down()`
- 'a': Calls `go_left()`
- 'd': Calls `go_right()`

**Main Game Loop:**
The code runs an infinite loop where the game progresses:
1. The window updates with each iteration of the loop.
2. The code checks for collisions with the boundary of the game window. If the snake hits the boundary, the game resets.
3. The code checks for collisions with the food. If the snake eats the food, its length increases, and the score is updated.
4. The snake's body segments follow the head's movement to simulate the snake's motion.
5. The code checks for collisions between the snake's head and body segments. If they collide, the game resets.
6. The delay between each iteration controls the speed of the snake's movement.

**Scoring:**
- The player earns 10 points for each food item the snake consumes.
- The highest score achieved during the game is stored in `high_score`.

**Game Over and Reset:**
- When the snake collides with the boundary or its own body, the game waits for 1 second before resetting the game.
- The snake's head returns to the center of the window, and the direction is set to "Stop."
- All the snake's body segments are hidden and cleared from the screen.
- The score is reset to 0, and the delay between each movement is reset to 0.1.
- The game displays the current score and the high score.

**Note:**
- The game will run indefinitely in the current implementation. To end the game, the user needs to close the window manually.

**Usage:**
1. Copy and paste the code into a Python environment.
2. Run the script.
3. Control the snake's direction using 'w', 's', 'a', and 'd' keys.
4. Try to eat the red food and grow the snake.
5. Avoid collisions with the boundary and the snake's own body.
6. The game will automatically reset after collisions, and the score will be displayed on the screen.
