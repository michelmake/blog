---
toc: true
layout: post
description: 3D-Printable Simplified Ventilator - COvid19 RESPirator OpeN SourcE
categories: [about, projects]
title: This is CORESPONSE
---
# CORESPONSE

## Objective

The development of a simplified ventilation device that is built with the help of a 3D printer and a few components so that it can be easily reproduced and assembled by volunteers all over the world. This device aims to save lives during the COVID19 crisis.

## Who we are?

We are an interdisciplinary team consisting of engineers and clinicians from RWTH Aachen University.

## The idea

The device is meant to provide a last resort for the possible situation when COVID19 infections outnumber the capacities of medical ventilation at healthcare facilities.

The device automatically squeezes widely available bag valve masks (BVMs, “Ambu-bags”).

The device is not developed as a medical device. It is not meant and not safe to be used without strict supervision. It is intended to be used when the situation is at a point where the only remaining alternative would be using volunteers to operate BVMs manually.


## The advantages

-Main components: 3D-printable parts, bag valve mask, motor
-All necessary files and building instructions will be made open source. 
-Anyone with access to a standard FDM 3D printer can build the device independently within one day. A large number of devices can be manufactured within a short period of time.

![]({{ site.baseurl }}/images/SchemeCORESPONSE_PNG.png "Scheme of the 3D-Printable Simplified Ventilator")


## State of the Project

Two different concepts are currently pursued in parallel. Both concepts should allow an adjustable breathing volume (tidal volume) and a variable respiratory rate. Additional oxygen can be administered via the BVM.

**Concept 1** uses a DC geared motor at a constant speed. This concept requires very simple electronics and no special control (“switch on and go”). The bag is operated using a 3D printed mechanism. The breathing volume is adapted by adjusting the mechanism.

![]({{ site.baseurl }}/images/KonzeptHebelV0.jpg "First prototype of Concept 1. Rapid development iterations are happening currently with improvements to the design.")


**Concept 2** uses a servo or stepper motor. This concept requires slightly more complex electronics for the control of the motor, but only a very few mechanical parts. The function can be adjusted using a smartphone.
![]({{ site.baseurl }}/images/concept_cable_winch_v0/assembly.jpg "First prototype of Concept 2. Rapid development iterations are happening currently with improvements to the design.")

The first prototypes have already been implemented and are currently evaluated and improved with a test lung (AEROtube®).
At the same time, a homepage is set up with replication instructions and all necessary files for printing the parts.

## COSTS AND MATERIAL

- Current status of building costs: below 75 Euro (Concept 1).
- Production: decentralized by volunteers owning an FDM 3D-Printer with a build plate of 20cmx20cm (250g Filament)
- Bag valve mask
- Electric motor and power supply
- Few mechanical small parts (e.g. screws)
