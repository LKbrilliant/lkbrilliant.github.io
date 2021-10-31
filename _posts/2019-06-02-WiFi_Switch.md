---
layout: post
title:  WiFi Switch
date:   2019-06-02 08:00:00 +0530
image:  2019-WiFi-Switch/img_01.jpg
---
This wall outlet can turn On/Off any device which is plugged into it. It uses an ESP8266-01 module to connect to the home network over WiFi.

Recently I wanted to remotely turn on/off a device which is connected to a wall outlet. Building an RF transmitter and a receiver was an option, but why build two separate RF units when we already have WiFi all around us.

So, instead of trying to integrate WiFi capabilities into the device, I've decided that it is more useful to build a wall outlet adapter which can be controlled over WiFi.

Since I had several of these universal travel adapters lying around, I used them as reference for my designs. 


🛠 Bumps!!

During soldering I found out that I've made some mistakes on this version(V1) of the board and I correct them using the old fashion way.


Other than that I've encountered some issues when using the GPIO2 pin of the ESP8266-01 with the relay. When booting up GPIO2 output a small pulse, which activates the relay interrupting the booting of ESP module. this issue was resolved by changing the pin to GPIO3.