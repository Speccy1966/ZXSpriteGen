# ZXSpriteGen (v12 on TAP)
 Sprite code for Speccy 48k

Sprite Generator 1985
D J Burt
Havensoft

This program is for the zx spectrum 48k and was used to create sprites for the game Aladdin's Cave.

Summary of keys in ZX-Spin with Joystick enabled 

Left arrow (or 5 on TAP)

Right arrow (or 8 onTAP)

Up arrow (or 6 on TAP)

Down arrow (or 7 on TAP) 

RT-CTRL (joystick fire or 0 on TAP) to make a pixel black

SPACE erase a pixel

R : Reflect the sprite

Z : Shift Sprite Left (TAP version only)

X : Shift Sprite Right (TAP version only)

A : Assemble Sprite

E : Calls data into a set of 8 sprites from an address (see SPRITES table below) and displays in the 2 sprite columns. 

C : Clear the grid

S : Saves either a data packet (only 512 bytes worth, or 8 sprites) - or the program (and the code on TAP)

L : Loads in a data packet (can be as up to 8kB - see addresses of Aladdin sprites below)

Addresses for Aladdin's Cave Sprites (in Game and with the Editor)

Address	Character in SPRITES
32768 	Aladdin Left
33024	Aladdin Right
33280	Aladdin Climb
33536	Monkey Left
33792	Monkey Right
34048	Monkey Climb
34304	Genie
34650	Bird R
34816	Bird L
35072	Spider
35328	Rock
35584	Bat R
35840	Net
36096	King with Sword
36352	Wizard
36608	Spider Again
37120	Dolphin R
37376	Dolphin L
37632	Port Cullis
38144	Skull
38400	Robot
38912	Flag
39168	Anchor
39424	Geyser
39936	Butterfly

Tutorial.
-------------

1. Using the .mdr with Spin or Fuse

Insert SPRTGEN.MDR into ZX-SPIN or an emulator that supports Interface 1 and Microdrive files. 

Start with "RUN" RETURN

Select the 4th version.

Start address for data ? is 0 RETURN (this sets it to be 32768)

L : Loads in some data, type in "SPRITES" RETURN (this brings in all of the Aladdin's cave sprites starting at 32768)


2. Using the .TAP version

This is set up to load in the Aladdin Sprites at start.

In Fuse or Spin just load in SprGen12.tap and then "RUN" RETURN

Start address for data ? is 0 RETURN (this sets it to be 32768)
 

Use E to bring in sprites from a Valid address 
With Joystick enabled in ZX-SPIN use cursor keys to move around and RT-CTRL to make a black square SPACE to delete a black square. 
A : assembles sprite into memory



