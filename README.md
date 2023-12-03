# ENGR6991
Implementation of Tic-Tac-Toe Game Using Python and Tkinter on Raspberry Pi

mplementation
4.1 Setting Up the Raspberry Pi
This step is to connect everything and set up the operating system now that the microSD
card and other components are ready. First, let’s connect each and every peripheral:
1. Place the microSD card into the Raspberry Pi’s bottom card slot.
2. Use any one of the four USB ports to connect the mouse and keyboard.
3. Using an HDMI cable designed specifically for your Raspberry Pi model. Connect a
monitor to one of the HDMI ports.
4. Link a power source to the USB power outlet.
After connecting the peripherals, turn on your Raspberry Pi to set up the operating
system [4].
4.1.1 Setup Wizard
Upon initial boot, Raspbian offers an installation process that assists with setting up your
Wi-Fi network, password, locale, and operating system update. Proceed and carry out these
actions as directed[4].
We may start learning Python on the Raspberry Pi by restarting the operating system
when we have finished the instructions!
4.2 Running Python on the Raspberry Pi
Python is a first-class citizen on the Raspberry Pi, which is one of the greatest things
about working with it. Python was chosen as the primary language by the Raspberry Pi
Foundation due to its strength, adaptability, and user-friendliness. Raspbian ships with
Python preloaded, so we’ll be good to go right away [4].
When it comes to programming Python on the Raspberry Pi, we have a wide range of
choices. Throughout the project, we will utilize the widely-liked option is the Mu editor.
10
4.3 Step by Step Guide for the Game Logic
4.3.1 Step 1: Set Up the Tic-Tac-Toe Game Board With Tkinter
We will utilize a regular Python installation to do this project. Since there is no requirement
for an external reliance, there is no need to construct a virtual environment. Tkinter is the
only package we will require, and it is included in the Python standard library[3].
Create a Class to Represent the Game Board:
Using the Tk class, which lets you make the main window of our Tkinter application, we
may construct the board for our game of tic tac toe. Next, we will add a grid of cells to fill
the remaining area of the main window and a display to the top frame.
Utilizing Button objects, created the three-by-three cell grid to expand the game display.
This technique forms the basis of the Tic-Tac-Toe game board inside the graphical user
interface by dynamically generating the interactive canvas on which players can make their
movements.
Figure 4.1: Tic-Tac-Toe Game Board With
Tkinter Code
Figure 4.2: Tic-Tac-Toe Game Board With
Tkinter
4.3.2 Step 2: Set Up the Tic-Tac-Toe Game Logic in Python
This section describes the fundamental principles and procedures that underpin the game of
Tic Tac Toe. The first comprehension builds a sublist of coordinates by iterating across the
grid’s rows, obtaining the coordinates of each cell. A winning combination is represented by
11
each sublist of coordinates. The coordinates of every cell in the grid columns are created as
sublists by the second comprehension.
A similar method is used in the third and fourth comprehensions to obtain the coordinates
of each cell in the board diagonals. Lastly, a list of lists with every conceivable winning
combination on the tic tac toe board is returned by the technique.
You may now consider processing the movements made by the players after setting up
your game board.
Figure 4.3: Figure Out the Winning Combinations.
4.3.3 Step 3: Process the Players’ Moves on the Game’s Logic
We will primarily deal with one kind of occurrence in this game of tic tac toe: player
movements. To put it in Tkinter language, a player can move by simply clicking on the
button widget that represents the selected cell [5].
The TicTacToeGame class will go through several operations in response to each player’s
move. Among these surgeries are:
• Validating the move
• Checking for a winner
• Checking for a tied game
• Toggling the player for the next move
Figure 4.4: Validating the move Figure 4.5: Checking for a winner
12
Figure 4.6: Checking for a tied game Figure 4.7: Toggling the player for the next
move
4.3.4 Step 4: Process Players’ Moves on the Game Board
We can now manage the players’ actions based on the logic of the game. It is now necessary
to link this reasoning to the actual game board. In order for the board to react to player
movements, we must also develop the programming. We can play the game for first time
now.
Figure 4.8: Process Players’ Moves on the Game Board.
4.3.5 Step 5: Provide Options to Play Again and Exit the Game
We’ll give the primary menu for our tic tac toe game in this part. The option to resume
the game will be available on this screen, allowing players to begin a new match. After the
players have completed the game, it will also offer the option to quit [2].
In many GUI programs, main menus are a crucial component. Therefore, developing
them using Tkinter is a useful exercise to enhance our GUI-related abilities outside of game
production.
Here’s an illustration of how creating your own games can be a highly educational ex-
perience as it lets you incorporate abilities and information into projects that aren’t games.
