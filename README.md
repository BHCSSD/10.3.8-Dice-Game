# 10.3.8-Dice-Game

**Note that this assignment has a visual mark.**

Choose font and text size thoughtfully.  Align your components carefully. Make it look professional! 

The rules of this casino game are simple.  The player rolls a die; the casino rolls a die.  The higher number wins.  If it is a tie, the player wins big!  You might want to open the NumberGuess game example to remind you about comparing a random number to a user’s number.

## Setting up your file
Set up 8 variables:
  - 6 to hold the dice pictures
  - 1 for the casino’s roll, set to zero to start
  - 1 for the player’s roll, set to zero to start
  - In the preload function, load your 6 dice images
  - In the setup function, create a large window
  - In the draw function, begin by setting a background colour.

## Instructions Area
1. Add the words “Your Name’s Casino” in a big font.
2. In smaller text, preferably in a different font, write the following instructions:
	- Hit the `c` key to roll the Casino’s die.
	- Hit the `p` key to roll your die (P for player).
  	- Hit the `w` key to see if you are a winner.

## Images Area
1. Below your instructions, allocate some space to hold the pictures of the dice.
2. Add text that says Casino’s Roll:  and Player’s Roll: 
3. Draw squares beside each of the above labels that are big enough to hold the pictures (perhaps 200x200).  When you first start, these squares will be empty.  The pictures will go in the boxes once the keys are pressed.
4. Using **TWO** 6-part if statements, draw the proper die image for each player. However, because your dice are both zero to start, no image should be drawn YET.
 ```
 if (casinoroll==1) {
    image(die1,            )
      } else if (casinoroll==2){
      image(die2,            )
``` 
 


## Basic Game Play Using the KeyPressed Function
1. When the `c` key is pressed:
  - randomly generate a number for the casino between 1 and six as shown below.
    - `casinoroll = round(  random(1,7) ) ;`     
  - You need to round so your `IF` statements will work below

2. When the `p` key is pressed
  - repeat the above for the player

3. When the `w` key is pressed, use a 3-part if… else if… statement so that you tell the user:
  - the casino wins if its number is higher
  - the player wins if his/her number is higher
  - the player wins a million dollars if it is a tie

4. in the screen, the text is aligned inconsistently, etc.


## Advanced Challenge
Try to implement a betting system in some way.
