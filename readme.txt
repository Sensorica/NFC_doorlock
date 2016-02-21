This project is about developing a multi functional NFC enabled doorlock for the exterior entrance to the new SENSORICA lab space.
The proof of concept will simply provide access using NFC tags. 

TODO:
*

The first prototype is built using materials at the lab and NeoPixel strip donated by the KING:

* Arduino UNO R3
* Original door striker which takes 12-16V AC
* MFRC-522 reader/writer 
* 5V relay breakout board
* 12V AC wall wart transformer
* NeoPixel LED strip (108 LDED's)

Installation:

* NFC Reader to Raspberry Pi diagram:
  
     3.3v --- 3.3v Pin
  SDA(SS) --- Pin 10 (Configurable)
      SCK --- Pin 13 / ICSP-3
     MOSI --- Pin 11 / ICSP-4
     MISO --- Pin 12 / ICSP-1
      GND --- GND Pin
      RST --- Pin 9 (Configurable)
	  
* Relay breakout:

       5v --- 5v Pin
      GND --- GND Pin
   Signal --- Pin 4
   
* NeoPixel light strip:

       5v (red) --- 5v Pin
    GND (black) --- GND Pin
 Signal (white) --- Pin A0
  
  
* Dependencies 

- Mifare RC522 device library
- Adafruit Neo Pixel library
  
 
  
 


