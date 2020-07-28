# STM32F429ZGT6

![Alt text](https://img.directindustry.com/images_di/photo-mg/33699-12766624.jpg)
![Alt text](https://github.com/OELECTRIC/MCU/blob/master/STmicro/STM32F429ZGT6/Test_Firmware/Picture/ARM.png)

## The test firmware will use a High-speed internal oscillator (HIS) 16MHz, Not required external crystal for the device for this testing.

### 01_Blink.bin
          Connected the LED with Resistor 330 or 1K to PB0. The LED will on/off 500ms.
### 02_UART_9600.bin
	Use PC11 as TX and PC12 as RX. Connect the USB to UART converter to these ports then set baud as 9600. The number will count without delay time.
 
### 03_LCD_I2C.bin
Use PD4 as SDA and PD5 as SCL. Connect to the LCD I2C (Can be use both 16X2 and 20X4). The number will count without delay time.
Note: Please considered the EMC may cause the display error. Use shield or coaxial wire for better data transfer. 
### 04_ADC.bin
Use PD4 as SDA and PD5 as SCL. Connect to the LCD I2C (Only supported LCD I2C 20X4).
Connect the variable resistor to PA5 to receive voltage divider value.
The ADC will display on LCD I2C on 12bits resolution (0-4095). 
### 05_INT.bin
This firmware for interrupt testing.
-Connected PA0 with pull-up resistor and button.
-Connected PB0 with LED series with Resistor 330 or 1K.
- Connect PD4 as SDA and PD5 as SCL to the LCD I2C (Only supported LCD I2C 20X4).
After upload program. The number will count up with 250ms delay time. When the button has been pushed. The interrupt will activate the number stop counting and LED will blink 10 times. After that the number will start counting start from previous number.


