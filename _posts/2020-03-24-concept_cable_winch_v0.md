---
title: "Concept Cable Winch v0"
summary: "Description, build instructions and lessons learned from the cable winch concept."
toc: true
comments: true
image: images/concept_cable_winch_v0/assembly.jpg
hide: false
search_exclude: true
categories: [instruction, concept]
---

# Concept Cable Winch
## Description

<iframe width="560" height="315" src="https://www.youtube.com/embed/jHJIzP7SPyo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The concept aims to realize a compression of a bag-valve-mask with as little moving parts as possible.
This reduces the number of parts which have to be printed and weak points.
A simple pulley is used to pull two printed parts together and compress the bag.

However, this concept requires a motor which can be position controlled (e.g. a servo or a stepper motor).
Consequently, a micro controller is required to pass the inputs to the motor.
On the plus side, the software allows a higher customizability of the air flow, volume and frequency.

## Required Components
![]({{ site.baseurl }}/images/concept_cable_winch_v0/components.jpg "Required components" =560x)

3D printed:
- enclosure
- pulley
- pusher

Electrics:
- Dynamixel servo motor (XL430-W250-T or better, we had an XM430-W350-T lying around)
- OpenCM9.04 board
- 12V DC power supply

Norm pieces:
- 4x: M2.5x16 cylinder head screws
- 4x: M2.5 washer
- 4x: M2x9 countersunk screws

Others:
- Elastic
- Lace

Tools:
- allen wrench size 2
- small slot screwdriver

## Build Instructions

First, mount the motor on the enclosure using the M2.5x16 screws and washers.
![]({{ site.baseurl }}/images/concept_cable_winch_v0/step_1.jpg "Step 1" =560x)

Next, pass the lace through the hole in the pulley and knot it tightly.
Pass the lace through the rectangular hole in the enclosing and mount the pulley on the motor's flange using the M2 countersunk screws.
![]({{ site.baseurl }}/images/concept_cable_winch_v0/step_2.jpg "Step 2" =560x)

Pass the elastics through the smaller holes of the enclosure and through the outer holes of the pusher.
The lace has to be passed through the center holes of the pusher.
If you would like a secure fit, pass the elastic and lace through the handle of the bag.
You could also place both over the handle for easier unmounting of the whole device.
![]({{ site.baseurl }}/images/concept_cable_winch_v0/step_3.jpg "Step 3" =560x)

Finally, knot the elastic and the lace to the other side of the enclosure.
![]({{ site.baseurl }}/images/concept_cable_winch_v0/assembly.jpg "Assembly" =560x)

## Programming the board
The code and instructions to flash the OpenCM9.04 board are available in [this github repository](https://github.com/CORESPONSE/dynamixel_software).

# Lessons learned
The bag can be compressed by the small servo motor but the bags are quite sticky.
Thus, the lace cannot move freely around the bag and the enclosure moves instead of the pusher.
Also, the motion is more like folding the bag and not pushing it in the middle.
On the plus side, the bag can be held at the handle and performs almost no motion.
This is beneficial for the patients well being.

The next iterations will continue to emphasize using the handle to place the bag over the patient.
An improvement should be expected by applying the force evenly in the middle of both sides to suppress the motion of the enclosure.