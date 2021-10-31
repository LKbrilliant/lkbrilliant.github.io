---
layout: post
title:  Security System
date:   2019-02-14 08:00:00 +0530
image:  2019-Security-System/img_04.jpg
---
If there is any disturbance detected while the system is armed the owner will receive a call and the alarm will go off. This system is intended to use in a small room or a small area because of the RCWL-0516 has a limited range.

Nowadays anyone with a basic understanding of electronics can build their own security systems with the help of microcontrollers like Arduino development boards. This is my take on that. 

My family owns a small grocery store, and due to several brake-ins in the nearby area, I’ve decided to build this simple security system.

Basic diagram:

![]({{ site.baseurl }} /media/2019-Security-System/Security_system_diagram.png)
*Basic module connections*

Features:

- Only the key can arm or disarm the device
- When the system is turned on using the key there will be a couple of minutes before it armed itself providing several minutes to the owner to close the shop.
- Since I’m using a pre-paid package for the sim card in the SIM800L module, during the arming sequence the system will check the available credit balance on the SIM card by USSD code. If the balance is within a critical range the owner will be notified by an SMS. To save credit, when the balance goes below the critical range the owner will not receive any further messages.
- After the arming sequence is completed, if the system is triggered it waits some predetermined period for the system to be disarmed using the key in case the owner is the one who triggered the system. Since we do not want to sound the alarm when the store opens in every morning.
- In case of a break-in, if the system is not disarmed after an above mentioned period, the alarm will go off and the owner will receive a call from the system.
- The system primarily powered by the main AC power line. In case of a power outage or a deliberate power cut, the system will power itself using backup batteries(2x18650-Li-Ion).
- In case of a Low Battery Level detection, the owner will be notified by an SMS
For visual indication, I’ve used an custom-made LED bar consisting of 8 LEDs (0603-SMD)   

![]({{ site.baseurl }} /media/2019-Security-System/trig.gif)
*LED bar when the system is triggred*

![]({{ site.baseurl }} /media/2019-Security-System/waiting.gif)
*Waiting before the system is fully armed*
