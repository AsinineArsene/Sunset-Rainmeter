# Sunset-Rainmeter
Just a few Rainmeter files
===============================================================================================================
===============================================================================================================
These are just a few Rainmeter skins that I've customized a bit.
///////VISUALIZER\\\\\\\
The visualizer skin just changes the settings for BarExtrude.ini
  I changed a few settings within the Settings.inc file


ItemColor=FFF700|FF0097|FFF700
ItemColor2=64,255,48,255
;
; Width of shapes/lines/bars
ItemWidth=4
;
; Number of shapes/lines/bars
NumOfItems=108
;
; How much to extrude line/bar/shape or max shape size for ShapeBubble
ExtrudeMax=180
ExtrudeMin=4
;
; Whether the line/bar/shape extrudes inwards or not
Inward=0

These are the only parts I changed, namely the ItemColor line so that I could get the yellow/pink gradient.
You can change the colors to your own colors by inserting different color hex codes.
I just used this site to find mine. https://htmlcolorcodes.com/
==============================================================================================================
///////CUSTOM ICONS\\\\\\\
For the custom icons, I just created a folder within Documents/Rainmeter/Skins called Custom Desktop Icons (although you can name it whatever you want).
Within that folder, you can see one called @Resources, along with an individual folder for each icon. If you want to add your own icon, you will need to create
a new folder in there.

In the @Resources folder, there's another folder called images. You store the images you want to use for the icons in that images folder.

Back to the individual folders, you just need to create a .ini file within each of them.
To do this, just create a text file and hit "save as", then save it as a .ini file rather than a .txt file.

Inside that file, Copy and paste this code:

[Template]
Meter=Image
ImageName=#@#Images\{image}.png
H={the height of your image}
LeftMouseUpAction=["{program path}"]
SolidColor=0,0,0,1
ToolTipText="{name of program}"

[Rainmeter]
Update=1000

To modify this for your own applications/icons, you just need to change these parts:
Replace {image} (yes, the brackets as well), with the name of the image (The image itself should be loacted in the Images file mentioned before)
Replace {program path} with the file path of your launcher (probably a .exe)
  I found that this worked well to find the file path if you don't already know where it is:
  Use the windows search function to find your program, right click on the program, click open file location, right click the program and hit properties, 
  and copy paste the target link into the spot in the .ini file.
Replace {the height of your image} with, well, the height of your image. In my case I used 96 since my images were 96x96
  
I know it sounds a bit tedious, but you'll get the hang of it after doing it once or twice and it really goes pretty quickly.
===================================================================================================================
In case you want to use the same type of images that I used in mine, they can be found here: https://icons8.com/icons/nolan.
I found they look best when downloaded at a higher resolution than 64px. I personally used 96px (Dont forget to change the H= to 96)
