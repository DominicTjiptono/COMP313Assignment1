# COMP313
### Dominic Flavio Tjiptono
### Student Number: 300502615
### COMP313 Assignment 1

## Simple Side Scroller Game

The game is created using Unreal Engine version 4.25. To ensure that the game runs smoothly, upgrade the version of Unreal Engine in your computer to
version 4.25 before playing the game. Alternatively, the executable file to run the game can be downloaded from 
https://github.com/DominicTjiptono/COMP313Assignment1/blob/master/COMP313Assignment1.exe.

### Game Description

"Simple Side Scroller Game" is a platformer game like New Super Mario Bros (see https://en.wikipedia.org/wiki/New_Super_Mario_Bros.) on Nintendo DS. The main
action of the game is to reach the right most end part of a level from the left most end part of the level without falling or getting hit by any obstacles 
in order to complete a level and then move on to the next level or win the game. Once the player falls from the level, the player's character object will be
automatically removed from the game once the its z-coordinate is below the Kill Z (i.e. -1175000.0). Besides, having player's character hit by an arrow in the game
in any way means the player loses the game. Also, if the player's character collides with a rock, the player will automatically lose the game unless if the rock
is stepped or shot as stepping or shooting at the rock will result in having the rock broken and removed from the game.

An important feature of the game is that it has four levels in increasing order of difficulty. The first two levels are relatively easy as they have rocks but no arrows.
The third levels starts to be difficult as it has both rocks and arrows. Meanwhile, the fourth and last level is the most challenging one.

The hardest part of the game to get working in Unreal is setting the functionality of the obstacles and blocks in the game. This is because for the obstacles, 
blueprint nodes for making it able to cause the player to lose the game (e.g. when rocks hit player's character from sides or the player's character collides with the arrow)
and to automatically move in the opposite direction when hitting a wall are necessary. To do these two things, collision boxes need to be created and they must be bigger than 
their size but not too large. Moreover, when creating the functionality of the blocks, it was challenging as it must be able to spawn a coin which the player can collect 
when the player hit it from the button using player character's head. This is to ensure that the blocks are not meaningless for just being objects occupying the level and also to 
make the game more challenging as the level of difficulty for the player to gain coins to increase score increases as the player needs to go above the blocks after hitting them to 
spawn a coin.

The game's most interesting part is its fourth and last level. This level is the most challenging among all due to a variety of structure of how the ledges and obstacles (i.e. 
arrows and rocks) are placed and that all coins can only be collected in areas which are not easy for the player's character to access (i.e. either above the blocks after the
player's character hit the blocks from the bottom using player's character's head or in areas separating ledges where the player will fall for not moving left or right. 
Moreover, near the right end of the level, there is a part containing three rocks and two arrows where the player must eliminate all the rocks and shoot the arrows so that they 
are not too close together to ensure that the player's character can stay in between them for a while before jumping to advance to the right of the level. Besides, that part 
also has two blocks above which may cause the player's character to fall to the ledge and accidentally get hit by either a rock or an arrow.

#### Game Controls
T: Shoot fire

Space Bar: Jump

A: Move left

D: Move right
