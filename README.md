# Pico8-MultipleChoiceEngine
A small multiple choice interactive fiction engine compatible with Jari Komppa's MuCho ZX Spectrum tag languaje.

It includes a complete game: "Blood of Dracula Pico-8 Adventure", you can play it online at this link:

https://furilloproductions.itch.io/blood-of-dracula-pico8-adventure

License: unlicense

Note: it is provided "as-is"... unfortunatly I do not have so much time for reviews or support, 
I apologize beforehand. Please feel free to make your own versions of the engine.

# How to use it:

1. Create a new Pico-8 empty project.

2. Copy-paste the content of "MultipleChoicePico8Engine.txt" inside the code page.

The game and the multiple choice engine are all together inside the code page. 

3. The "mucho_compatible_text" long string variable at the beginning of the code is the MuCho ZX Spectrum compatible game script.
It follows the rules of Jari Komppa's MuCho tag language:

https://solhsa.com/mucho/mucho.html

4. Once you make your own game or if you want to test the included game, just RUN the project.
   
5. It will work WITHOUT music and IMAGES.

6. How do I add images and music to my projects?

You can create up to 16 images for this engine. There are two steps:

First Create 4x4 images in the 0,1,2,3
tile banks, they are numerated (starting from left of bank 0 up to right of bank 3) 
0,1,2,3,4,5,6... up to 15 (so there are 4 4x4 tile images on each bank). 
This images can be called using the tag $I numberofimage, e.g. $I 0 will
load the bank 0 first image on the left. E.g. $I 9 will load the 
bank 3 second image starting from left, etc.

!how-to1.png

!how-to2.png

!how-to3.png

!how-to4.png

Then go to the map screen and put the images as if they were a map, 
the first 8 images in the top left part of the map, and the
rest of the images in the block below the first one. So if you 
see the map you will see all the images as if they were a map.

This is important, because the engine will show the images as
if they were a block from the map. You just need to make
the arrangement as explained above, the engine will do the rest.

You can add as many music as Pico-8 let you depending on the memory left.
Music is added using a $M musicidtag, where musicidtag is a number
starting from 0 onwards... (same natural order than the added songs)

E.g. $M 0  will play the first music available at the music list of the project.

I hope you enjoy it, cheers! :)


