---
layout: post
title:  "Origami Circuit"
date:   2018-09-10 06:00:00 -0600
categories: [ Atlas-Object ]
---

<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/Origami-Circuit.gif" alt='origami ciruit gif' style="width:600px;"/>

This project is an implementation of Lab 1 from the [Object](https://objectfall2018.wordpress.com/lab-1/) class for [ATLAS](https://www.colorado.edu/atlas/) at CU Boulder. The purpose of this lab is to learn about simple circuits, custom made switches, and conductive materials.

## Overall Objectives
- Learn to build circuits on a breadboard
- Understand the difference between components in series and components in parallel Craft a custom switch
- Build a creative enclosure

## Part 1: LEDs in Series and Parallel

### Objective
Create two LED circuits with a switch. The first circuit should have LEDs in series and the second, LEDs in parallel.

### Materials
- Breadboard
- Assorted LEDs
- Jumper Wires
- 9V DC power supply
- Barrel Jack Connector
- 330Ω Resistors
- Momentary Switch

### LED Specifications

<table>
    <tr>
        <th>LED</th>
        <th>Voltage (V)</th>
        <th>Current (mA)</th>
    </tr>
    <tr>
        <td>Red</td>
        <td>1.8 - 2.2</td>
        <td>20</td>
    </tr>
    <tr>
        <td>Yellow</td>
        <td>2.0 - 2.4</td>
        <td>20</td>
    </tr>
    <tr>
        <td>Blue/Green</td>
        <td>5</td>
        <td>30</td>
    </tr>
</table>

### LEDs in Series
<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/LED-in-series-schematic.JPG" alt='LEDs-in-series-schematic' style="width:600px;"/>

<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/LEDs-in-series-off.JPG" alt='LEDs-in-series-off' style="width:600px;"/>

<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/LEDs-in-series-on.JPG" alt='LEDs-in-series-on' style="width:600px;"/>

### LEDs in Parallel
<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/LED-in-parallel-schematic.JPG" alt='LEDs-in-parallel-schematic' style="width:600px;"/>

<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/LEDs-in-parallel-off.JPG" alt='LEDs-in-parallel-off' style="width:600px;"/>

<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/LEDs-in-parallel-on.JPG" alt='LEDs-in-parallel-on' style="width:600px;"/>

## Parts 2 & 3: DIY Switch and Creative Enclosure
For my switch I made an origami fortune teller with LEDs. Different LEDs light up depending on the orientation of the origami. Here is a schematic of the circuit required for this project.
<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/origami-schematic.JPG" alt='origami schematic' style="width:600px;"/>


The circuit is very similar to the parallel LED ciruit created before. However, this circuit uses two switches - one for each LED.

### Materials
- Paper
- Blue and Green LED
- Conductive Copper Tape
- Regular Tape
- 3V Coin Battery

### Procuedure

- First I created a paper fortune teller. I won't describe how to do this here. Just think back to 3rd grade (or find a tutorial online).
- Next, I unfolded the paper fortune teller and drew the circuit directly on the paper. This way, I could create the circuit without worring about keeping the origami together. 
- Watch out for the creases in the paper. Copper tape can run over these creases but harder materials (bateries, LED leads) cannot or they will prevent the paper from folding correctly. The leads of the LEDs poke through the back of the paper so they can be connected to the battery.

    <img src="{{ site.baseurl }}/assets/image/Origami-Circuit/origami-final-1-edited.png" alt='origami ciruit drawing' style="width:600px;"/>

- This orange layout is a bit different from the final product but it demonstrates how I drew the components on the outside of the origami.
<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/origami-prototype-4.JPG" alt='origami ciruit drawing' style="width:600px;"/>
<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/origami-prototype-7.JPG" alt='origami ciruit drawing' style="width:600px;"/>
- After experimenting with a few circuit layouts, I put the components down on the paper.
<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/origami-final-2-edited.png" alt='origami ciruit components' style="width:600px;"/>
- The copper tape carries current from the positive terminal of the battery (top), through each of the contacts (also made of copper tape), throught the LED and finally back to the ground terminal of the battery (bottom). I used regular scotch tape both as insulation and to keep my components in place. 
- One complication I ran into was with keeping the battery in contact with the copper tape. I had a hard time getting the battery to stick to *anything.* The circuit worked great when lying flat on the table, but when I folded it up the battery would slip out of place. I tried scotch tape, hot glue and even tried soldering the tape to the battery. I ended up placing the copper tape in the appropriate places above and below the battery and tightly wraping the "sandwich" with regular tape. This took a few tries.
<img src="{{ site.baseurl }}/assets/image/Origami-Circuit/Origami-Circuit.gif" alt='origami ciruit gif' style="width:600px;"/>

### Thanks for reading!