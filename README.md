# Pi_5B_LCD_MP3_Player

A simple MP3 Player using a Raspberry Pi and 5 buttons, and 1 I2C LCDs, either 16x2 or 20x4

All buttons are connected between gpios and gnd (1k resistors in series are usually recommended), LCD connected as shown. Backlight control (if required) via a opto-isolator, if not then leave the supplied link in place on the LCD.

5 button switches, PREVIOUS,PLAY,NEXT,VOLUME,SLEEP but they have multi purposes as shown.



At boot it will look for mp3 tracks in '/home/pi/Music', and on a USB stick with the format /Artist/Album/Tracks

To install copy 5B_LCD_MP3_player.py to /home/pi

and then

sudo apt-get install mplayer

sudo pip3 install mutagen

to run python3 5B_LCD_MP3_player.py
