## Adafruit USB Host FeatherWing with MAX3421E PCB

<a href="http://www.adafruit.com/products/5858"><img src="assets/5858.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit USB Host FeatherWing with MAX3421E. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5858

### Description

Lots of microcontrollers these days have USB ports on them, to program or debug, act like a keyboard or disk drive, or simply send data between a computer and your firmware. But did you know that you can also add a USB Host port? That means that your microcontroller project can have a keyboard or mouse or disk drive plugged into it - which opens up a huge ecosystem of common off-the-shelf devices that you can now integrate. The Adafruit USB Host FeatherWing makes it easy to add USB Host support, especially now that TinyUSB supports it in the Arduino library as a 'native' interface for host support. 

This Wing uses the MAX3421E - a tried and true USB Host chip. It uses SPI plus an IRQ pin to send data to just about any USB device. Note that because the chip is older, and you're limited to the SPI port speed, you're not going to get blazing 480Mbps high speed data transfer. But for basic HID interfacing, or even reading/writing to a Mass Storage device, it does work quite well. There's a famous USB Host Library that can be used, and it's specialty is AVR support, but also seems to support nRF52 and ESP32. We personally recommend using the TinyUSB Arduino library - however the trade-off is that the chip must have TinyUSB support already which means it's great for RP2040, ESP32-S2 or S3, nRF52840, SAMD21/51 chips. Between the two libraries, just make sure your desired Feather mainboard is supported before purchasing! 

Next to the MAX3421E we have a 5V 1A booster with 500mA fuse, which can provide a nice clean 5V from the USB or Battery power supply. An enable pin is available to power cycle when desired.

Comes as an assembled Wing with some header. Solder on the header and plug into a Feather Mainboard to expand it's capabilities! Don't forget, you need driver support for the MAX3421E (see above for chips that are known working) and unless you're using a generic mouse, keyboard, CDC serial or USB mass storage device you will also need a USB driver that knows how to talk to the device - and writing a driver is non-trivial.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
