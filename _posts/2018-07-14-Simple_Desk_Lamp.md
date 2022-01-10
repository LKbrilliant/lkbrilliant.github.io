---
layout: post
title:  Simple Desk Lamp
date:   2018-07-14 08:00:00 +0530
image:  2018-Simple-Desk-Lamp/img_01.jpg
# tags:   3d-printing
---
Recently I needed to replace my old desk lamp. Instead of going to a shop and buying one like a normal person, I have decided to design one for myself.

I designed the lamp to be able to fully 3D print even using a small 3D printer. I printed all the parts of this lamp using a **Creality Ender 2** printer. Ender 2 has a print volume of `150x150x200mm³`. To design this lamp, I used `Fusion360`.

![]({{ site.baseurl }}/media/2018-Simple-Desk-Lamp/img_05.jpg)
*3D model of the lamp*

![]({{ site.baseurl }}/media/2018-Simple-Desk-Lamp/img_06.jpg)
*Spiral cable protector*

For the light source, I used a LED light panel with `36` LEDs (`5730` LEDs). That might have been overkill for a desk lamp. Therefore, I have decided to change the color of half of the LEDs. The panel originally contained only cool white LEDs. I de-soldered `18` LEDs and replaced them with warm white ones.

![]({{ site.baseurl }}/media/2018-Simple-Desk-Lamp/img_02.jpg)
*Warm white light*

The original PCB design needed `53V` volts to properly function (LED configuration:`2p18s`). Since I didn’t have a high voltage source, I’ve reworked the PCB for the LEDs to work with `5V`. Then, all I had to do was connect a `5V` phone charger to it. To get a diffused light, I’ve added a hand-sanded acetate sheet to the front.

![]({{ site.baseurl }}/media/2018-Simple-Desk-Lamp/img_03.jpg)
*Sanded acetate sheet as the light diffuser*

When replacing the cool LEDs with warm ones, I distributed them evenly across the PCB. Later, I added a two-way switch to the back of the lamp to switch between two colors.

![]({{ site.baseurl }}/media/2018-Simple-Desk-Lamp/img_04.jpg)
*Addition of warm white LEDs to the PCB*

Initially, I wanted to add brightness control circuits for both colors. So, I’ve placed two holes on the lamp base to mount two potentiometers, but later, when testing, I realized that I did not need to control the brightness. Since I printed it before the testing, there are two holes left on the base. (Design Files do not contain these holes).

As for further modifications, I’ve mounted several Li-Ion batteries to the lamp base and added a USB charger/discharger module. Now, I can use the lamp for up to `4-5` hours without plugging it into a wall outlet.

## Design Files
You can download all the design files of this project on my [Thingiverse](https://www.thingiverse.com/thing:2855826) page.