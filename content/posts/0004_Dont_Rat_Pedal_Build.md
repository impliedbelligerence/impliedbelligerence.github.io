---
title: "Don't Rat Pedal Build"
date: 2023-06-08T00:08:39-08:00
draft: true
---

# DONT RAT PEDAL
DIY RAT CLONE BUILD

<br>
<br>

### THE PLAN
---

For my first pedal build I went with a [Helios from Aion FX](https://aionfx.com/project/helios-vintage-distortion/ "Helios from Aion FX"), which is a Rat clone. A Rat was one of the first pedals I used almost 20 years ago but I've never owned one, so it seemed fitting. Truthfully, I really wanted to do Aion FXs Klon clone, but the PCBs were sold out when I was browsing. That will be coming soon though.

I did the majority of this build through out a single day while on vacation and didn't document anything while working it all out. There was a lot more to manage than I anticipated so I focused on the task at hand. I learned a lot during the process and am documentating it now that I have had some time to reflect. I didn't get as many pictures of the process as I would have liked, so this will mostly be a text post.

I sourced the compoents myself and got the vast majority from Mouser (and stocked up on a few caps and resistors while I was at it). I had to grab some caps and battery clips from Digi-key because Mouser was out of stock and I grabbed the potetiometers and switches from [Love My Switches](https://lovemyswitches.com/ "Because I love Love My Switches"). I love buying pots from LMS, the prices are great and they ship quick.

This was my first pedal build, so I took time making sure I had all the right components and getting them sorted for an easy assembley. I spent a few days just thinking it all over and making sure I understood as much as I could before I jumped in. Once I built enough confidence I finally started building.

<br>
<br>

### THE BUILD
___

I like to start with the shorter components first, like the resistors and dioides. After that I did the ceramic caps and dip socket for the IC. I should have done the 3mm LEDS next, but I actually forgot about them until later. I moved onto the film caps, JFET and electrolytic caps. I did the LEDs somewhere in between all of that when I realized I had forgot. 

I drilled the box out next to make sure I understood exactly where to mount the pots and jacks and wire everything up dry before I committed to soldering anything else to my PCBs. I have a drill press here, so this was actually pretty easy. I taped a paper guide to the face of the work and used a center hole punch to mark where I wanted my bits to start. I put the work into into a drill press vice which I didn't even both clamping the vice down to be honest. I just moved here and turns out I don't have any c-clamps who can handle the job anymore. With the low RPM of the press and thinest of the work, I still had about 97% control of where the holes went. Good enough for our purposes here. 

After dry fitting the pieces I could, I spent some time just making sure I understood how it was all even supposed to lay out in the box. Once I had that figured out, I trimmed up some hookup wire to connect the switch PCB to the main PCB and jacks but didn't solder it up yet. I went ahead and got the pots and clip switch soldered to the main board and did a few more dry fits. This is where things started getting really exciting, because it looks like a real pedal, albeit naked. 

Someone on [r\diypedals](https://www.reddit.com/r/diypedals/) told me to make sure to wire the switch PCB to the main PCB before soldering the switch on and this was great advice. I actually mounted the switch into the enclosure and used it to mount up the switch pcb and plan everything out. Not having a gigantic footswitch attached to the PCB I was solderings leads onto was lit. I soldered the leads to everything, jammed it all into the box and then soldered the footswitch in place. Everything is ready to fire up and test for the first time...

<br>
<br>

### THE TEST
----

The first hook up failed, of course, but nothing exploded so we are already making progress. To be exact, the pedal powers up with a beautiful led and passes clean audio without issue. But as soon as the circuit engages the signal stops dead. A little troubling, but we don't learn anything when everything works out all the time. Time to put our debugging skills to use, and I coincidently built the perfect tool for this job already, the audio probe!

Using the audio probe, I traced the issue to the second component in the signal path, not a good start... At anty rate, the second component is a 22nF film capacitor and when it visits my meter for a checkup we discover there is no capacitence at all, the part is fried. Doing some research it turns out film caps are pretty easy to burn out (opps!) and it sounds like I will need to turn the iron down a bit and give the caps a little more breathing space from the PCB. I normally use a tempature of 700 degrees, which melts the 63/37.015 solder I use almost instantly. They say to not leave the iron on more than 3 seconds at about 650 degrees, so I am going to rip this cap out and try that. 

I decided to test the rest of the film caps on the board and discovered two more fried caps. Luckily I bought enough extras, but I only have one of each so I will need to be more more careful this time. 

* C1 22n Film capacitor, 7.2 x 2.5mm
* C2 1n Film capacitor, 7.2 x 2.5mm
* C8 3n3 Film capacitor, 7.2 x 2.5mm

<br>
<br>

### BACK TO THE BENCH
---

C8 is right next to C9 on the board, so I will have to be careful of not overheating the board while desoldering C8. I bought some soldering wick and this was my first time using it. It did not go as smooth as I would have liked. In about 2 hours of work, I was able to get two caps completely out and prepare the pads for new components. But the third pad gave me a lot more trouble, the cap broke off from the leads and while attempting to clear the pcb of solder ond one of the pads lifted off the board. It looks like I can repair it, but that's a hell of a setback.



