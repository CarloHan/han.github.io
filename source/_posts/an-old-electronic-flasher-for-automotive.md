---
title: An old electronic flasher for automotive
tags:
  - analog cicuit
  - flasher
  - multivibrator
top: 26
categories:
  - - HW
description: >-
  Analyzing and simulating the working principle of an old electronic flasher.
  This flasher control unit is used to control the position, direction and
  emergnecy lights flashing on vehicle.
abbrlink: 12487
date: 2021-01-12 17:46:50
---

<style>
  .box {width:60%; text-align:center; font-size:10px; margin:0 auto;}
  .box img {border-radius: 10px;}
</style>

<div class="box">
  <img src="https://raw.githubusercontent.com/CarloHan/pic-blog/master/pictures/an%20old%20flasher.jpeg" alt="electric flasher"/>
</div>
<br />

Last month I opened an electronic flasher for automotive, it's an old version which designed by transister, not IC. I have been busy testing a new BMS all month, and until now I have no time to talk about this component. The schematic copy as below.

<div class="box">
  <img src="https://raw.githubusercontent.com/CarloHan/pic-blog/master/pictures/flasher%20schematic.png" alt="schematic" />
  Schematic
</div>

Pin B is the positive 12V, pin E is ground, pin L is connected to a direction light lever. It was replaced by a 820ohm resistor. Let's see what will happen in the simulation.

<div class="box">
  <img src="https://raw.githubusercontent.com/CarloHan/pic-blog/master/pictures/flasher%20simulate.png" alt="simulation" />
  Voltage(LED) - T
</div>

The direction light flashes every 300 ms, and there is no clock no timer no mcu, only a little basic electronic components. Let's analyse how it is realized.
