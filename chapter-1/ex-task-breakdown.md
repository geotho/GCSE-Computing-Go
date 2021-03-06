# Example: breaking down our task

Clark is designing a <span class="circle">game</span> that allows
<span class="circle">players</span> to <u>move</u> around a 7x7 <span class="circle">grid</span>.
Each <span class="circle">position</span> in the <span class="circle">board</span> has a <span class="circle">number</span> to represent the <span class="circle">space</span>:
```
43 44 45 46 47 48 49
42 41 40 39 38 37 36
29 30 31 32 33 34 35
28 27 26 25 24 23 22
15 16 17 18 19 20 21
14 13 12 11 10 09 08
01 02 03 04 05 06 07
```

Players must move through the spaces in numerical order, starting from space 1, all the way to space 49.

Players <u>roll</u> two <span class="circle">6-sided dice</span> and move that number of places, e.g. if they are on space 4 and they roll a
3 and a 2, they move 5 spaces to space 9.

The <span class="circle">winner</span> is the first player to reach space 49. Players do not need to roll an exact number to reach
space 49, for example if they are on 48 and roll 3, they will still win.

Analyse the requirements for this system and design, develop, test and evaluate a program that:
1. allows 2 players to <u>play</u> the game
1. allows the players to take it in turns to roll two 6 sided dice and move
1. <u>displays</u> the <span class="circle">result</span> of each move on the board
1. makes a player move back the number of positions rolled if they roll a double (two dice with the
same number)
1. displays the <span class="circle">messages</span> below when the condition for display is met (the condition is given to you
below):
  1. Start Game message: displays either just before the first roll of the dice, or upon start-up
  1. A message when a ‘double’ is rolled (e.g. a 3 on each die): displays only when the score
both die are identical.
  1. Win message when they finish the game: displays when the player score is 49 or greater.
  1. These messages should be <u>stored</u> externally and then <u>read in</u> to the game at the start of the program.

Some games have <span class="circle">obstacles</span> or <span class="circle">challenges</span> that may send you back or forward by a set number of
spaces.

1. Create a way of externally storing at least 4 “obstacles” and the number of squares they move
forward or backward by.
1. <u>Load</u> these obstacles into the game when it starts.
