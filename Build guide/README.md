This guide shows how to assemble our PRKL30 Kit.
================================================

### Tools needed:

\-Flush cutters

\-Soldering iron & solder (solder sucker just in case)

\-**OPTIONAL:** Diode Bender (like this [3D-printable one](https://www.thingiverse.com/thing:2651766), send us a message and we can print one for you), Kapton tape for insulating the Pro Micro.

Step 1: Diodes
--------------

Place the PCB onto your workspace so that the PRKL30 Logo is facing up

![](https://pohjola.works/wp-content/uploads/2020/08/PRKL30_guide_0-scaled-e1598365152634-800x246.jpg)

Start laying diodes so that the black stripe of the diode matches with the square pad on the diode hole, you can keep something under the PCB so that the diodes stay in place OR bend the diode legs so they stay in place without moving. HINT: A diode bender makes things easier and the bends more uniform.

![](https://pohjola.works/wp-content/uploads/2020/08/IMG_6177-359x400.jpg)

Install all the diodes on to their footprints, verify orientation (black stripe to square pad) and solder them in place from the same side where the diodes are.

![](https://pohjola.works/wp-content/uploads/2020/08/PRKL30_guide_1-1-800x367.jpg)

Clip the diode legs with flush cutters from the top side after this.

Step 2: Reset button
--------------------

It's a good practice to tin the SMD pads for the reset button beforehand to make the solder job easier:![](https://cdn.discordapp.com/attachments/720743794386927678/747463548413804564/IMG_20200824_173108.jpg)

And then solder the SMD reset button into the SW\_RST1 footprint as shown in the picture.

![](https://pohjola.works/wp-content/uploads/2020/08/PRKL30_guide_2-1-183x400.jpg)

Step 3: Pro Micro Headers
-------------------------

**OPTIONAL: You can also socket your pro micro, following this awesome guide [https://www.40percent.club/p/socketing-pro-micro.html](https://www.40percent.club/p/socketing-pro-micro.html) this is totally optional, but totally recommended. The main principle is pretty much the same, but allows detaching the pro micro without desoldering !**

Solder the included Pro Micro headers like shown in the picture, **shorter pins through the pcb pin holes !** This is to make it easier to fit the switches, so there isn't any extra solder laying around on the top side.

![](https://pohjola.works/wp-content/uploads/2020/08/IMG_2383-513x400.jpg)

Step 4: Switches
----------------

Solder in your switches next, and place them on to the side where there aren't any Logos or extra graphics.

Step 5: Pro Micro
-----------------

Drop the pro micro into the longer headers with components **facing the main PCB**, and solder into place.

![](https://pohjola.works/wp-content/uploads/2020/08/IMG_0929-547x400.jpg)

### \+ OPTIONAL: WS2812 RGB Underglow

The PCB has pinout near the pro micro at the edge of the board for WS2812 RGB Strip, hook it up + for pwr, gnd for gnd, data for data.

Step 6: Configuring & Flashing QMK Firmware
-------------------------------------------

Open [https://config.qmk.fm/#/handwired/prkl30/promicro/LAYOUT\_all](https://config.qmk.fm/#/handwired/prkl30/promicro/LAYOUT_all) in your desktop browser, tweak the layout to your liking, press compile and download the resulting .hex file of the firmware.

Install [QMK Toolbox](https://qmk.fm/toolbox/)

Follow QMK Guidelines in flashing.

You should be able to reset the keyboard by pressing the reset button on the PCB.

### That's it ! Enjoy your awesome new keyboard ♥️