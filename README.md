# Python-Snake-Game
Import the curses module to provide an interface for a text based user interface. Also import the random integer module.

Now for the main code, we initialize the screen and create a new window of a specified height and width.

Next, we enable the keypad and make sure echoing of keys is turned off so the characters pressed don't appear on the screen and also put the curs_set to 0 so it doesn't display the cursor on the screen.

We then enable the global key variables for the arrows, score, snake, and food. We set the snake to 3 'O's and set up the food coordinates in the window

We create a while loop to run the program until the 'esc' key is pressed.

We add a string to display the score and ensure that the snake gets faster as it eats more by altering the timeout() function and we also implement a getch to refresh the screen and wait for the user to press a key.

After a key press we calculate the new coordinates of the snake or break the program if the snake crosses the window boundaries or runs over itself.

For the game progression, every time food is consumed by the snake we increase the score by 1 and create a while loop with a condition of food==[] to randomly generate food and addch() to place it in the window.

Finally, we add the food to the snake by removing the food from the window using pop() and addch() to add the character to the tail of the snake.
