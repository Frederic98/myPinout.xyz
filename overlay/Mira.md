<!--
---
name: Mira board
class: board
type: power,io,display,motor,multi
formfactor: Custom
manufacturer: Frederic
description: A board for Mira
github: https://easyeda.com/Frederic98/mira
schematic: https://easyeda.com/Frederic98/mira
image: 'mira.png'
pincount: 40
eeprom: no
power:
  '1':
  '2':
  '4':
  '17':
ground:
  '6':
  '9':
  '14':
  '20':
  '25':
  '30':
  '34':
  '39':
pin:
  '8':
    name: LED MOSI
    mode: spi
  '10':
    name: LED SCLK
    mode: spi
  '11':
    name: Servo 0
    mode: output
  '13':
    name: Servo 1
    mode: output
  '15':
    name: Servo 2
    mode: output
  '16':
    name: Fan PWM
    mode: output
  '18':
    name: Display backlight
    mode: output
    active: low
  '19':
    name: Display MOSI
    mode: spi
    active: high
  '21':
    name: Display MISO
    mode: spi
  '22':
    name: Display D/C
    mode: output
  '23':
    name: SPI SCLK
    mode: spi
  '24':
    name: Display CS0
    mode: output
    active: low
  '26':
    name: Display CS1
    mode: output
    active: low
    
  '3':
    mode: i2c
  '5':
    mode: i2c
  '12':
    mode: i2s
  '35':
     mode: i2s
  '38':
     mode: i2s
  '40':
     mode: i2s
  '32':
    name: GP12 pin 4
  '33':
    name: GP12 pin 3
  '29':
    name: RGB LEDs enable pin
    mode: output
    external_pull: up
    active: high

-->
#Mira board

The Mira board is an addon for a Raspberry Pi 4 to connect components of Mira to the RPi.  
It has connections for 3 servo motors for yaw, pitch and roll movements, 2 connectors for ST7735 TFTs for the eyes,
a connector for an APA102 LED strip, and a connector for a 4-pin PWM fan running at 5V.
Additionally, it has a connection to supply 5V to the whole system to power the Pi and components.
