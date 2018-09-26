---
layout: post
title:  "Project 1: Proposal"
date:   2018-09-26 4:38:53 -0600
categories: [ Atlas-Object ]
---
## Goal

Create a digital hardware monophonic synthesizer with 12 capacitive touch keys and an internal speaker. The enclosure will be made by lasercutting wood pieces into a box that will hold the keys, wiring, microcontroller and speaker.

## Inspiration

My main inspiration comes from Korg's [Volca](https://www.engadget.com/2016/06/11/korg-volca-fm-synthesizer/) sythesizers as well as their [monotron.](https://www.korg.com/us/products/dj/monotron/)

## Resources

- Arduino Capacitive Sensor Library https://playground.arduino.cc/Main/CapacitiveSensor?from=Main.CapSense
- Arduino I2S Library https://www.arduino.cc/en/Reference/I2S
- Arduino Theremin example https://create.arduino.cc/projecthub/Arduino_Genuino/i2s-theremin-cec47a

## Parts & Materials

- [Arduino MKR Zero](https://store.arduino.cc/usa/arduino-mkrzero) OR [Sparkfun SAMD21 Mini](https://www.sparkfun.com/products/13664)
- [I2S Audio Breakout](https://www.sparkfun.com/products/14809)
- [Small speaker](https://www.adafruit.com/product/1314)
- 9V Battery
- Copper tape
- scrap wood

## Extra Challenges

- Include a volume knob
- Include a touch controlled slide potentiometer that controls a synth parameter such as a filter cutoff value
- Include a switchable auxilary output to connect to a larger speaker

## Sketches

<img src="{{ site.baseurl }}/assets/image/synth/schematic.jpg" style="width:600px;" alt="schematic"/>
<img src="{{ site.baseurl }}/assets/image/synth/box-sketch.jpg" style="width:600px;" alt="schematic"/>
