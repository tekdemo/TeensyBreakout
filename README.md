# Teensy Breakout

A small PCB to break out a Teensy into a form factor suitable for small electronics prototyping

# Features
- Adapts Teensy pinout to Arduino shield, so existing shields can be fit to a Teensy
- Adds LiPo battery monitoring and charging capability
- Adds three wire pinouts for all pins
- All PWM outputs have an LED
- All PWM outputs connect to 3 wire servo headers that supply input or battery voltage for use with servos or motor controllers


# BOM

Due to the nature of the breakout, many components can be omitted depending on the needed sections. 

## Components 
 Part | Quantity  | Description | Part Number
---|---|---|---
 Teensy | 1 | Teensy Microcontroller | [OSH Park][oshteensy] or [Adafruit][adateensy] or 
PCB | 1 | Bare PCB | [OSH Park][pcb]
LED |11| 0603 or 0805 LED | any
1uF cap  |2| 0603 or 0805 cap | any
0.1uF cap |4| 0603 or 0805 LED | any
10uF cap |2| 0603 or 0805 cap | any
LiPO Battery |4| Any with JST connector | [Adafruit][lipo]
JST Battery Connector |4|  | [JST-PH-2-THM-RA][JST-PH-2-THM-RA]
MCP73871| 2 | LiPO Battery Management IC | [MCP73871][MCP73871]
MCP1703| 2 | 3.3V voltage regulator | [MCP1703][MCP1703]
Large (100uF+ cap) |2| 0603 or larger | any

## Pin Connections
The various use cases may or may not require some or all of these pins. Here's the most you can solder to the board in the simplest orientation

Most of these can be swapped, omitted, or assembled with small 1x3 connectors or whatever you have on hand. Otherwise, they can be purchased at [Digikey](http://digikey.com) or [Adafruit](http://adafruit.com)

Part | Quantity  | Description 
---|---|---
Arduino Sockets | 2 | 0.1" 1x8 F socket 
Arduino Sockets | 2 | 0.1" 1x6 F socket 
3 wire output headers | 2 | 0.1" 3x8 M Angle Pins 
3 wire output headers | 1 | 0.1" 3x6 M Angle Pins 
Servo output headers | 2 | 0.1" 3x3 M 90 degree Pins 
Servo output headers | 1 | 0.1" 3x4 M 90 degree Pins 

[oshteensy]: http://store.oshpark.com/products/teensy-3-1
[adateensy]: https://www.adafruit.com/product/2756
[pcb]: https://oshpark.com/import?url=https://raw.githubusercontent.com/tekdemo/TeensyBreakout/master/TeensyBreakout.brd
[lipo]: https://www.adafruit.com/categories/574
[MCP1703]: http://www.digikey.com/product-detail/en/microchip-technology/MCP1703AT-3302E-CB/MCP1703AT-3302E-CBCT-ND/3598398
[MCP73871]: http://www.digikey.com/product-detail/en/microchip-technology/MCP73871-2CCI-ML/MCP73871-2CCI-ML-ND/1680971
[JST-PH-2-THM-RA]: http://www.digikey.com/product-detail/en/jst-sales-america-inc/S2B-PH-K-S(LF)(SN)/455-1719-ND/926626

# Special Thanks

Thanks to Adafruit, who supplied the base schematic for the Battery monitor IC. Awesome work. 