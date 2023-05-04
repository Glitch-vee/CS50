"Flappy Sprite" is a fun and addictive game, inspired by the popular "Flappy Bird". In this game, you control a cute little sprite that must fly through a series of block-like obstacles, while avoiding pipes and other hazards. The gameplay is simple yet challenging, and the graphics are colorful, making it an enjoyable experience for all ages.
This project was created using Scratch.

heres a video for the gameplay
https://youtu.be/7JoqmTMqPkA

![Alt text](https://i.imgur.com/FVit6XG.gif)

The game involves 4 sprites, which are all created and managed using Scratch's block-based programming language.

**Sprite 1 is the obstacle blocks. It has two functions:**

![Alt text](https://imgtr.ee/images/2023/05/04/aaNUR.png)

1. When the green flag is pressed, a clone of itself is created after a 2-second delay using the "create clone of" block. Additionally, a custom variable "Var" is changed by 1, which is used to keep track of the number of clones created, using the "change Var by" block. This is done in a forever loop, which continuously runs until the game is ended.

2. When the clone starts, it is shown on the screen using the "show" block. Then, an if-else condition is run to determine where to place the block. This is done by generating a random number between 1 and 2 using the "pick random" block. If the number is 1, the block is placed above with a random height within a certain limit, otherwise, it is placed below with the same height limit. The blocks move from right to left using the "change x by -5" block until they reach a certain position on the x-axis. Once this position is reached, the block (i.e., Sprite 1) is deleted using the "delete this clone" block.




The "cat flying" sprite is responsible for controlling the movement of the flappy cat. Here's how its code works:

![Alt text](https://imgtr.ee/images/2023/05/04/aa5eb.png)

1. When the green flag is pressed, the variable "Var" is set to 0 and the position of the sprite is set to x=0 and y=0 using the "go to x:0 y:0" block.
2. The sprite is then placed inside a forever loop, which means the code within it will run continuously until the game is ended.
3. Inside the forever loop, there is an if-else conditional block that checks whether the backspace key is pressed or not.
4. If the backspace key is pressed, the code inside the "if" block runs. Here, there is another if condition that limits the y position by stating that if y is below 120, then for every backspace key press, the y position changes by 5 using the "change y by" block. This allows the player to move the flappy cat upwards.
5. If the backspace key is not pressed, the code inside the "else" block runs. Here, there is another if condition that limits the height of the y position by -78. If the y position is greater than -78 and the backspace key is not pressed, the y position changes by -5 using the "change y by" block. This allows the player to move the flappy cat downwards.
6. Lastly, there is another if condition below the primary if-else block that checks whether the "cat flying" sprite touches the "Sprite1" (i.e., obstacle block). If the two sprites collide, a message "dang" is broadcasted using the "broadcast" block and the game is stopped using the "stop all" block.
