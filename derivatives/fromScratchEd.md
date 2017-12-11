---
layout: derivative
category: derivative
title: fromScratchEd's Primo play set
folder: fromScratchEd
---

<div id="notes">
This document lists all necessary information needed to build your own prototype like <a href="http://fromscratched.nl/?lang=en">fromScratchEd</a> did.<br>
Please use this document side-by-side the original documentation of Primo for the building instructions.<br>
<br>
Please <a href="http://fromscratched.nl/index.php/neem-contact-op/?lang=en">contact me</a> when you need more information or have questions.<br>
<br>
Sjoerd Dirk Meijer, the Netherlands<br>
Blog: <a href="http://fromscratched.nl/?lang=en">http://fromScratchEd.nl</a><br>
Twitter: <a href="https://twitter.com/fromScratchEd">@fromScratchEd</a> (tweets in Dutch and English)<br>
<br>
License: CC BY-NC-SA 3.0
</div>
<br>

### Bill of materials
([Tayda publishes discount codes on their Facebook page regularly!][5])

#### Cubetto

* 1 x Shrimp ([http://Shrimping.it)][6]: replacement of Arduino UNO (or Leonardo)
* 1 x Stripboard ([Tayda][7]): replacement of Arduino Proto Wireless Shield
* 1 x Active(!) XBBO - break out board for XBee shaped modules ([Ciseco][10]): replacement of Arduino Proto Wireless Shield
* 1 x XRF wireless RF radio UART RS232 serial data module XBee shape ([Ciseco][9]): replacement of XBee
* 1 x L293D ([Tayda][8]): replacement of SN754410 Motor Driver
* 2 x SolarBotics Wheels ([Technobots][11])
* 2 x SolarBotics Gear Motors GM3 ([Technobots][12])
* 2 x Ball Casters 3/8 inch ([Technobots][13]): replacement of Ball Casters 1/2 inch
* 2 x CNY70 ([AliExpress][14])
* 2 x 10KΩ Resistors
* 2 x 220Ω Resistors
* 1 x Battery Holder ([Tayda][15])
* 4 x Rechargeable Batteries (local store)
* 1 x Voltage regulator kit ([Ciseco][16]) (not shown in schematics below)
* 1 x Switch (local store) (to cut the power)

#### Interface Board

* 2 x Shrimp ([http://Shrimping.it)][17]: replacement of Arduino Mega 2560
* 2 x Stripboard ([Tayda][18]): replacement of Arduino Proto Wireless Shield
* 1 x Active(!) XBBO - break out board for XBee shaped modules ([Ciseco][20]): replacement of Arduino Proto Wireless Shield
* 1 x XRF wireless RF radio UART RS232 serial data module XBee shape ([Ciseco][19]): replacement of XBee
* 16 x 5mm Red LED ([Tayda][21])
* 16 x 220Ω Resistors ([Tayda][22])
* 16 x 10KΩ Resistors ([Tayda][23])
* 1 x Push Button ([Tayda][24])
* 16 x Magnets ø 4 h 4 ([Magnetenspecialist][25]): replacement of Magnets ø 4 h 3
* 1 x Battery Holder ([Tayda][15])
* 4 x Rechargeable Batteries (local store)
* 1 x Voltage regulator kit ([Ciseco][26]) (not shown in schematics below)
* 2 x CD4052 ([Tayda][52]) (to add extra analog inputs)
* 1 x Switch (local store) (to cut the power)

#### Instruction Blocks

* 4 x 4.7KΩ Resistor ([Tayda][27])
* 4 x 100KΩ Resistor ([Tayda][28])
* 4 x 220Ω Resistor ([Tayda][29])
* 4 x 10KΩ Resistor ([Tayda][30])
* 16 x Magnets ø 4 h 4 ([Magnetenspecialist][31]): replacement of Magnets ø 4 h 3

#### Wood

* 6 x 60cm x 30cm x 4mm plywood (local store)
* 1 x 50cm x 30cm x 1mm plywood (a.k.a. flexible plywood, bendy plywood, flexiply of airplane plywood) ([Yvonne's Hobby-corner][32])

### The adventures (links to my blog)
* [Day 1][33]: Getting the source files
* [Day 2][34]: Ordering materials
* [Day 3][35]: Editing lasercutter files
* [Day 4][36]: Buying the 4mm wood
* [Day 5][37]: Buying the 1mm wood
* [Day 6][38]: Sawing
* [Day 7][39]: Reordering materials
* [Day 8][40]: Lasercutting (with tips!) @[FabKlas][41]
* [Day 9][42]: Wheels arrived
* [Day 10][43]: CNY70's arrived
* [Day 11][44]: GM3 alternative (don't use them!)
* [Day 12][45]: Making the interface board and blocks
* [Photos][46]: Photos of the building process
* [Schematics and software][47]
* [Finished][48]: Why I made Primo, what I'm going to do with Primo and who I am (and why I think programming with young children is important)

### Source files
[Arduino files][49]

[Lasercutter files][50]

### Schematics
For the Interface Board I used two Shrimps connected with I2C (connect A4 at A4, A5 at A5, 5V at 5V and GND at GND).

The primary Shrimp is connected to the block holes of the interface board, the secondary Shrimp is connected to the LED's.

![enter image description here][51]


  [1]: http://fromscratched.nl/index.php/category/primo/?lang=en
  [2]: http://fromscratched.nl/index.php/neem-contact-op/?lang=en
  [3]: http://fromScratchEd.nl/?lang=en
  [4]: https://twitter.com/fromScratchEd
  [5]: https://www.facebook.com/TaydaElectronics
  [6]: http://shrimping.it
  [7]: http://www.taydaelectronics.com/small-stripboard-94x53mm-copper.html
  [8]: http://www.taydaelectronics.com/catalogsearch/result/?q=l293d
  [9]: http://shop.ciseco.co.uk/xrf-wireless-rf-radio-uart-rs232-serial-data-module-xbee-shape-arduino-pic-etc/
  [10]: http://shop.ciseco.co.uk/xbbo-break-out-board-for-xbee-shaped-modules/
  [11]: http://www.technobotsonline.com/solarbotics-gmpw-plastic-red-wheel-33812.html
  [12]: http://www.technobotsonline.com/solarbotics-gm3-90-degree.html
  [13]: http://www.technobotsonline.com/pololu-ball-caster-3-8-inch-plastic-ball.html
  [14]: http://www.aliexpress.com/item/Free-Shipping-10pcs-CNY70-DIP-4/1644744700.html
  [15]: http://www.taydaelectronics.com/aa-battery-holder-4.html
  [16]: http://shop.ciseco.co.uk/voltage-regulator-kit-for-xino-basic-for-atmel/
  [17]: http://shrimping.it
  [18]: http://www.taydaelectronics.com/small-stripboard-94x53mm-copper.html
  [19]: http://shop.ciseco.co.uk/xrf-wireless-rf-radio-uart-rs232-serial-data-module-xbee-shape-arduino-pic-etc/
  [20]: http://shop.ciseco.co.uk/xbbo-break-out-board-for-xbee-shaped-modules/
  [21]: http://www.taydaelectronics.com/
  [22]: http://www.taydaelectronics.com/
  [23]: http://www.taydaelectronics.com/
  [24]: http://www.taydaelectronics.com/
  [25]: http://www.magnetenspecialist.nl/?catalogproduct/1351262/SCHIJFMAGNEET%204x4mm.aspx
  [26]: http://shop.ciseco.co.uk/voltage-regulator-kit-for-xino-basic-for-atmel/
  [27]: http://www.taydaelectronics.com/
  [28]: http://www.taydaelectronics.com/
  [29]: http://www.taydaelectronics.com/
  [30]: http://www.taydaelectronics.com/
  [31]: http://www.magnetenspecialist.nl/?catalogproduct/1351262/SCHIJFMAGNEET%204x4mm.aspx
  [32]: http://www.hobby-corner.nl/vliegtuigtriplex-triplex-berken-hout/vliegtuigtriplex-triplex-berken-hout-100x25cm
  [33]: http://fromscratched.nl/index.php/28-februari-2014/?lang=en
  [34]: http://fromscratched.nl/index.php/primo-1-maart-2014/?lang=en
  [35]: http://fromscratched.nl/index.php/primo-dag-3-2-maart-2014/?lang=en
  [36]: http://fromscratched.nl/index.php/primo-dag-4-3-maart-2014/?lang=en
  [37]: http://fromscratched.nl/index.php/primo-dag-5-4-maart-2014/?lang=en
  [38]: http://fromscratched.nl/index.php/primo-dag-6-5-maart-2014/?lang=en
  [39]: http://fromscratched.nl/index.php/primo-dag-7-6-maart-2014/?lang=en
  [40]: http://fromscratched.nl/index.php/primo-dag-8-7-maart-2014/?lang=en
  [41]: http://fabklas.nl
  [42]: http://fromscratched.nl/index.php/primo-dag-9-11-maart-2014/?lang=en
  [43]: http://fromscratched.nl/index.php/primo-dag-10-12-maart-2014/?lang=en
  [44]: http://fromscratched.nl/index.php/primo-dag-11-13-maart-2014/?lang=en
  [45]: http://fromscratched.nl/index.php/primo-dag-12-18-maart-2014/?lang=en
  [46]: http://fromscratched.nl/index.php/primo-foto-maartapril-2014/?lang=en
  [47]: http://fromscratched.nl/index.php/primo-schemas-en-software/?lang=en
  [48]: http://fromscratched.nl/index.php/primo-klaar/?lang=en
  [49]: https://github.com/sdmeijer/arduino-sketches/blob/master/fromScratchEd/fromScratchEd.zip?raw=true
  [50]: https://github.com/sdmeijer/arduino-sketches/blob/master/fromScratchEd/fromScratchEd_laser.zip?raw=true
  [51]: http://fromscratched.nl/wp-content/uploads/2014/04/Scan-140415-0001_small.jpg
  [52]: http://www.taydaelectronics.com/cd4052-4052-cmos-multiplex-demultiplexer-ic.html
