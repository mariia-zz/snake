The following classes are presented in my code:
- Snake (main object of the game)
- Room (space where the snake crawls)
- Mice (objects that the snake eats)

The Snake class is a set of parts - components (SnakeSection), they have

there are fields x and y of type int, which are responsible for the location of the pieces.
It is known that one of these parts is the head.
The Snake has a list of all the pieces that make it up.

The head is the piece whose index (index) is 0.
The snake has a direction of movement. The class is responsible for this - enum

SnakeDirection. Possible values ??are -UP, DOWN, LEFT, RIGHT.

The KeyboardObserver class is responsible for implementing the control

Snake.

The Mouse class has two private fields, x and y, of type int. These

the fields are responsible for the location of the mouse.

The Room class has the dimensions of the playing field (width and height), snake

and a mouse.

After a snake has eaten a mouse, a new mouse appears randomly

on the field (within width and height).

The longer the snake, the faster it is. But the maximum speed

is reached at level 15 and then remains constant.

The snake's body is drawn with an "x" and the head with an "X".
A snake dies if it crosses itself or a wall.
In this case, the game ends.

The movement logic is implemented as follows: each move is added one

slice in front and remove from behind. If a snake ate a mouse, then we

do not remove the piece from the back.