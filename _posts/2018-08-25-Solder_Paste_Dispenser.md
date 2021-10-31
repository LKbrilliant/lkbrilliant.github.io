---
layout: post
title:  Solder Paste Dispenser
date:   2018-08-28 08:00:00 +0530
image:  2018-Solder-Paste-Dispenser/img_01.jpg
---
The easiest way to apply solder paste onto a PCB is by using a stencil. But when prototyping, the layout of the PCB changes over time. For small PCBs often the stencil is more expensive than the PCB itself. So, using stencils for every iteration of the board is not very cost effective.That is where solder paste dispensers come in. 

There are two types of dispensers. Not very DIY friendly air-pressure-controlled dispensers and motor-controlled dispensers. In this project I designed a Motorized dispenser which uses a screw to to convert the rotational motion into linear motion.

Most of the parts which are needed to complete the project can be 3D printed. Parts are designed to fit with standard solder paste syringes. feel free to change them however necessary. 3D model files can be found on Thingiverse - Solder Paste Dispenser

An attiny85 microcontroller is used to dive the stepper motor through a ULN2003A Darlington transistor array. Firmware for the microcontroller -  GitHub Repository


Schematics and PCB layout - EasyEDA - Solder Paste Dispenser


Due to ATtiny85 GPIO limitations this device only contains one push button. So only the forward motion can be controlled manually, backward motion is automated. Although the RESET pin of the microcontroller can be re-purposed as an IO pin with some modification to the ATtiny85 fuses, since I didn't want to complicate the project I went with one push button.

If backward motion needs to be controlled manually it can be done by either adding an extra push button to the RESET pin or changing the existing code of this project to rotate the motor backward when "double button press" registered.