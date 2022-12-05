# yh-028 display

This is information about the mystery TFT display found in My-Arcade mini arcade machines.  This is the one I dismantled to investigate the display.  
![image](https://user-images.githubusercontent.com/14888910/205723200-45ef9e3c-4e67-40b9-b353-c3d8db31a363.png)


This display will have on the back YH-028v0.1.1 on the back.  
![image](https://user-images.githubusercontent.com/14888910/205723860-62488b0c-b11e-4ffd-ba19-35e49a89a53f.png)


Driver: ILI9341 8 Bit Parallel.  
Resolution: 320 x 240.

## Pinout.  
The display has a  1 cm wide ribbon cable - a breakout board is available, however the pins seemed to be reversed on there.  So, for convenience I've put both pin number of the ribbon cable ( first number), and the pin number of the breakout board.

| Pin           | Function |
| ------------- | ---------|
| 1 or 24       | 3.3v     |
| 2 or 23       | GND.     |
| 3 or 22       | LED Backlight 5v |
| 4 or 21       | Reset    |
| 5 or 20       | TFT_CS   |
| 6 or 19       | TFT_DC   |
| 7 or 18       | TFT_WR   |
| 8 or 17       | TFT_RD   |
| 9 or 16.      | TFT_D0   |
| 10 or 15      | TFT_D1   |
| 11 or 14      | TFT_D2   |
| 12 or 13      | TFT_D3   |
| 13 or 12      | TFT_D4   |
| 14 or 11      | TFT_D5   |
| 15 or 10      | TFT_D6   |
| 16 or 9       | TFT_D7   |
| 17-24 or 8-1. | Not Connected|

After connecting to an ESP32, and with the library 'eTFT_SPI', with the setting "Setup14_ILI9341_Parallel",  I get this:   
![image](https://user-images.githubusercontent.com/14888910/205724639-276af5fb-23f0-4a5f-a22e-0919ae720730.png)

