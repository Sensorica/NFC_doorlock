This project is about developing a multi functional NFC enabled doorlock for the exterior entrance to the new SENSORICA lab space.
The proof of concept will simply provide access using NFC tags. 

TODO:
*

The first prototype is built using materials at the lab:

* Raspberry Pi Revision B
* Original door striker which takes 12-16V AC
* MFRC-522 reader/writer 
* 5V relay breakout board
* 12V AC wall wart transformer

Installation:

* NFC Reader to Raspberry Pi diagram:
  (RC522) --- (GPIO RaspPi)
     3.3v --- 1  (3V3)
      SCK --- 23 (GPIO11)
     MOSI --- 19 (GPIO10)
     MISO --- 21 (GPIO09)
      GND --- 25 (Ground)
      RST --- 22 (GPIO25)
	  
  Relay breakout:  
  
  GPIO RaspPi A & B  - http://robig.net/blog/files/images/Raspberry-Pi-GPIO-Layout-Revision-2-e1347664831557.png
  GPiO RaspPi B+ & 2 - http://www.rpi-spy.co.uk/wp-content/uploads/2012/06/Raspberry-Pi-GPIO-Layout-Model-B-Plus-rotated-2700x900.png
  
* Dependencies 
  
  Make sure SPI is enabled in the kernel.
  sudo raspi-config (change setting under *advanced*)
  
  Make sure you are root!
  
  wget http://www.airspayce.com/mikem/bcm2835/bcm2835-1.35.tar.gz
  tar -zxf bcm2835-1.35.tar.gz
  cd bcm2835-1.35
  make install
  
 


