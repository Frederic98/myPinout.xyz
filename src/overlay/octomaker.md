<!--
---
name: Octomaker
class: board
type: 3D-printer
formfactor: Custom
manufacturer: Frederic
description: An add-on board for the RPi to talk to the Ultimaker 2 mainboard
github: https://easyeda.com/Frederic98/octomaker
schematic: https://easyeda.com/Frederic98/octomaker
image: 'octomaker.png'
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
  '3':
    mode: i2c
  '5':
    mode: i2c
  '7':
    name: OLED reset
    mode: output
    active: low
  '8':
    name: UART Tx
    mode: output
    active: high
  '10':
    name: UART Rx
    mode: output
  '11':
    name: Button push
    mode: input
  '13':
    name: Button A
    mode: input
  '15':
    name: Button B
    mode: input
  '16':
    name: Power detect
    mode: input
  '18':
    name: Output enable
    mode: output
    active: low
  '19':
    name: SPI MOSI
    mode: output
    active: high
  '21':
    name: SPI MISO
    mode: input
  '22':
    name: SPI reset
    mode: output
    active: low
  '23':
    name: SPI SCLK
    mode: output
    active: high
  '32':
    name: Buzzer
    mode: output
    active: high
i2c:
  '0x3C':
    name: OLED
    device: SSD1306
  '0x03':
    name: x
    device: x
  '0x4F':
    name: Temperature sensor
    device: LM75
  '0x60':
    name: Button LEDs
    device: PCA9632
  '0x70':
    name: x
    device: x

-->
#Octomaker

Octomaker is an addon for a raspberry pi to communicate with an Ultimaker 2 3D-printer.
It uses UART to send GCodes to the motion controller, and SPI to program new firmware on the ATmega2560.

The board also has connections to which the Ulticontroller can be connected, providing access to the OLED, rotary encoder, buzzer and other stuff.
