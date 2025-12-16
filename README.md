# Pico8-MultipleChoiceEngine
A small multiple choice interactive fiction engine compatible with Jari Komppa's MuCho ZX Spectrum tag languaje.

It includes a complete game: "Blood of Dracula Pico-8 Adventure", you can play it online at this link:

https://furilloproductions.itch.io/blood-of-dracula-pico8-adventure

License: unlicense

Note: it is provided "as-is"... unfortunatly I do not have so much time for reviews or support, 
I apologize beforehand. Please feel free to make your own versions of the engine.

# Please note

You need to know the basics about Pico-8 before using this engine. Starting from zero will be hard. 

Please check out this great link for plenty of Pico-8 resources and manuals:

https://github.com/pico-8/awesome-PICO-8

# How to use this engine:

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

E.g. in the sample game, the tile banks 0,1,2,3 have 4 images of 4x4 tiles (in Pico-8 tile=cell) as
follows:

![a](https://raw.githubusercontent.com/Iadvd/Pico8-MultipleChoiceEngine/refs/heads/main/how-to1.png)

![b](https://raw.githubusercontent.com/Iadvd/Pico8-MultipleChoiceEngine/refs/heads/main/how-to2.png)

![c](https://raw.githubusercontent.com/Iadvd/Pico8-MultipleChoiceEngine/refs/heads/main/how-to3.png)

![d](https://raw.githubusercontent.com/Iadvd/Pico8-MultipleChoiceEngine/refs/heads/main/how-to4.png)

Then go to the map screen and put the images as if they were a map, 
the first 8 images in the top left part of the map, and the
rest of the images in the block below the first one. So if you 
see the map you will see all the images as if they were a map.

E.g. in the sample game, if you go to the map screen, you will see the images written at the map, the first 8 ones in the left-top map position, the following 8 images just below them as follows:

This is a zoom out so you can see both files of images at the map screen:

![e](https://raw.githubusercontent.com/Iadvd/Pico8-MultipleChoiceEngine/refs/heads/main/how-to5.png)

Zoom-in, basically we put the images inside the map, as if they were map tiles:

![f](https://raw.githubusercontent.com/Iadvd/Pico8-MultipleChoiceEngine/refs/heads/main/how-to6.png)

This is important, because the engine will show the images as
if they were a block from the map. You just need to make
the arrangement as explained above, the engine will do the rest.

You can add as many music as Pico-8 let you depending on the memory left.
Music is added using a $M musicidtag, where musicidtag is a number
starting from 0 onwards... (same natural order than the added songs)

E.g. this is the music of the sample game, only three songs, so I am using $M 0 or $M 1 or $M 2 in the sample game:

![g](https://raw.githubusercontent.com/Iadvd/Pico8-MultipleChoiceEngine/refs/heads/main/how-to7.png)

E.g. $M 0  will play the first music available at the music list of the project.

I hope you enjoy it, cheers! :)


