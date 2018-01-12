# Walrus Board

Walrus is an open-source platform for battery-powered sub-GHz and 2.4 GHz radio communication

### Dual Radios

Walrus has two radios, accessed over SPI:

* [RFM69HCW transceiver](http://www.hoperf.com/rf_transceiver/modules/RFM69HCW.html)
  for 900 MHz (also usable at 433 MHz)
* [CC2500 transceiver](http://www.ti.com/product/CC2500)
  for 2.4 GHz

### Designed for Raspberry Pi Zero W

* Raspberry Pi Zero form factor
* 40-pin Raspberry Pi GPIO connector
* HAT EEPROM

![Walrus board connected to Raspberry Pi Zero W](images/walrus_board.png)

### Battery Power Management

* JST PH 2.0mm connector for 3.7 V LiPo battery
* 500 mA battery charging when Raspberry Pi is connected to 5 V via micro-USB
* hard power-off via pushbutton or GPIO disconnects battery from Raspberry Pi
* programmable power-on via RTC alarm

### Other Peripherals

Walrus has the following I2C devices:

* Real-Time Clock (M41T62LC) with power-on alarm
* Analog-Digital Converter (ADS1015) for battery voltage and charge current measurement
* 3-axis Accelerometer (LIS3DH) with single and double-tap detection
