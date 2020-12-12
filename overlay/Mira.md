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
#Mira

Mira is a small robot designed by Pixar 3D artist Alonso Martinez. He created the robot to bring a character to life, just like in a move, but making it possible to interact with them. The goal was to create a very simple robot that still had a lot of personality. It consists of a partial sphere with a head that moves over it. Inside the body is a joystick mechanism with three servo motors that make the head move around. In the head are two screens, to animate the eyes, and a camera so that it can perceive the world around it.