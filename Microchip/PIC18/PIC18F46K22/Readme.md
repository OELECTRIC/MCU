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
 Connect RB0 to pull-up Switch and connected RA0 to LED.    
 If no interrupt (SW not pushed) the LED will blink on/off = 500ms.     
 If interrupt occurred (SW was pushed) the LED will blink on/off = 100ms. 10 times.   
 
## 3.UART Function
![Alt text](https://github.com/OELECTRIC/MCU/blob/master/Microchip/PIC18/PIC18F46K22/Test_Firmware/Picture/03_UART.SVG)

	3.UART.hex
	This firmware will be running the number without delay time with Baud rate = 115200.
	Use RC6 as TX and RC7 as RX. Connect to the USB to UART converter and use Arduino serial port monitor to display the value.
     
![Alt text](https://github.com/OELECTRIC/MCU/blob/master/Microchip/PIC18/PIC18F46K22/Test_Firmware/Picture/031.png)

## 4.ADC (Analog to digital Converter)
	PIC18F46K22 has ADC port up to 28 ports ( AN0 to AN27). However, For the test firmware will only test AN0(RA0) and AN27(RD7). The resolution of ADC is 10bit (0-1023).
![Alt text](https://github.com/OELECTRIC/MCU/blob/master/Microchip/PIC18/PIC18F46K22/Test_Firmware/Picture/04_ADC_UART.SVG)
### 4.1ADC0.hex
Connect Variable resistor to “RA0” (AN0) and set baud to 115200 to receive ADC value
### 4.2ADC27.hex
Connect Variable resistor to “RD7” (AN27) and set baud to 115200 to receive ADC value
![Alt text](https://github.com/OELECTRIC/MCU/blob/master/Microchip/PIC18/PIC18F46K22/Test_Firmware/Picture/041.png)

## 5.LCD I2C (5.LCD_I2C.hex)
This firmware will display the 10 bits (0-1023) ADC value read from RA0 and display on LCD I2C.
Connect the SDA to RB0 and SCL to RB1

![Alt text](https://github.com/OELECTRIC/MCU/blob/master/Microchip/PIC18/PIC18F46K22/Test_Firmware/Picture/05_LCDI2C.SVG)

