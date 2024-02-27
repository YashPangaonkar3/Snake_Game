# Snake_Game
#Brif Description
1.	Main Class - SnakeGame.java:
•	The ‘SnakeGame’ class extends ‘JFrame’ and serves as the main class for the game.
•	It creates an instance of the Board class (representing the game board) and sets up the game window.
•	The game window title is set to "Snake Game," and the window dimensions are initially set to 300x300 pixels.
•	The main method creates an object of the ‘SnakeGame’ class, initializing the game.

2.	Game Board Class - Board.java:
•	The Board class extends ‘JPanel’ and implements the ActionListener interface for handling game events.
•	It loads images for the snake, apple, and head of the snake.
•	The game board is set to have a black background and a preferred size of 300x300 pixels.
•	The constructor initializes the game by calling ‘loadImages()’ and ‘initGame()’.
•	The ‘loadImages()’ method loads images from files using ‘ImageIcon’.
•	The ‘initGame()’ method sets up the initial state of the game, including the snake's starting position and the first apple.
•	The game loop is managed by a Timer object that triggers the ‘actionPerformed’ method at regular intervals.

3.	Game Logic:
•	The snake is represented by an array of x and y coordinates for each segment.
•	Arrow keys or designated keys control the snake's direction through the ‘TAdapter’ class, which extends ‘KeyAdapter’.
•	The move() method updates the snake's position based on its direction.
•	Collision detection is handled by the ‘checkCollision()’ method, which checks for collisions with walls and the snake's own body.
•	The ‘checkApple()’ method checks if the snake has eaten an apple and increases the score and snake length accordingly.

4.	Drawing and Rendering:
•	The ‘paintComponent(Graphics g)’ method is responsible for rendering the game elements on the screen.
•	The ‘draw(Graphics g)’ method draws the snake, apple, and head on the screen based on the game state.
•	If the game is ongoing (‘inGame’ is true), the graphics are updated. Otherwise, a "Game Over" message is displayed.

5.	User Input Handling:
•	The ‘TAdapter’ class handles keyboard input using the’ keyPressed’ method.
•	Arrow keys control the snake's direction, with checks to prevent the snake from reversing its direction.

6.	Randomized Apple Generation:
•	The ‘locateApple()’ method generates random coordinates for the apple within the game board.

7.	Game Over Screen:
•	If the game ends, the’ gameOver(Graphics g)’ method displays a "Game Over" message in the center of the screen along with the final score.

8.	Usage:
•	The game can be played by running the ‘SnakeGame.java’ file.
•	Players control the snake with arrow keys and aim to collect apples while avoiding collisions.
