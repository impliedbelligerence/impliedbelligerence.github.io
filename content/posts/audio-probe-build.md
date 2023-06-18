---
title: "Audio Probe Build"
date: "2023-06-15"
description: "Build guide for audio circuit probe."
categories:
  - "Builds"
tags:
  - "Builds"
  - "Audio-Circuit"
  - "Analog-Circuit"
menu: main # Optional, add page to a menu. Options: main, side, footer

# Theme-Defined params
thumbnail: # Thumbnail image
lead: "How to make a simple probe for audio circuits." # Lead text
comments: true # Enable Disqus comments for specific page
authorbox: true # Enable authorbox for specific page
pager: true # Enable pager navigation (prev/next) for specific page
toc: false # Enable Table of Contents for specific page
mathjax: false # Enable MathJax for specific page
sidebar: "right" # Enable sidebar (on the right side) per page
widgets: # Enable sidebar widgets in given order per page
  - "search"
  - "recent"
  - "taglist"
---

# AUDIO PROBE BUILD

<br>

![audio_probe](./staged_images/0003_Audio_Probe_Build/audio_probe.JPG)

<br>

Based on the directions from [diy-fever.com](http://diy-fever.com/misc/audio-probe/), this is a simple probe to test audio circuits.

The idea behind its operation is that aftering grounding one wire, the other can be used to safely probe around an audio circuit. Starting at the input components we trace the signal playing through the circuit until the point of failure. When you discover where the audio stops passing, you've likely found your issue. 

This build is as easy as it gets.

<br>

| You will need:   |
|---------|
|1/4" TS connector, male or female  |
|two pieces of wire or a bit of old unbalanced audio cable |
|alligator clip |
|probe lead (not required but nice to have) |
|1uF 63v cermanic capacitor (I actually used 50v on mine...)|

\
You can use a female connector if you want to be able to plug a guitar cable into the probe for extra length as needed. If you use a male connector, you would just be plugging the probe directly into your amp. This could make probing a little more difficult than needed, so I reccomend the female connector here.

Solder one wire to the sleeve of the jack for grounding, the other end of this wire gets the alligator clip so it can easily be clipped to the ground of a circuit and remain there safely. 

The other wire will be soldered to one end of your 1uF 63v capacitor, with the other end of the cap soldered to the tip of the jack. You should get the probe lead on the other end of the wire if you are using one. You can probe with bare wire if it suits your purposes.

<br>

![audio_probe_cap](./staged_images/0003_Audio_Probe_Build/audio_probe_cap.JPG)




