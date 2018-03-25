# 8088 CPU card for the CBM-II computers
 
This is the replica of the 8088 processor card for the Commodore CBM-II computers, made by Ruud Baltissen. The replica is 100% compatible with the original card.

The following changes have been made to the replica:

* JP3 was added to allow installing the 8087 coprocessor. This jumper is missing from the original card.
* Card EPROM has been enlarged to fill the whole F000 segment.

You can use the original MS-DOS 1.25 and CP/M-86 1.1 software with the card. However, the ROM also contains the 0.64 version of PC compatilibility layer, allowing it to boot newer versions of PC-DOS and MS-DOS.

The enlarged EPROM containg boot files of PC-DOS 3.2. To boot this system, create a disk from the attached *empty.d80* or*empty.d82* image, and press Shift+RunStop to bootstrap the disk. The disk will load the 6509 part of the IPC library into memory and boot PC-DOS from the EPROM.   

The card has been successfully tested with a high-profile CBM-II machine, using either 8088 or V20 processor, as well as 8087 coprocessor. 

## TODO:

* Change the (very hard to obtain) 6525 chip to standard 8255 I/O chip. 
* Implement SPI interface to allow connecting a SD card, RTC chip etc.
* Add a small EPROM at $1000 containing the 6509 code, so that diskless boot is possible.


 



