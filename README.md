QMK-keyboard  
Files for the different layouts for my KBD67 rev2.   
 
Basically in this respository you wil find the files for the layouts for my keyboar.  
I have 2 layouts, one being a VIA compatible layout you can just load to your own keyboard from the VIA software.  
The other one is a .c file where i explicitly create the layout and i also create two functions to use the backlight of the pcb as a caps lock.  

I have been using this layout for the last year, until i applied some case foam to better up the sound of the keyboard and now i just used the VIA layout and a white LED soldered to the caps lock.


On the qmk folder you will find 3 files:  
rules.mk - Basically it just the default one, i didt change anything, i just copied from another layout.  
config.h - Same as rules.mk, i just got the default one from another layout.  
keymap.c - .c file where the real layout is defined. The first array you will find is the layer 0 where all the normal keys are located and where the only difference is the far right column where i have media keys to Play/Pause, Previous, Next and Delete.  
The second array is the layer 1 where you will find some lighting keys for the brightness, Hue, On/Off and some different modes like breathing etc.  

If you dont understand the keycodes, you can check them here: https://beta.docs.qmk.fm/using-qmk/simple-keycodes/keycodes


In the VIA folder you will find a json file that defines the layoyut and that you can just upload to VIA and flash the layout into your board.  
