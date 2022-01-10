---
layout: post
title:  Ball Balancing Bot
date:   2017-09-25 08:00:00 +0530
image:  2017-Ball-Balancing-Bot/img_01.jpg
# tags:   computer-vision pid exhibit
---

This is one of the projects I build as an exhibit during my university freshman year. In this project, a ping-pong ball was balanced on a small servo-controlled platform. The platform has two degrees of freedom (2-DoF) and it was controlled using two 5V servos motors. To track the ball on the platform I used a vision-based technique.

A USB camera was mounted on top of the apparatus to track the position of the ball relative to the center of the platform. Since I used a simple color tracking technique for tracking the ball, I've added some white LEDs to the camera to get a fixed lighting condition. This allowed me to track the ball consistently in differently lit environments. 

![]({{ site.baseurl }}/media/2017-Ball-Balancing-Bot/img_03.jpg)
*USB Camera*

The programing to detect the ball position and control the servos was coded using python. The python script uses [OpenCV](https://opencv.org) to analyze the camera feed. After calculating the distance to the ball from the center of the platform, the control angles of the servos were calculated using two [PID](https://en.wikipedia.org/wiki/PID_controller) controllers. 

An *Arduino Nano* board was used to control the actual servo motors. The calculated angles were sent from the computer to the Arduino board through the [Firmata-protocol](https://github.com/firmata/arduino).

![]({{ site.baseurl }}/media/2017-Ball-Balancing-Bot/img_02.jpg)
*An Arduino Nano board was used to control the servos*

## Balancing on the center
The following video shows how the ball is balancing on the platform. Here you can see how small deviations of the ball from the center are detected by the camera and corrected by the servos.

<video height="480" controls>
  <source src="/media/2017-Ball-Balancing-Bot/vid_ball_center.mp4" type="video/mp4">
</video>

## Trying to move on a circle
In this example, the set point where the ball is supposed to settle on is moving in a circle. So, the ball is constantly trying to catch up to it by following a circular path.

<video height="480" controls>
  <source src="/media/2017-Ball-Balancing-Bot/vid_ball_circle.mp4" type="video/mp4">
</video>

## Source Files
You can find the source code of this project on my GitHub repository: [Ball-Balancing-Bot](https://github.com/LKbrilliant/Ball-Balancing-Bot)
