© OELECTRIC
===============================================================================
This firmware dedicated to test output portB of PIC24EP128GP206  
Use INTOSC FRC 7.477 MHz  
Test circuit is below.  

![Test Circuit](https://github.com/OELECTRIC/MCU/blob/master/Microchip/PIC24/PIC24EP128GP206/pic/PIC24_Test1.JPG)

1.)To upload hex.  
  1.) Connect LED,R330 Ohm to port B0-B7.  
  2.)Use MPLAB X IPE to upload the HEX file to MCU via PICKIT3.  
  3.)Press reset botton the see the result.  

2. Problem.  
  1.) If PICKIT3 can't detect the MCU please check the ICSP connection and CCAP, CCORE should be 10uF according to datasheet.  
  2.) Program problem : Check the wire connection.  

