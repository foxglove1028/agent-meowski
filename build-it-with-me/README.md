# Agent-Meowski - Build it with me
Follow along the various documents to build your own Agent-Meowski game using JavaScript, CSS and HTML5 canvas.

##The lessons are as follows:

###Setup
*Setting up the various basic functions/methods of the game such as environment, sound, character, points, movement and task accomplishments.*

####Setup involves creating the classes for:

* global stuff
* level requirements/tasks
* tutorial text
* scoring
* inventory
* movement - slow, normal, fast (speed ranges from 1-10)
* basic attack/defense - melee/ranged
* armor - box, frying pan, sweater, tux (makes him much cooler)
* weapons - claws, teeth, spray
* potions - healing, growth, shrink, invisible
* food/water - heals hitpoints, tainted food/water makes the player sick and removes hitpoints
* hitpoints
* deaths/lives
* interactive dialog
* text, choices and conditions
* environment
* sound
* preloading level
* story introduction
* character
  * npc - uses: interactive dialog, inventory;
  * player - uses: levels, movement, hitpoints, inventory, lives/deaths, attacks/defense, armor, weapons, potions, scoring
  * enemy - uses: levels, movement, hitpoints, lives/deaths, attacks/defense, weapons, armor
	
###Level 1 - Here we learn the basics of extending our character class to create our first NPC and PC.
 
* build the player class - an extension of the character class
  - melee/range
  - normal moving
  - hitpoints
  - spritesheet
* build the npc class - an extension of the character class
  - normal moving
  - dialogue and conditions
  - inventory
  - spritesheet
* setup the scene using the environment class
  - define which sprites to use and how big the room is
  - define music
* define tutorial text
  - set steps and conditions that players must accomplish before tutorial is completed
* define level requirements: player gets used to controls of the character - how to use basic weapons and player learns how to use inventory
  - must talk to old cat
  - must obtain item
  - must equip item
  - must try movement (L,R,U,D and jump)
	
###Level 2 - forest to find mid-boss (a bird)

* build the enemy class - an extension of the character class
  - melee/range
  - slow - fast moving
  - varied hitpoints
  - spritesheet
* setup scene
* define level requirements (tasks to be completed)
  - navigate forest
  - level up to lvl 3
	
###Level 3 - mid-boss fight - in the nest

* build the boss class - an extension of the enemy class
  - heavy range - hits hard, long reach
  - fast moving
  - lots of hitpoints
  - spritesheet
* setup scene
* define level requirements (tasks to be completed)
  - defeat mid-boss find out that kibble was taken by Biscuit
  - learn of biscuit's weakness (if player decides to not kill birdman)
	
###Level 4 - suburbia

* build the car enemy class - an extension of the enemy class
  - normal melee - hits fair, short reach
  - varies on moving (slow to fast)
  - 10hps
  - player should avoid if possible
  - spritesheet
* setup scene
* define level requirements (tasks to be completed)
  - navigate suburbia
  - level up to at least lvl 8
  - obtain object of biscuit's weakness (optional)
    - bacon! it will attract other dogs and has a time limit
      - if times up then dogs will pile on meowski; they eat the bacon and meowski gets away
			
###Level 5 - in the dog house

* build the boss class - an extension of the enemy class
  - heavy melee - hits hard, short reach
  - slow moving
  - lots of hitpoints
  - spritesheet
* setup scene
  - setup the intro scene of this level 
    - area for monologue from Biscuit
    - then player dropped down into secret doghouse labrinth
  - area for boss fight
* define level requirements (tasks to be completed)
  - listen to monologue
  - find boss hidden in labrinth
  - fight boss and win
* boss fight
  - fight apply a time limit?
  - win/lose
    - win - save kibbles
    - lose - becomes Biscuit's new chew toy or Meowski goes hungry for that night
