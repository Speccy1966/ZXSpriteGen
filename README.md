# ZXSpriteGen
 Sprite code for Speccy 48k

Sprite Generator 1985
D J Burt
Havensoft

This program is for the zx spectrum 48k and was used to create sprites for the game Aladdin's Cave.

Summary of keys in ZX-Spin with Joystick enabled

Left, Right, Up and Down with cursors.
RT-CTRL (joystick fire) to make a pixel black
SPACE erase a pixel
R : Reflect the sprite
A : Assemble Sprite

E : Calls data into a set of 8 sprites from an address (see SPRITES table below) and displays in the 2 sprite columns. 
C : Clear the grid
S : Saves either a data packet (only 512 bytes worth, or 8 sprites)
L : Loads in a data packet


Tutorial.
-------------

Insert SPRTGEN.MDR into ZX-SPIN or an emulator that supports Interface 1 and Microdrive files. 

Start with "run" RETURN

Select the 4th version.

Start address for data ? is 0 RETURN (this sets it to be 32768)

With Joystick enabled in ZX-SPIN use cursor keys to move around and RT-CTRL to make a black square SPACE to delete a black square. 

A : assembles sprite into memory

E : displays in the sprite columns (type 0 again when prompted for address). 

L : Loads in some data, type in "SPRITES" RETURN (this brings in all of the Aladdin's cave sprites starting at 32768)

You cany then use E : to move around the data as follows

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

Sprites can be called back onto the grid and edited then replaced into the bank of 8 with A: to assemble. 