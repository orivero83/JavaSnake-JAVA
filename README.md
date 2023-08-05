# Snake Game

This is a simple Snake Game implemented in Java using Swing. The game allows the player to control a snake and eat apples to grow longer. The goal is to eat as many apples as possible without colliding with the snake's body or the screen's boundaries.

## Instructions

1. Clone or download the repository.
2. Make sure you have Java Development Kit (JDK) installed on your system.
3. Compile and run the `GamePanel.java` file to start the game.

## How to Play

- Use the arrow keys to control the snake's movement.
- Eat the red apples to grow longer.
- Avoid hitting the snake's body or the screen's boundaries.

## Game Features

- The snake moves at a constant speed.
- Apples are randomly generated on the screen.
- The game ends if the snake collides with its own body or the screen's boundaries.
- The score is displayed at the top of the screen.

## Code Structure

The game is implemented in the `GamePanel` class, which extends `JPanel` and implements `ActionListener`. The `GamePanel` class contains the game logic, drawing methods, and keyboard input handling.

The `startGame()` method initializes the game by creating a new apple, setting the game state to running, and starting the game timer.

The `paintComponent()` method is responsible for drawing the game components on the panel.

The `draw()` method draws the snake, apples, and score on the panel. It is called by `paintComponent()`.

The `newApple()` method generates a new random position for the apple.

The `move()` method updates the snake's position based on the current direction.

The `checkApple()` method checks if the snake has collided with an apple, and if so, it increases the score and generates a new apple.

The `checkCollisions()` method checks for collisions with the snake's body or the screen's boundaries, ending the game if a collision is detected.

The `gameOver()` method displays the final score and a "Game Over" message when the game ends.

The `MyKeyAdapter` inner class handles keyboard input and updates the snake's direction accordingly.

## Game Customization

- You can adjust the `SCREEN_WIDTH` and `SCREEN_HEIGHT` constants to change the size of the game window.
- Modify the `DELAY` constant to adjust the speed of the snake (lower values increase speed).
- You can customize the colors of the snake and apple by changing the `Color` objects in the `draw()` method.
- Feel free to modify the game logic or add new features to make the game even more exciting!

Have fun playing the Snake Game! If you have any suggestions or improvements, feel free to contribute to the repository. Happy coding!
