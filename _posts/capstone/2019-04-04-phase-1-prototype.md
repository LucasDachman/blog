---
layout: post
title:  "Prototype: Phase 1"
date:   2019-04-04 4:38:53 -0600
categories: [ Capstone ]
---

# Melody Generator

This prototype focuses on using randomness and probability to generate endless and unique melodies.

## Role

Functionality
- Musical sequences are created through a "piano roll" style interface
- Probabilities can be assigned to each note trigger
- Sequences loop infinitely
- User can change the length of the loop
- User can set note duration
- User can choose between monophonic and polyphonic
- User can change the tempo
- 127 keys
- Triggered notes are highlighted to provide feedback

## Look & Feel 

UI Mockups showing possible theme and layout

<img src="{{ site.baseurl }}/assets/image/capstone-1/buttons.png" alt="screenshot" style="width:550px;"/>
<img src="{{ site.baseurl }}/assets/image/capstone-1/Piano roll.png" alt="screenshot" style="width:550px;"/>

## Implementation

A web app that implements a simple piano roll with note probabilities.

[**Link to demo**](https://lucasdachman.github.io/melody-generator/)

[**Link to code**](https://github.com/LucasDachman/melody-generator)

### Recordings

<iframe src="https://player.vimeo.com/video/328570614" width="550" height="421" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
<iframe src="https://player.vimeo.com/video/328570631" width="550" height="487" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

### How the code works

When a user activates cells in the UI, chords are formed. Say a user makes a C Major chord (C,E, G). Then, the user sets the note's probabilities: C: 40%, E: 40%, G: 20%. The program will make an array where the first 40 elements are equal to "C", the next 40 elements are equal to "E" and the last 20 are equal to "G". Next, the program generates a random number between 0 and 100. This number is used as an index to pick a note from the array. The code looks something like this:


<img src="{{ site.baseurl }}/assets/image/capstone-1/melody-gen-code.png" alt="screenshot" style="width:800px;"/>