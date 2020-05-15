# Syfe-MemoryGame
Name of the project: Syfe
Description:

In the first 2 seconds, a Welcome message will be displayed on the lcd display, and after that a menu will be shown.

 * Menu(You can go through the menu using the joystick.There will be a cursor in the shape of ">" in front of several menu options: 
   * Play (while playing, the LCD will display the score, time, level and lives)
   * High score(displays the highest score of the player for each of the three levels)
   * Settings(where you can set the level for the game and leave feedback)

# The game: #

* Before the game, a map with bombs will be randomly chosen
* In the first 5 seconds, bombs will be displayed on the screen for 5 seconds, time in which the player cannot move. The player must remember their location because they disapper after 5 seconds.
* Then, you will be placed in the upper left corner and you will have to reach the opposite corner without hitting too many bombs
* The number of bombs depends on the level.
* if you hit a bomb, you will lose 5 points from your score but you will be shown the location of the bombs for 3 seconds on the display.
* The player has 20 seconds to finish the level.
# The levels: #

There are 3 levels, and each level has 5 more bombs than the previous one.
* level 1: 10 bombs
* level 2: 15 bombs
* level 3: 20 bombs.

You can set the level from the settings.
# The feedback: #
In settings you can give feedback to the game from 1 to 5.
# The RGB led: #

* If you are one step away from a bomb, the LED becomes red
* If you are two or more steps away from a bomb, the LED becomes green
# The distance sensor: #

Detects your distance and turns of the red/green option if you are too close to the screen.
The score:

* In order to make a high score, you must go through as many boxes and as few bombs as possible until you reach the bottom right corner
you will receive a point on each box
* Score is obtained by going through as many boxes but as few bombs as possible until you reach the bottom right corner. The player will recieve a point for each box.
* Each box is unique, so you cannot get two points for the same box.
* If you step on a bomb, you will lose 5 points. If your score is less than 5, the score becomes 0.
* At the end of te game, the remaining seconds will be transformed into points(each second representing one additional point)
high score for each level will be stored in EEPROM
# End of the game: #
*Video link: https://youtu.be/ZYHMe5cUwU4
* At the end of the game, the player will be greeted with a "Congratulations" message and a "You made a new high score" if the player has gotten more points than his previous highscore. After that, the final score and number of seconds he spent will be displayed on top of the LCD.At the bottom a Play again and a Menu with the ">" cursor.

Used materials: 8x8 LED matrix, LCD display, Joystick, MAX7219 Driver, RGB led, arduino board, breadboards, distance sensor, potentiometer, wires, resistors, electrolytic capacitor of 10 μF, ceramic capacitor of 104 pF


# User Stories: #
## User1: ###
I would like to see my highest score.

Notes:

Highscores should be saved and and should remain even after the device is restarted.

Priority:

Required

Status: 

*Done*

## User2: ##
I want to play multiplayer with other people and see who finishes fasterwhen we rush to the end point.
Notes:

A multiplayer mode would be require player interaction. In the current iteration competition is achieved through comparing each player scores in different gaming sessions and mesured through highscore.
Priority:

Unnecessary

Status:

*Canceled*

## User3: ##
I have played with the game for quite a bit and the proximity light is too bright. Can it be toned down ?

Notes:
On the initial game, lenght expose to the bright light led to reduced player satisfaction.
We have installed a distance sensor that turns on the led only when the player is at a reasonable distance from the game.
Priority:
Optional
Status:
*Done*



## User4(lead developer Bogdan): ##
The circuitry is exposed and can be easily messed up.
Notes:
We have built a casing that houses the hardware.
Priority:
Highly recommended(but not required)
Status:
*Done*
## User5: ##
The game is too easy and boring.
Notes:
We have added 2  more levels each with increased number of bombs.
Priority:
Recommended
Status:
*Done*
## User6: ##
The game runs slowly and has moments when it stops running.
Notes:
We have refactored the code to remove freeze and make it run smoothly.
Priority:
Highly recommended
Status:
*Done*
## User7: ##
I would like to save and load the game.
Notes:
The game has a low duration and a save&load feature would be impractical.
Priority:
Very low priority
Status:
Canceled
## User8: ##
Does this game have sound ?
Notes:
Sound could create a pleasant environment for playing the game.
Priority:
Recommended
Status:
* Canceled due to time retraints *


## User9: ##
So the game has no story? That is very bad.
Notes:
A story was added. It might creatge immersion(probably not).
Priority:
Low priority
Status:
*Done*


## User10: ##
The game is unforgiving if you are distracted even for a second at the beginning.
Notes:
We have added a second life as an error margin.
Prority:
Low priority
Status:
*Done*


| # | Comments | Notes | Priority | Status |
| ------------- | ------------- |
| 1  | I would like to see my highest score.  | Highscores should be saved and and should remain even after the device is restarted. | Required | Done |
| 2  | Content Cell  |
| 3  | Content Cell  |
| 4  | Content Cell  |
| 5  | Content Cell  |
| 6  | Content Cell  |
| 7  | Content Cell  |
| 8  | Content Cell  |
| 9  | Content Cell  |
| 10  | Content Cell  |
