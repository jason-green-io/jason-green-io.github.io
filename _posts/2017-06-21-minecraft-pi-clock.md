---
layout: single
title: "Minecraft server connected Raspberry Pi clock"
published: true
comments: true
link:
image:
  feature: 
  credit: 
---

With just a glance, I know the time, just like a clock in an item frame.


# What it displays

* sun/moon's position
* moon's phase (the brighter the more full)
* sky color, changes during sunrise and sunset


# How it works

* Python module running on the Minecraft server
  * watches level.dat file for changes
  * parses level.dat for server time
  * publishes time to AWS IoT using MQTT

* Python module running on the Raspberry Pi
  * subscribes to the servertime MQTT topic
  * updates the display when it receives a new time from AWS IoT

No mods, in fact, this works on snapshots


# Hardware

* [Raspberry Pi Zero W](https://shop.pimoroni.com/products/raspberry-pi-zero-w)
* [Blinkt! pHAT](https://shop.pimoroni.com/products/blinkt)
* USB cable
* [IKEA USB charger](http://www.ikea.com/gb/en/products/lighting/light-bulbs-accessories/koppla-3-port-usb-charger-art-20291890/)


# Why

* Because hardware hacking is fun!