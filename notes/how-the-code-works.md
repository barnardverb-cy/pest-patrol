# How the code works

The main game is in [index.html](../index.html). It sets up a canvas, draws the sari-sari store, and then runs a game loop that keeps the scene updating.

The first section of the script grabs the canvas and the HUD elements from the page. It also stores the mouse position, the list of mosquitoes, and the game state variables such as `score`, `timeLeft`, and `gameRunning`. The score is kept in a plain JavaScript variable near the top of the script, and it is displayed by the HUD drawing function and by the final-score overlay at the end of the round.

The store drawing code uses a series of helper functions to paint walls, shelves, products, jars, counters, and decorations. The mosquito data is stored as small objects with a position, scale, points value, and lifetime. A function called `spawnMosquito()` adds a new mosquito only when the game is running and the spawn limit is not hit.

The main animation loop, `gameLoop()`, clears the canvas, draws the store, updates the time remaining, removes expired mosquitoes, and draws the aiming crosshair. Each frame also checks whether the timer has reached zero. When it does, `endGame()` stops the round, shows the final score, and clears out the remaining mosquitoes and hit effects.

Player input is handled with a `mousemove` listener for the aim position and a `click` listener for the shot. The click logic checks each mosquito to see whether the pointer is within its hit radius. If it is, the score increases by the mosquito's value, a hit effect is created, and the mosquito is removed.

The restart button calls `startGame()`, which resets the score, timer, hit effects, and mosquito list before restarting the animation loop.
