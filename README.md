# CanHacker (lawicel) CAN adapter on Arduino + MCP2515

Testes with Arduino Nano.
On Arduino Uno have problem with too long boot period and losing first command when work with CanHacker application

## Installation

1. Install [MCP2515 Library](https://github.com/autowp/arduino-mcp2515)
2. Install [CanHacker Library](https://github.com/autowp/arduino-canhacker)
3. Configure sketch: MCP2515 CS pin, SoftwareSerial pins if required, change baudrates
4. Use with [CanHacker](http://www.mictronics.de/projects/usb-can-bus/) or CANreader (soon)

The sketch for it is here
https://github.com/autowp/can-usb

Libraries and connection diagrams for it are here
https://github.com/autowp/arduino-mcp...
https://github.com/autowp/arduino-can...

After installing the libraries you may have to edit the canhacker.h file to match the clock speed of your MCP2515 adapter. Mine is an 8Mhz adapter and the default is 16Mhz.

If you bought a Nano from eBay you may need to select Nano then select ATmega328P(Old Bootloader) to get the sketch to upload.

If you get nothing on the CANHacker software 
1. Double check you are using the correct CANbus speed for your car.
2. Check the baud rate of the Serial port is correct.
3. Check in the settings that "Listen Only" is unticked.

https://www.youtube.com/watch?v=wwq_yD-mth8
