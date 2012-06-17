v1.3: Changed to the same micro-SD card PCB footprint as the Kliment SDRamps board, using some generic micro-SD card socket from eBay.
Also changed to self-oscillating through-hole buzzer, removed buzzer drive oscillator, and reduced prototyping hole number to keep total drill hits less than 300.

Pinout: The pinout takes the 20-way cable from the display board (IDC header plug) and splits it in half, with 13 wires going to 13 contiguous pins on the 18-way single-row
expansion header on the edge of the RAMPS board, and 7 wires going to an 8-pin dual-row IDC header plug which connects to the SPI header. So you can just take a 13-way
single-row 0.1" IDC ribbon cable header plug and a 8-pin dual-row 0.1" IDC ribbon cable header plug and just crimp them on and plug them straight on without any crossovers or
the like.

Note that the 8th pin on the SPI header plug is not connected to the cable.

This is the pinout for the 20-pin (dual-row) IDC ribbon cable header on the display board:

1: RS (Pin 18 on 18-pin RAMPS expansion header, Arduino pin 16)  
2: EN (Pin 17 on 18-pin RAMPS expansion header, Arduino pin 17)  
3: D4 (Pin 16 on 18-pin RAMPS expansion header, Arduino pin 23)  
4: D5 (Pin 15 on 18-pin RAMPS expansion header, Arduino pin 25)  
5: D6 (Pin 14 on 18-pin RAMPS expansion header, Arduino pin 27)  
6: D7 (Pin 13 on 18-pin RAMPS expansion header, Arduino pin 29)  
7: Sw (Pin 12 on 18-pin RAMPS expansion header, Arduino pin 31)  
8: Buzzer (Pin 11 on 18-pin RAMPS expansion header, Arduino pin 33)  
9: Encoder A (Pin 10 on 18-pin RAMPS expansion header, Arduino pin 35)  
10: Encoder B (Pin 9 on 18-pin RAMPS expansion header, Arduino pin 37)  
11: Backlight (Pin 8 on 18-pin RAMPS expansion header, Arduino pin 38)  
12: TC2 (Pin 7 on 18-pin RAMPS expansion header, Arduino pin 41)  
13: TC3 (Pin 6 on 18-pin RAMPS expansion header, Arduino pin 43)  

14: +5V (Pin 1 on RAMPS 8-pin SPI header, 8x2 IDC header plug)  
15: SD CS (Pin 2 on RAMPS SPI header, Arduino pin 49)  
16: MISO (Pin 3 on RAMPS SPI header, Arduino pin 50)  
17: MOSI (Pin 4 on RAMPS SPI header, Arduino pin 51)  
18: SCK (Pin 5 on RAMPS SPI header, Arduino pin 52)  
19: TC1 CS (Pin 6 on RAMPS SPI header, Arduino pin 53)  
20: Gnd (Pin 7 on RAMPS SPI header)

(Note: Pin 8 on 8-pin IDC header plug is not connected.)

![](https://github.com/lukeweston/RAMPSdisplay/raw/master/v1.3/RAMPSdisplay-pcb.png)
