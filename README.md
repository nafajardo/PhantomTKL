# PhantomTKL
Repository for my Mechanical Keyboard project. 

## About the author
Nicholas Fajardo.
Mechanical keyboard enthusiast extraordinaire. My [email](nafajardo15@gmail.com).

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

Hardware:
* [Cherry MX Clears PCB Mounted - 100](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=594) 
* [Blank Keycaps - 90+](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=1652)
* [Phantom TKL PCB - 1](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=536)
* [Costar Stabilizers + 1 set](https://www.winnja.com/keyboard-accessories/costar-stabilizers-for-cherry-mx-switches.html)
* [Teensy 2.0 - 1](https://www.pjrc.com/store/teensy.html)
* [Diodes - 90+](https://www.digikey.com/product-detail/en/on-semiconductor/1N4148/1N4148FS-ND/458603)
* [Teensy headers - 1 set](https://www.amazon.com/OdiySurveil-2-54mm-Straight-Single-Header/dp/B00UVPT5RI/ref=sr_1_sc_3?ie=UTF8&qid=1511016648&sr=8-3-spell&keywords=heaaders+for+circuit)
* [5V LEDs](https://www.amazon.com/Uxcell-a15050500ux0653-Bright-Light-Emitting/dp/B013U338OI/ref=sr_1_4?ie=UTF8&qid=1511016710&sr=8-4&keywords=5v+led&dpID=514QXT64ulL&preST=_SX342_QL70_&dpSrc=srch)
* [Acrylic - 1 set of (609.6 mm x 457.2 mm)/(24" x 18")](http://freckleface.com/shopsite_sc/store/html/product902.html)
* [USB Mini B Male to USB Mini B female - 1](https://www.digikey.com/product-detail/en/assmann-wsw-components/AK669M-1/AE10311-ND/1754621)
* [USB A Male to USB Mini B Male - 1](https://www.digikey.com/product-detail/en/assmann-wsw-components/AK672M-2-2/AE9929-ND/821683)
* [Parachord - 1 set](https://www.amazon.com/Paracord-Planet-Parachute-Strand-Popular/dp/B00GG0RLJQ/ref=sr_1_2?s=sporting-goods&ie=UTF8&qid=1511016892&sr=1-2&keywords=black+paracord)

### Notes on Required Materials
You can get 90 switches at the link above for $49.5 dollars, or 100 for $50. Spend the extra 50 cents.
Some materials above (like the parachord, acrylic, and switches) are up to the user to decide based on personal preference.
I know the switches are PCB monuted on a plate build. I did this becaause I want the remaining PCB mounted switches for future projects and the BULK order price would have been cut if I got plate mounted.

## Phase 1 - Case structure
In terms of the case, all of my research has led me to the famous "Sandwich" case. This case basically has a bunch of layers that are laser cut to make a complete aparatus for your Switches and/or PCB.

### Sandwich Case details
The case consists of the following layers:
* Top Layer: The top layer is the border that covers the switch layer. This can be any height that is below the keycap height.
* Switch Layer: The switch layer has to be 1.5mm to 1.0mm in order for the cherry switches to properly clip onto the layer.
* Spacers: Currently, the research I have conducted shows that 15.0mm of spacers seems to be a comfortable balance for room for wires and the PCB. Keep in mind these layers will be hosting the cable connection for the keyboard.
* Bottom Layer: This layer can be as thick as you want.

### Materials
* Acrylic: Popular, cost effective, could flex but thicker layers and proper engineering can reduce this.
* Wood: Good for prototyping, bit I do not reccomend it for a final product.
* Metal: if you have the money, then sure this is a great material!

### How to make the case
I generated my specific case by using [Keyboard layout generator](http://www.keyboard-layout-editor.com/#/) and [CAD 2D sandwich case generator](http://builder.swillkb.com/). You first go to Keyboard Layout editor, and generate your configuration. Once that is done, copy and paste the raw data into the CAD 2D sandwich case generator and set your settings. In my case, I put a bit of a border, anad set kerf to .05 since thats the specification of the laser cutter I will be using.

Once you have this done, make a DWG file ready with all the parts laid out to cut. For me, I needed to make the parts on aa 24x18 sized sheet for all laayers except the switch layer. And then I made the switch laayer on a 12x24 piece of 1.5mm thick acrylic to match the clip mechanism specs on a Cherry MX switch. You can find more details on this [here](http://cherryamericas.com/product/mx-series-2/).

After cutting your pieces, you should have an assembly ready. The design I maade calls for 8 M3 screws to fasten the case. I bought [Countersink Screws](https://www.amazon.com/gp/product/B01D9HIVNS/ref=od_aui_detailpages00?ie=UTF8&psc=1) and [nuts](https://www.amazon.com/gp/product/B01IWUSDYY/ref=od_aui_detailpages00?ie=UTF8&psc=1) because the thickness of my case, in total, is 25 (24.85)mm.

In terms of angle, I am going to be installing some mechanisms after the keyboard is done that will allow me to dynamically change the position of the keyboard. This will not be part of the main phases.
