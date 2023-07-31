**Full-Front-End-Game**

This GitHub repository contains a front-end game built using HTML5 Canvas and JavaScript. Let's focus on the code, the technologies used, why they are used, and how they work in the context of the project.

**Technologies and Languages Used:**
1. **HTML5 Canvas:** The game uses the HTML5 Canvas element to create a graphics context for rendering 2D shapes and images. The canvas allows the game to render graphics in real-time, enabling smooth animations and interactive visuals within the web browser.

2. **JavaScript:** The game logic and interactivity are implemented using JavaScript. JavaScript is used to handle player input, update game elements, perform collision detection, and manage game flow.

**Code Overview:**
The code starts with an event listener for the "load" event on the window. When the page loads, it initializes the game elements and sets up the game loop.

**Initializing the Game:**
The canvas element and its context (ctx) are fetched from the HTML. The canvas dimensions are set to 1280x720 pixels. The game class is defined and contains various game objects, such as the player, obstacles, eggs, enemies, hatchlings, and particles.

**Player Class:**
The player class is responsible for representing and controlling the player character. It has properties to handle collision detection, movement, animation frames, and the player's image (bull sprite).

**Obstacle Class:**
The obstacle class represents static objects that obstruct the player's movement. Each obstacle is randomly positioned within the game window, and collision detection is performed to avoid overlap with other obstacles.

**Egg Class:**
The egg class represents the collectible eggs in the game. Eggs are randomly generated at regular intervals. Once an egg is collected, it hatches into a larva.

**Larva Class:**
Larvae are hatched from eggs and need to be guided to safety. The larva class handles their movement and collision detection with other objects.

**Enemy Class:**
Enemies (toads) are hostile creatures that move horizontally across the screen. The enemy class manages their position, movement speed, and collision detection.

**Particle Classes:**
The game has two particle classes - fireflies and sparks. Particles are small visual effects that enhance the game's aesthetics. Fireflies fly upwards, while sparks gradually fade away.

**Game Class:**
The game class contains the game's main logic. It handles initializing the game objects, rendering them on the canvas, updating their positions and states, and handling user input (mouse movements and clicks).

**Game Loop:**
The game implements a basic game loop using the `requestAnimationFrame` method. It ensures that the game is rendered at a consistent frame rate, providing smooth animation and responsiveness.

**Collision Detection:**
The game checks for collisions between different game objects using the `checkCollision` method. This method calculates the distance between two objects and determines if their collision circles overlap. If a collision is detected, the game handles the interaction between the objects, such as repositioning them or triggering specific events.

**Debug Mode:**
The game has a debug mode that can be toggled with the 'd' key. When enabled, it displays collision circles and lines to help developers visualize the collision detection and positioning of game elements.

**Game Over and Win Conditions:**
The game tracks the player's score, and there are two end conditions: winning and losing. The player wins when they reach a certain score, and they lose if all hatchlings are lost. The game handles these conditions by displaying appropriate messages and preventing further gameplay.

**Restarting the Game:**
The game can be restarted by pressing the 'r' key. It resets all game objects and allows the player to start a new game.

**Conclusion:**
This GitHub repository showcases a front-end game built using HTML5 Canvas and JavaScript. The code demonstrates effective use of the canvas element for rendering and updating graphics in real-time. It utilizes various classes to represent game objects and manages collision detection to create an interactive gaming experience. The implementation of a game loop ensures smooth animations, and the addition of particles and debug mode enhances the visual aspects of the game. With further improvements and feature additions, this project has the potential to become a polished and engaging web-based game.
Original code created by: Frank's Laboratory
