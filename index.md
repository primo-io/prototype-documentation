---
layout: default
title: Home
---

##0. What is this document

In this document we gathered and organized all the information necessary to build a Primo Play Set Prototype.
You can find more info about the project on the [primo.io](http://primo.io) website.

#IMPORTANT
The documentation and instructions inclosed in this document will allow you to produce a Primo prototype as show in this video, which is different to the final product. However, we will also keep releasing the necessary documentation for updates and new versions of the Primo Play Set, including files for the final product, as and when we have them tried and tested.


#MORE IMPORTANT
The license under which we release the Primo Play Set gives you the freedom to build your own Prototype. However, under any circumstances, you are not entitled to sell it as Primo Play Set. If you wish to develop a derivative of our product, you have to quote the original project (as we do with all our sources), and use the same license we do: [CC by-nc-sa 4.0 International](http://creativecommons.org/licenses/by-nc-sa/4.0/). 
This is not just to protect intellectual property, but also to keep track of all the ideas spawned from the original project and create a community. We are spending a lot of time and resources to keep this documentation free and accessible, we encourage you to "give back" to our community by posting your derivatives, results, suggestions, insults and praises on our forum. We will listen to feedback and blog cool stuff directly on our website.

##1. What is Primo

<primo picture>

Primo is a tangible interface designed to introduce programming logic to little children (3 to 7), without the need for literacy. The goal of the game is to drive a little robot called Cubetto back to his house. To accomplish the goal, children have to program the little robot using a limited set of instructions: forward, left, right and function. While the first three are rather intuitive, the last one calls a sub-routine, an extra line of instructions packed in a single command.

<primo video>

##2. Research

Teaching programming to children is a widely debated topic. We are aware of a moderate number of solutions that try to accomplish this for children above the ages of 8. However, there aren't many of these solutions suitable for younger children, and there aren't any that work without a screen or without the need for literacy. We see an increasing number of Apps for tablets and computers, also in combination with physical robots, but none of them are free from the pixel domain as the Primo Play Set.

I chose wood as main material, first of all because it's natural; the feeling you get is very warm and it makes a nice sound. The second reason is cultural. I went to observe the games used in traditional kindergartens in Switzerland (where the product was originally designed) to discover that the games loved by children are all made out of wood. These toys are very durable and you can see marks and scratches on them, signs of their past usage from other children. It's a material with memory. 
In the  third place, I chose wood because of the contrast that it makes with technology. Inside of Primo there's a circuit board, but I wanted to keep everything as magical as possible, hiding the complexity.

<papert>

The concept behind Primo is heavily inspired by the work of Seymour Papert, a mathematician who co-founded the MIT Artificial Intelligence Laboratory with Marvin Minsky, in the sixties (if you are interested in the subject, we encourage you to read Mindstorms, his most famous book). He was directing the team who invented LOGO, probably the most used and long lasting resource to teach programming to children. The goal of Seymour Papert was not just to teach code, but also to help children discover their own personal way of solving problems. Primo can be considered an extreme simplification of LOGO and the physical turtle. We limited the instructions, to their purest form, avoiding any kind of textual or numerical language.

I realized the first prototype in SUPSI Lugano, during the [MAInD - Master of Advanced Studies in Interaction Design](http://www.maind.supsi.ch/). My background is in product design, at the time I just learned the Arduino basics and a bit of code, so after the concept, I started to look around for technical solutions that were approachable for me at the time to develop this kind of application. The main issues were two: making a robot car from scratch and an interface board that could easily recognize different kinds of instructions.

For the first issue I was lucky enough to get a [Oh_Oh board](http://david.cuartielles.com/w/Maquila2/Ohoh) from David Cuartielles, one of the Arduino founders who was holding a lecture in SUPSI. The Oh_Oh robot is an open project, you can find the source files in the link above. It is basically a car shaped Arduino, I just had to add an XBee for radio communication.

The second issue was how to design a reliable way to detect the blocks. I started to look around for solutions and the inspiration came from a [CIID](http://ciid.dk/) project called ["Barcode Piano"](http://ciid.dk/education/portfolio/idp11/courses/physical-computing/projects/barcode-piano/). 

<embed-barcode piano>

The idea is to use multiple blocks that can be recognized by a board using resistors. It's a basic voltage divider: with the analog pins of an Arduino I can read the resistor values. It's a very simple method, but rather effective for a prototype.

Design wise there are some features that required testing, for this reason I went trough some testing iterations before arriving at the actual design. 

The 'snake' or 'zig-zag' path of the instruction sequence is due to avoid literacy pre-conceptions.  

<literacy illustration>

Then there's the 'D' shape of the blocks. The reason for this is because the blocks can be inserted just in one way, to be consistent with the path design and the direction of the car. Multiple designs can be used for this. The D shape was chosen as it is basically an 'oriented circle' and circle is the shape that I wanted to use from the beginning, to recall similar pin-board designs.

<instruction blocks>

Instruction Blocks design is still in testing. The actual design works fine, children get the idea very quickly, they are just confused between left and right. We are currently testing more designs to see if this can be improved.

<primo vimeo concept video embed>

At the beginning the design for the robot was a toy car. It was very complicated and time consuming to produce them, as it's all laser-cut layer by layer then glued together, then sanded for like one hour. The car had another major issue, it was very boy oriented. We are aware of the big discussion that involves 'brain toys' producer, claiming that the majority of them are all boy-oriented. Think about LEGO or Meccano. We totally agree that the way to go is gender neutral, we didn't want to create a toy specifically for boys or girls, so we opted for a very neutral geometry, a box.

We gave the little box a personality, to make it appealing for children, we drew a face on it and we called it Cubetto (little cube in Italian). The idea with Cubetto is also to create a basic module that can be expanded and customized.

<cubetto face>

##3. Getting Started

###3.1 The basics

Primo is composed of three parts: Cubetto, Interface Board and Instruction Blocks ans children interact with Interface Board by placing Instruction Blocks into the holes, to create a sequence. 

There are four types of Instruction Blocks, this means that we will use resistors of 4 different values, possibly quite distant between each other.

The blocks are inserted into the holes of the Interface Board, where the resistor value is identified. After that, the values are processed into a string that is sent to Cubetto using two XBee modules. Cubetto then executes the instructions, one after the other.

The brain of the prototype are two Arduino Boards, a UNO (or Leonardo, even Duemilanove maybe) for Cubetto, and a Mega for the Interface Board, where we need 16 analog inputs.

###3.2 Electronics

Tools Required

* Soldering Iron
* Solder
* Wires
* Hot Glue Gun
* Wood Glue
* Copper Tape 5mm wide

Cubetto

* Arduino UNO (or Leonardo) - 20 + VAT
* Arduino Proto Wireless Shield - 14.90 + VAT
* SN754410 Motor Driver - 3.90 + VAT
* XBee (series 1 or 2, doesn't make any difference) - 23.90 + VAT
* SolarBotics Wheels x 2 - 4.74
* SolarBotics Gear Motors GM3 x 2 - 8.36
* CNY70 x 2 - 1
* 2 Ball Casters
(* Battery Holder - 2)
(* 4 x Rechargeable Batteries)

Interface Board

* Arduino Mega 2560 - 39.00 + VAT
* Arduino Proto Wireless Shield - 14.90 + VAT
* 16 5mm Red LED - 2.5
* 16 220 Ω Resistors - 1
* 16 10K Ω Resistors - 1
* 1 Push Button - 1.9
* 16 Magnets ø 4 h 3
* 50 Male Headers
* 16 Double male headers
* 50 female headers

Instruction Blocks

* 4 x 4.7K Ω Resistor
* 4 x 100K Ω Resistor
* 4 x 220 Ω Resistor
* 4 x 10K Ω Resistor
* 16 Magnets ø 4 h 3

###3.3 Energy

Cubetto and (optionally) Interface Board, are battery powered. For the prototype you can use LiPo battery or regular AA batteries, that's entirely up to you. We used both, LiPo batteries are good but you need some extra equipment, if you are starting from scratch we recommend AA batteries. Just mind that they disacharge very quickly, so the best would be to use rechargeable batteries, like NiMh.

###3.4 Prototype Design

The whole product is made out of laser cut wood, mainly 4 mm thick, just one layer is 1mm. You can laser this using Ponoko or other local services, like a FabLab. The first prototype was laser cut inside FabLab Lugano, while the product development advanced in FabLab Torino, where part of Primo development team still resides.

Building Cubetto and the Interface Board it's quite long but very simple, as their shells are basically boxes. The real complexity lays in the Instruction Blocks.
They are a double 4mm wood layer with magnets and resistors soldered inside.

##4. Prototype Making

###4.1 Interface Board

To make the interface board you have to laser cut two files: interfaceBoard4.dxf and interfaceBoard1.dxf: the first one is for 4mm plywood and the second one for 1mm plywood. As you can see from the files, the parts are numbered, to ease thew assembly process. The numbers are stored on a different layer, so you can easily remove them before laser cutting. I recommend to adjust the hole for the push button, based on the size of the button that you have.

First of all, you have to glue parts 3 and 4 together, use the holes in the corners to align them while gluing and let it rest for a night. 

Then take the copper tape, cut 32 pieces of 70mm each and put them inside the rectangular holes in the part that you just glued, they should be at least 30mm wide on each side. Once you finished, you can now glue all the remaining top layers of the interface board, this is the correct order:

<order>

Once the glue has dried, we put the magnets in the little holes. Turn your top layer upside-down and fill the little holes with the magnets, all in the same direction of course. Doesn't matter if north or south, just be very sure that they are all facing the same direction (either all the North or South end facing the same side). Seal the hole with a drop of hot glue.

Now the electronics. Start by making rails for the 5V and the GND, all along the hole lines as in the picture. I used to make them using naked wire, just in my last prototype i tried to use copper tape also for the rails and it's really time saving. Also, you can create connections very easily. 

The next step is to wire one of the two connectors of every hole, to the ground rail. If you used copper tape, you can just use a tiny extra bit of it, just enough to touch both ends.

Now we have to connect the other side of each connector to the 5V rail, but this time, with a 10KΩ resistor in-between. A cool thing of copper tape is that solder melts very well on top of it. This is the technique i used:

<10k-connector>

At the end of this process, you should have something like this:

<10k-scheme>

Now it's time to put the LEDs; stick one red LED in each one of the 16 holes, then use a drop of hot glue to seal them to the wood. Once the glue is cold, we have to connect them. Just mind that LEDs have a polarity: the long leg is the anode and the short one the cathode. Connect each cathode to the ground rail, using a 220Ω Resistor.

<illustration-leds>

The long leg of the LED, must be connected to a basic Arduino digital pin I/O pin On the Arduino Mega, these pins are numbered from 22 to 53. The LEDs must be connected in order, so that it will be much easier to access them later on in the code, in my prototype for example I started from pin number 30 up to 45 (there are 16 LEDs). The starting point is not important, as long as they are in the correct sequencial order. This means for example that if we start from pin 30, the first LED must be attached to pin 30, the second to pin 31, the third to pin 32 and so on until LED 16 to pin 45. 

I soldered the cables to a rack of double male headers, as the digital pins on the Arduino Mega are layed out in a double line. In this way it's easy to plug and remove the Arduino from the board.

<rack headers>

Once all the LEDs are soldered, we have to solder our hand made connectors. These must be wired to the Arduino Mega analog pins, to read the different resistor values. Just like the LEDs, these must be connected in order, starting from A0 for hole 1 to A15 for hole 16. The wire has to start from the same point where we soldered previously the 10K resistor. See illustration:

<illustration connessioni connectors>

Here I used some single male headers, as the analog pins are all on a single line.

The last thing to connect is the button: take it and solder two cables to two opposite headers, then slip them trough the button hole, from the top, and push it all the way down, until it stops. Now flip the board, you should have the two wires coming out of the hole. Connect them as in the following illustration: one straight to 5V, the other one to GND using a 10k Resistor. Then connect it to an Arduino digital pin from the button-end of the resistor, I used pin number 50.

<button-illustration>

Almost done with the board, now you just have to plug the Wireless Shield on top of the Arduino Mega and stick the headers in place in the board. To recap, 30 to 45 for the LEDs, A0 to A15 for the connectors and 50 for the button. Use the A0 to A5 pins on the Wireless Shield for the first 5 connectors. 

Last thing: don't forget to connect the ground rail to the GND pin and the 5V to the 5V pin.

###INSTRUCTION BLOCKS

This is one instruction block, exploded:

<esploso>

To make the Instruction Blocks, the first thing you have to do is laser cut the files, there's one for 4mm thick wood and one for 1mm wood. They are four layers, numbered from 1 to 4 and the drawings provided can be used to make 16 blocks, four of each kind.

Each one of the four types of the blocks has a different resistor. The way I used them in the prototype is the following:

FORWARD: 4.7K Ω
LEFT: 100K Ω
RIGHT: 220 Ω
FUNCTION: 10K Ω

To make blocks, first you have to glue part 4 with part 3. 

After the glue has dried, this is the moment to paint the product. See the illustration below to see what part should be colored:

<colors>

Now you have to cut two pieces of copper tape, 40mm long. Slip them in the holes of the two blocks that you just glued, making a ring around it using the upper and lower fessure, the ring must be quite tight.

<ikea-blocks>

After that, you have to put the magnet in the hole. While doing this, BE SURE THAT IT IS CORRECTELY ORIENTED, so that the block 'sticks' into the hole. If you put it the other way, it's going to be repelled by the other magnet, a funny outcome but not what we want to achieve.

After putting the magnet, you can stop it with a little drop of hot glue and before the glue gets cold, put the right resistor on top, with the 'legs' laying on the copper tape. After that, the resistor must be soldered on the two pieces. After soldering, cut the extra leg and glue part 2 on top of the resistor.

Finish your block by gluing the last layer, part number 1, on the top, then repeat the whole process for 16 blocks :)

###CUBETTO

Electronics:

The prototype for Cubetto can be built using an Arduino Uno or Leonardo, with a Proto Wireless Shield on top. The reason for the Proto Shield is because it has a small prototyping area, that is wide enough to put the motor driver, the connectors for the optical encoders, motors and power. 

Cubetto has to spin 90 degrees left and right. A very inaccurate way is tgo use timing event, like "spin right for one second" and you can expect more or less the same result. More or less because it depends a lot from different factors, such as the floor, the battery power and so on. The way I solved this problem, is by detecting the amount of rotation from the wheel using two CNY70 optical encoders in combination with a sticker. The round sticker goes in the inner wheel and it's something like this:

<wheel sticker>

The sticker is split into black and white slices, this is because the CNY70 is able to detect the variation between a white slice and a black one. Basically inside it has an infrared LED that is always on and a phototransistor that is reading the amount of infrared light. When a black material is facing the component, almost no light is relfected, as the black color tends to absorb it. On the contrary, if the material is white, it reflects all the light, so the value read from the sensor it's very high. The difference between readings is used to count the rotation steps.

The prototyping area of the Wireless Proto Shield is where i soldered the motor driver and other connectors for the other parts. For these I used simple male headers as connector and female headers on the other part.

<illu shield>
<male-female connectors>

The SN754410 motor driver has 16 pins that must be connected like in the following scheme:

<SN754410 scheme>

Design:

Start by lasering cubetto.dxf; All Cubetto parts are cut from 4mm plywood, follow these visual instructions to build the base:

<ikea-cubetto>

Don't mount the motors for now, first you have to mount the ball casters.

<ball casters illu>
<ball casters picture>

Now the CNY70. Solder the two opposite headers, that must be connected to 5V, together with a wire; then solder three wires to the remaining headers of the CNY70. At the end of these wires solder a row of three femal headers, that will be connected later on to the headers on the proto shield.

The two cny70 must be placed on the edge of the bottom layer, with the LED and the photoransistot horizontally aligned. To fix them you can use some hot glue (or other types of glue). 

See the picture to understand the location.

<CNY70 photo>

Just like for the CNY70, solder two wires to the little flaps that come out of each motor. You can twist the two wires to make them more resistent, then at the end, solder them to a row of two female header, just like in the illustration.

Now print the inner drawing with the black and white slices, then glue them on a piece of cardboard (or laser cut wood, that's up to you), cut the perimeter and make a hole in the middle, as they will be inserted between the motor and the wheel. The white and black slices must point towards the inner side of Cubetto and the distance between the print and the CNY70 must be between 1 and 3 millimeters for the CNY70 to work properly.

<inner-cubetto-wheel>

Now you can put the wheels on the motors, if you used the Solarbotics wheels, you can fasten them with the screw provided, don't make it too tight. 

Glue three out of the four 'walls' of cubetto, parts 5, 7 and 8. We are going to leave the back removable, just in case we want to modify something. 

Take the battery holder and solder the black and red cable to other 2 female connectors. The headers on the shield will go to VIN and ground. A switch that breaks the red wire is heavily suggested.

Now you can place the Arduino + Proto shield on top of the motors, plug all the headers on the shield and you are done!



