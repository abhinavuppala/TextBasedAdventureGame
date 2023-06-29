# Text Based Adventure Game

Using Java, I created this game as my capstone project in AP Computer Science A, during my junior year of high school. This project didn't use any modules or addons except for the Scanner class to take in user input. The player travels on a 2D grid, fighting enemies and purchasing buffs using gold obtained when beating enemies. This project was completely written by me, Abhinav Uppala.

## Classes

The map is stored in a custom class called Map, which stores a 2D matrix of GameObjects. A GameObject is the parent class for Location and Player, allowing both kinds of classes to be stored and displayed in the grid. A Location is the ? shown on the map, where encounters occur. The Player is shown on the map as the first letter of their name. The Driver class is where the bulk of the game logic occurs, such as moving the player, triggering encounters, running battles, and buying items from the shop.

![map screenshot](https://github.com/abhinavuppala/TextBasedAdventureGame/assets/64037392/c0ba56d3-5cd8-4dcc-b1d0-cda1721775c2)

## Map

Each turn the player can move by typing M and U/D/L/R to specify the direction, or type B to enter the shop. The ? icons on the map represent enemy encounters, and the ? in the very bottom right is the final boss fight. If they want to quit the game, they can do so by typing Q.

![shop screenshot](https://github.com/abhinavuppala/TextBasedAdventureGame/assets/64037392/877b07a8-e7b6-425b-a4c6-9b6416968b5d)

## Shop

Upon entering the shop, the user can buy different types of buffs to their different stats - Attack, Block, and Health. If they do not have enough gold for the purchase, it fails and they get kicked out. Otherwise, the buff is applied and gold is taken from their balance.

![battle scene screenshot](https://github.com/abhinavuppala/TextBasedAdventureGame/assets/64037392/d5c0c825-2fed-4299-b059-9e8774b0929f)

## Battle

In battle, the user has two different options - to attack or to block the incoming attack. The user's stats influence the impact of these actions: the attack stat decides how much damage to do, and the block stat decides the maximum amount of damage that can be blocked with any one block. The Health stat, of course, determines the user's max HP. The user is healed to full health at the start of each battle automatically.
