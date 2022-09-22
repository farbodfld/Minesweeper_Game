# Minesweeper_Game
Minesweeper game implementation with object oriented in CPP language.

## Implementation cases in the project
In this assignment, you must implement this game on the console.

When the program runs, get the length, width, and number of bombs from the user. 
Note that the number of bombs should not exceed the number of houses. There should 
also be room for at least one bomb-free house.

After getting the screen specifications from the user, show him the game screen.
The way of presentation is up to you and there is no compulsion in this field.
Every time you show the page to the user, you need to get a command from them.
This command can be one of the following commands:

* Print: This command prints the page (as far as the user has gone). This display should show the same details as you see in the screenshots above.

* Clicking on a house: This command gets the row and column from the user, and 
reveals the desired house to the user. If the desired house is the flag, nothing will 
happen. If a bomb explodes, the user loses. Otherwise, the corresponding 
number in that house will be shown to the user.
* Placing a flag on a house: with this command, after getting the row and column 
from the user, a flag is placed in the corresponding house. Note that the flag can 
only be placed on unrevealed houses.
* Placing a question mark on a house: with this command, a question mark is 
placed on the corresponding house after receiving the row and column from the 
user. Note that the question mark can only be placed on houses that are not 
revealed.
* Total number of bombs: Prints the number of bombs in the table.
* Number of Undiscovered Bombs: Assuming the user has flagged the correct 
houses, this number represents the number of bombs the user has yet to 
discover.

Also, in case of winning or losing, display the corresponding message to the user. After 
this, it is not necessary to ask the user for instructions.

## Bonus
* Add a command to the game that shows the user the past time. This time should 
be measured relative to the start time of the game.
* Save the best times that the user has achieved in previous games in a file. Load 
this file in your program every time you open the program. By entering a 
command, the user can see the top ranks (along with the name of the person 
who registered the record). Also, if the user solves the game in a time when he 
can be in the Top 10, you should get his name from him and save it in the 
rankings. For this you can read the fstream library.
* If you look at the original game, sometimes when the user clicks on a house with 
the number zero (before he knows it's zero!), all the houses adjacent to the 
clicked house will open! This issue can also be seen in the screenshots in case 
of questions. For example, in the second screenshot, I have clicked on only one 
empty house, but many houses are revealed. Hint: You can study the DFS 
algorithm.
