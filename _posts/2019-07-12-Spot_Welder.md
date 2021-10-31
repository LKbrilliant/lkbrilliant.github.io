---
layout: post
title:  Spot Welder
date:   2019-07-12 08:00:00 +0530
image:  2019-Spot-Welder/img_01.jpg
---

When connecting 18650 Li-ion cells to build battery packs, soldering conductors directly to the cells is a bad idea. The best possible way is to spot weld metal strips to the batteries. But welding machines are usually expensive. There are several ways that you could build a spot welder. All you need is a sufficient enough current source to heat up and weld two metals together.

Current is the flow of electron through a conductor. Due to the internal resistance of conductors the kinetic energy of electrons will convert into thermal energy. When the current is high enough the generated heat could melt the metal conductor. This is the basic principle of spot welding. 

Electrodes of spot welders are made from highly conductive metals like copper to keep them from melting.

Transformers in microwave ovens are designed to step up the mains voltage to 2kV. By replacing the secondary coil with a coil of fewer turns, the output voltage can be stepped down. 

Since the input and the output power should be the same, by decreasing the voltage it will be able to produce a large amount of current. To accommodate this current, a large diameter wire must be used. I've used a 25 mm² wire and it produced about 2.6V at the output. Since this voltage is very low, it is not enough to shock someone.

To control the amount of time for a weld, a timer module(XY-WJ01) was employed. The minimum delay period is 0.01s. So the power that goes into a weld can be adjusted accordingly.

The enclosure and the foot-switch were 3D printed. The handle of the enclosure is reinforced by nuts and screws.

The design of the foot-switch is inspired by Adafruit's USB foot-switch design. A 3.5mm headphone jack is used to connect the foot-switch to the welder.

Update: 06.03.2020
This battery pack was built by using the spot welder to use in the backup battery pack project.