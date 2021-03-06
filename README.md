# Indiana Jones and the Roleplaying Game of Doom -  RPG game
RPG game javascript - "Indiana Jones and the Roleplaying Game of Doom" 
-  Blair Erickson

# Known bugs
- Occasionally during a whip attack sequence, there's a null error of an img not being loaded. Appears to be from the script looking for an image that's already been erased. Retimed animation code to hopefully prevent.

- Occasionally background music file in m4a format will not play. Compressed to around 1 MB and it appears to have resolved bug.

# Code libraries included and used to create:

- PixiJS .v4 which handles the graphics display in javascript.
https://github.com/pixijs
- fork of open source Role Playing Game Maker v. MW Ace project skeleton template from Github for X,Y pathfinding, maps, level transporting, stat variable framework, player movement. 
https://github.com/rpgmaker
https://rpgmakermv.co/resources/
https://rpgmakermv.co/threads/creating-dialogue-using-javascript.3327/

- Victor Engine VX Scripts Javascript plugins  VE_Basic Module and VR_CharacterFrames to handle displaying sprite animations.
https://github.com/bsides/rpgvxace-scripts/blob/master/victor-engine/field/ve-fixed-parallax.rb
https://drive.google.com/file/d/0B0cSp2lASM9wV1d0cFBtZWtfZEk/view

- menu select uses VXace alternate menu systems scripts
https://rpgmaker.net/scripts/rmvxace/menusystems/

- Custom built simple animation hack on top of the framework to create the 14 frame Indy vs. Opponent cartoon effect.

- Sprite library used to build Photoshop animation templates downloaded from Spriters-Resource.
https://www.spriters-resource.com

- Indiana Jones spritesheets from archives for Lucasfilm games Indiana Jones and His Desktop Adventures as well as the 1989 Lucasfilm adventure game classic Indiana Jones and the Last Crusade.
 
- JQuery and Bootstrap are not used as the game is not mantipulating within the DOM very well when added. Planned future expansion would mix a 4-div column with content that displayeda graphic of the player's face, health, attacks recevied, and remained on screen as scenes within game area are refreshed. I ran out of time to build a player health model for this alpha version.

- custom font is Adventure by Pixel Saga

# What's next version?

- Planned longterm may include building out the engine to create an Indiana Jones Roguelike. Procedurally designed levels that matched a basic formula.

- Improve rough collision detection. I primarily relied on an event trigger system built into the grid model that came with the forked role playing game template. It checks if two actor objects are positioned on the same grid square simultaneously. As a result the collision is often missed. The boulder scene was particularly problematic and had to be hacked to cause a game over scenario upon player collision on the trigger square. Outrunning the boulder was not possible since it often failed it catch collision with player. There are better, proximity systems that can be used to better detect collisions between the player and sprite objects.



