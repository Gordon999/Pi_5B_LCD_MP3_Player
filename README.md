# Pi_5B_LCD_MP3_Player

A simple MP3 Player and Internet Radio Player using a Raspberry Pi, 5 buttons, and 1 I2C LCD, either 16x2 or 20x4.

All buttons are connected between gpios and gnd (1k resistors in series are usually recommended), LCD connected as shown. 
Backlight control (if required) via a opto-isolator, if not then leave the supplied link in place on the LCD.

## schematic

![schematic](schematic.jpg)

5 button switches, PREVIOUS,PLAY,NEXT,VOLUME,SLEEP but they have multi purposes as shown.
## Button usage

![modes](modes.jpg)

## screenshot showing status... R for Random, G for Gapless,  S for SLEEP Timer set

![schematic](photo002.jpg)

## screenshot showing ALBUM MODE, GAPLESS ON and SLEEP Timer set.

![schematic](photo001.jpg)


At boot it will look for mp3 tracks in '/home/pi/Music/artist name/album_name/tracks', 
and/or on a USB stick, under /media/pi/usb_stick_name/artist name/album_name/tracks

To install copy 5B_LCD_MP3_player.py to /home/pi

and then

sudo apt-get install mplayer

sudo pip3 install mutagen

to run python3 5B_LCD_MP3_player.py
