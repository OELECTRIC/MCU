# PIC18F46K22
![Alt text](https://www.microchip.com/_images/products/medium/a6d7ff1e606a7ffb60475e93c1b59c99.png)

Use 16MHz precision internal oscillator: OSCCON = 0x70;
No need for an external crystal for the test. (If the crystal has been installed. No problem for the test)

## 1.Blink
![Alt text](https://github.com/OELECTRIC/MCU/blob/master/Microchip/PIC18/PIC18F46K22/Test_Firmware/Picture/01_BLK.SVG)

### 1.1Blink_INT_A0.hex
     To blink LED connected to RA0. 0.5ms On and 0.5ms Off.

### 1.2Blink_INT_B0.hex
    To blink LED connected to RB0. 0.5ms On and 0.5ms Off.

## 2.Interupt
![Alt text](https://github.com/OELECTRIC/MCU/blob/master/Microchip/PIC18/PIC18F46K22/Test_Firmware/Picture/02_INT.SVG)

### 2.1Interupt_RB0.hex   
### Connect RB0 to pull-up Switch and connected RA0 to LED.    
### If no interrupt (SW not pushed) the LED will blink on/off = 500ms.     
### If interrupt occurred (SW was pushed) the LED will blink on/off = 100ms. 10 times.    

