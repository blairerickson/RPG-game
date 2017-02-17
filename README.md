# Indiana Jones and the Roleplaying Game of Doom -  RPG game
RPG game javascript - "Indiana Jones and the Roleplaying Game of Doom" 
-  Blair Erickson

# Known bugs
- Occasionally during a whip attack sequence, there's a null error of an img not being loaded. Appears to be from the script looking for an image that's already been erased. Retimed animation code to hopefully prevent.

- Occasionally background music file in m4a format will not play. Compressed to around 1 MB and it appears to have resolved bug.


Code uses mutliple libraries including: 
- PixiJS .v4 which handles the graphics display in javascript.

- An open source fork of the Role Playing Game Maker .VW Ace project skeleton from Github for player movement

- Javascript plugins for VE_Basic Module and VR_CharacterFrames to handle displaying sprite animations

- Custom built simple animation hack on top of the framework to create 14 frame Indy vs. Nazi cartoon

- Sprite library used to build Photoshop animation templates downloaded from Spriters-Resource 

- Indiana Jones sprites from archives for Lucasfilm games Indiana Jones and His Desktop Adventures as well as the 1989 Lucasfilm adventure game classic Indiana Jones and the Last Crusade
