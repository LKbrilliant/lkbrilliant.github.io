---
layout: post
title:  Simple Desk Lamp
date:   2018-07-14 08:00:00 +0530
image:  2018-Simple-Desk-Lamp/img_01.jpg
---
Recently I needed to replace my old desk lamp. Instead of going to shop and buy one, I've decided to design one for myself. 

he Lamp was designed to 3D print completely even using a small entry level printer. This one was printed with Creality Ender 2 Printer. It has a print volume of 150 x 150 x 200 mm.

All of the Design files can be found on https://www.thingiverse.com/thing:2855826

The lamp was designed using Fusion 360

For the light source I've used a LED light panel with 36 LEDs (5730 LEDs). That is an overkill for a desk lamp. The panel originally contains only cool white LEDs. So I've de-soldered 18 LEDs and replace them with warm white LEDs. The Original PCB was designed to use it with 53V (LED configuration - 2p18s). Since I didn't have a driver circuit I've redesign the PCB for LEDs to work with 5V.

Initially I wanted to add brightness control circuits for both colors so, I've added two holes on the base of the lamp to mount two potentiometers, but later when testing I realize that I don't really need to control the brightness. Since the print was done before the testing, there are two holes left on the base. (Posted design files does not contain these holes).