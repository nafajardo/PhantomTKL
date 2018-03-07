# PhantomTKL
Repository for my Mechanical Keyboard Project.

## About the author
Nicholas Fajardo.
Mechanical keyboard enthusiast. My [email](nafajardo15@gmail.com).

## Required materials and resources
Resources:
* Time
* ~$150
* Soldering equipment
* A Computer
* Laser Cutter
* 3D Printer

Software:
* Soldiworks (or a suitable CAD program to view/edit files)
* [Keyboard layout generator](http://www.keyboard-layout-editor.com/#/)
* [CAD 2D sandwich case generator](http://builder.swillkb.com/)

Hardware used in my build:
* [Cherry MX Clears PCB Mounted - 100](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=594)
![Clear Switch](https://github.com/nafajardo/PhantomTKL/blob/master/Pics/Switch.jpg)
* [Blank Keycaps - 90+](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=1652)
![Blanks](https://github.com/nafajardo/PhantomTKL/blob/master/Pics/Caps.jpg)
* [Phantom TKL PCB - 1](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=536)
![PCB](https://github.com/nafajardo/PhantomTKL/blob/master/Pics/PCB.jpg)
* [Costar Stabilizers](http://www.wasdkeyboards.com/index.php/products/keyboard-parts.html)
![Sample costar stuff](https://github.com/nafajardo/PhantomTKL/blob/master/Pics/Costar.jpg)
* [Teensy 2.0 - 1](https://www.pjrc.com/store/teensy.html)
![Teensy](https://github.com/nafajardo/PhantomTKL/blob/master/Pics/Teensy.jpg)
* [Diodes - 90+](https://www.digikey.com/product-detail/en/on-semiconductor/1N4148/1N4148FS-ND/458603)
![Diodes 500 pack](https://github.com/nafajardo/PhantomTKL/blob/master/Pics/Diodes.jpg)
* [Teensy headers - 1 set](https://www.amazon.com/OdiySurveil-2-54mm-Straight-Single-Header/dp/B00UVPT5RI/ref=sr_1_sc_3?ie=UTF8&qid=1511016648&sr=8-3-spell&keywords=heaaders+for+circuit)
* [5V LEDs](https://www.amazon.com/Uxcell-a15050500ux0653-Bright-Light-Emitting/dp/B013U338OI/ref=sr_1_4?ie=UTF8&qid=1511016710&sr=8-4&keywords=5v+led&dpID=514QXT64ulL&preST=_SX342_QL70_&dpSrc=srch)
* Acrylic - 1 set of (609.6 mm x 457.2 mm)/(24" x 18") .1875" thick
* [Acrylic - 1 set of (609.6 mm x 304.8 mm)/(24" x 12") .06" thick](https://www.amazon.com/gp/product/B006QZ7J1G/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1)
* [USB Mini B Male to USB Mini B female - 1](https://www.digikey.com/product-detail/en/assmann-wsw-components/AK669M-1/AE10311-ND/1754621)
* [USB A Male to USB Mini B Male - 1](https://www.digikey.com/product-detail/en/assmann-wsw-components/AK672M-2-2/AE9929-ND/821683)
* [Parachord - 1 set](https://www.amazon.com/Paracord-Planet-Parachute-Strand-Popular/dp/B00GG0RLJQ/ref=sr_1_2?s=sporting-goods&ie=UTF8&qid=1511016892&sr=1-2&keywords=black+paracord)
* [M3x30MM Countersink bolts](https://www.amazon.com/gp/product/B01D9HIVNS/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)
* [M3 nuts](https://www.amazon.com/gp/product/B01IWUSDYY/ref=oh_aui_detailpage_o00_s01?ie=UTF8&psc=1)
* 3D printer PLA material (1.5mm grey)

Hardware that can be added/substituded:
* [Holtite](http://winkeyless.kr/product/holtite/)
* Any M3 bolts if you do not want countersinks
* Any CherryMX/Gateron switches can be substituted and/or replaced
* Any material choice I make can be substituted

### Notes on Required Materials
You can get 90 switches at the link above for $49.5 dollars, or 100 for $50. Spend the extra 50 cents.
I know the switches are PCB mounted on a plate build. I did this because I want the remaining PCB mounted switches for future projects and the BULK order price would have been cut if I got plate mounted. In order to convert PCB mounted to Plate mounted, you have to cut/pry off the two plastic tabs on the bottom.

## Phase 1 - Case structure
In terms of the case, all of my research has led me to the famous "Sandwich" case. This case basically has a bunch of layers that are laser cut to make a complete apparatus for your Switches and PCB.

### Sandwich Case details
The case consists of the following layers:
* Top Layer: The top layer is the border that covers the switch layer. This can be any height that is below the switch top height.
* Switch Layer: The switch layer has to be 1.5mm to 1.0mm in order for the cherry switches to properly clip onto the layer.
* Spacers: Currently, the research I have conducted shows that 15.0mm of spacers seems to be a comfortable balance between room for the wires and the PCB. Keep in mind these layers will be hosting the cable connection for the keyboard.
* Bottom Layer: This layer can be as thick as you want.

### Materials
* Acrylic: Popular, cost effective, could flex but thicker layers and proper engineering can reduce this.
* Wood: Good for prototyping, bit I do not reccomend it for a final product.
* Metal: if you have the money, then sure this is a great material!

### How to make the case
I generated my specific case by using [Keyboard layout generator](http://www.keyboard-layout-editor.com/#/) and [CAD 2D sandwich case generator](http://builder.swillkb.com/). You first go to Keyboard Layout editor, and generate your configuration. Once that is done, copy and paste the raw data into the CAD 2D sandwich case generator and set your settings. In my case, I put a bit of a border, anad set kerf to .05 since thats the specification of the laser cutter I will be using.

![Settings for CAD stuff](https://github.com/nafajardo/PhantomTKL/blob/master/Pics/CAD%20Settings.png)

Once you have this done, make a DWG file ready with all the parts laid out to cut. For me, I needed to make the parts on a 24x18 sized sheet for all layers except the switch layer. And then I made the switch layer on a 12x24 piece of 1.5mm thick acrylic to match the clip mechanism specs on a Cherry MX switch. You can find more details on this [here](http://cherryamericas.com/product/mx-series-2/).

After cutting your pieces, you should have an assembly ready. The design I made calls for 8 M3 screws to fasten the case. I bought [Countersink Screws](https://www.amazon.com/gp/product/B01D9HIVNS/ref=od_aui_detailpages00?ie=UTF8&psc=1) and [nuts](https://www.amazon.com/gp/product/B01IWUSDYY/ref=od_aui_detailpages00?ie=UTF8&psc=1) because of my case dimensions.

I am making 5 layers of .1875" thick acrylic, and one layer of .06" acrylic. This leads to a total of 25.34 mm of thickness. The nuts are 2.25 mm thick, so we have a leftover of 2.4 mm of screw at the bottom. So far, I will probably install some rubber feet here similar to [this](http://www.mocap.com/threaded-plastic-caps-for-metric-threads.html) if I can find it in 3mm.

In terms of angle, I am going to be installing some mechanisms after the keyboard is done that will allow me to dynamically change the position of the keyboard. This will not be part of the main phases, so dont worry about it right now.

## Phase 2 - Soldering your ass off
You are gonna have to solder SO MUCH, so get a place with good ventilation, alot of solder, a good iron, and a voltmeter to fix those happy mistakes.

Here is the order we are going in:
* Diodes
* Teensy
* Switches
* LEDs

So for the diodes, we have to make sure that they are facing the right way. Each spot where the diodes are going to be soldered is going to have a square and a circle. The rule of thumb is to make sure that the black strip (if you got the diodes form where I got them) is closer to the square part of the terminals.

The Teensy must be placed with male to male headers soldered onto the actual logic board.

Now for the switches. We are going to put four or five switches in each corner of the plate layer, and then put that onto the PCB. This will let us make sure that the switches are aligned, and makes the process of combining the switch layer and the PCB layer easier.

Once this is done, the soldering is finished!

## Phase 3 - Code Upload and Testing
First, depending on your system, you must download the correct [drivers/compiler](https://www.pjrc.com/teensy/loader.html) for the Teensy board. Once you do this,

use the Teensy to test by putting in your [custom key mapping](https://www.pjrc.com/teensy/usb_keyboard.html) and hoping that each key works. You can go to [this](http://www.keyboardtester.com/) to test.


## Phase 4 - Miscellaneous Topics
Depending on the application, stabilizers might be a good or bad idea. In my specific applicaiton, costars were the best choice, but cherry stabilizers might be better for tighter fits.

After this, make any visual changes! I put some divots for the holes that the screws go in, since the screws that I am using have a countersink.

The acrylic that I used for the switch layer warped during the laser cutting process. This can be avoided by using a thicker material, or using metal. Be warned that thicker material will not allow cherry switches to latch on, which might be a problem for your' certain application.

## Conclusion
This project was not only fun for me, but it was a great experience in general for laser cutting, C programming, micro processor interaction, CAD drawing, and general ergonomic design. My keyboard came out very nice, and to this day it still holds up!

I wish you luck on your journey through mechanical keyboards, and please email me with any questions!

Nick
