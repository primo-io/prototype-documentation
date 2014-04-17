---
layout: default
title: Primo Prototype Documentatie
language: Nederlands
category: language
---

<br>

<div id="content" markdown="1">
##0. Doel van dit document

![primo play set]({{ site.baseurl }}images/photo/maker-guide.jpg)
Dit document bevat alle informatie die nodig is om een Primo Prototype te maken.
Meer informatie over het project vind je op de [primo.io](http://primo.io)-website.

<br>

##1. Wat is Primo?

![primo play set]({{ site.baseurl }}images/photo/primo.jpg)

Primo is een tastbare interface, ontworpen om programmeerlogica te introduceren bij jonge kinderen (3 tot 7 jaar), zonder dat ze hoeven te kunnen lezen. Het doel van het spel is om een kleine robot, genaamd Cubetto, naar zijn huis te laten rijden. Om dit doel te bereiken, zullen kinderen de  robot moeten programmeren met behulp van een beperkte set instructies: vooruit, linksom, rechtsom en functie. De eerste drie zijn redelijk intuïtief. De laatste roept een subroutine aan; een extra regel met instructies aangeroepen door één commando.

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/82620072" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">        
    </iframe> 
</div>

##2. Onderzoek

Kinderen leren programmeren is een wereldwijd besproken onderwerp. We zijn ons bewust van een bescheiden aantal oplossingen die dit proberen te bereiken voor kinderen van 8 jaar en ouder. Echter, de meeste van deze oplossingen zijn niet geschikt voor jonge kinderen. En geen enkele werken zonder een beeldscherm of zonder te hoeven lezen. Er verschijnt een groeiend aantal apps voor tablets en computers die ook werken in combinatie met fysieke robots, maar geen een van deze zijn volledig vrij van het pixeldomein, zoals de Primo speelset dat is.

Er is voor hout gekozen als primair materiaal, vooral omdat het natuurlijk is; je krijgt warme gevoelens van het en het maakt een mooi geluid. De tweede reden is cultureel. Er is gekeken naar spelletjes in traditionele kleuterscholen in Zwitserland (waar dit product oorspronkelijk is ontworpen) en daaruit bleek dat de geliefde spelletjes allemaal gemaakt zijn van hout. Houten speelgoed zijn zeer duurzaam en je kunt krassen en deuken zien, tekenen van het gebruik van andere kinderen. Het is een materiaal met geheugen. Hout is ook gekozen als materiaal, omdat het een sterk contrast heeft met technologie. Binnenin Primo is een printplaat, maar we wilden een "magische" beleving maken door de complexiteit van de speelset te verbergen.

<img class="float" src="{{ site.baseurl }}images/photo/logo-turtle.jpg">

Het concept achter Primo is sterk geïnspireerd door het werk van Seymour Papert, een wiskundige die in de jaren zestig het MIT Artificial Intelligence Laboratory oprichtte, samen met Marvin Minsky (indien je meer wilt weten of dit onderwerp, dan raden we je aan om [Mindstorms](http://www.amazon.co.uk/Mindstorms-Children-Computers-Powerful-Ideas/dp/0465046746/ref=sr_1_1?ie=UTF8&qid=1393675158&sr=8-1&keywords=mindstorms+papert) te lezen, zijn meest bekende boek). He gaf leiding aan het team dat [LOGO](http://en.wikipedia.org/wiki/Logo_(programming_language)) bedacht, waarschijnlijk de meest en langst gebruikte bron om kinderen te leren programmeren. Het doel van Seymour Papert was niet om alleen alleen te leren coderen, maar ook om kinderen hun eigen manier van probleemoplossing te laten ontdekken. Primo mag beschouwd worden als een extreme versimpeling van LOGO en de fysieke schildpad. We hebben het aantal instructies beperkt, in zijn puurste vorm, om enige tekstuele of numerieke taal te omzeilen.

Het eerste prototype werd gemaakt in SUPSI Lugano door Matteo Loglio (medeoprichter van Primo.io en interactie ontwerper), tijdens zijn [MAInD - Master of Advanced Studies in Interaction Design](http://www.maind.supsi.ch/). Matteo heeft als achtergrond productontwerp. Nadat hij de basis van Arduino had geleerd en een beetje kon programmeren om het prototype te maken, is hij op zoek gegaan naar technische oplossingen, die toegankelijk zijn voor een beginner, om een applicatie te kunnen ontwikkelen, zoals Primo. Er waren twee uitdagingen: een robotauto maken (vanaf nul) en een interfacebord dat makkelijke verschillende instructies herkend.

De eerste uitdaging werd opgelost door een [Oh_Oh board](http://david.cuartielles.com/w/Maquila2/Ohoh) van David Cuartielles te gebruiken, één van de Arduino oprichters die een lezing gaf in SUPSI. De Oh_Oh robot is een open project, je kunt de bronbestanden vinden via bovenstaande link. Het is Arduino in een autovorm; alleen voor de draadloze communicatie werd een XBee toegevoegd.

De tweede uitdaging was het ontwerpen van een betrouwbare manier om de blokken te onderscheiden. De oplossing was geïnspireerd door een [CIID](http://ciid.dk/)-project genaamd ["Barcode Piano"](http://ciid.dk/education/portfolio/idp11/courses/physical-computing/projects/barcode-piano/). 

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/19704918" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">    
    </iframe>
</div> 


Het idee is om meerdere blokken te gebruiken, die door weerstanden herkend worden door een bord. Het is een eenvoudige spanningsdeler, waarbij de analoge pinnen van de Arduino de weerstandwaardes uitlezen. Het is een simpele methode, maar zeer effectief voor een prototype.

Sommige mogelijkheden moesten getest worden; het uiteindelijke ontwerp is het resultaat van meerdere iteraties.

Het 'slang'- of 'zigzag'-pad van de instructievolgorde werd gekozen om invloeden van aangeleerd leesgedrag uit te sluiten.

![left to right]({{ site.baseurl }}images/illustrations/left-to-right.jpg)

De 'D'-vorm van de blokconnectoren zorgt ervoor dat de blokken maar op één manier gebruikt kunnen worden en om consistent te zijn met het padontwerp en de richting van de auto.

![instruction blocks]({{ site.baseurl }}images/photo/instruction-blocks.jpg)

Het ontwerp voor de vorm van de instructieblokken wordt nog steeds getest. Het huidige ontwerp werkt redelijk goed; kinderen pakken makkelijk het juiste blok, ze hebben in het begin alleen wat moeite om te wennen aan de linksom- en rechtsomblokken. Dit komt ook omdat "links" en "rechts" redelijk nieuwe begrippen voor ze zijn. We testen op dit moment andere vormen, om dit nog verder te 

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/50570097" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">
        
    </iframe>
</div>

In eerste instantie was de robot een speelgoedauto. Een zeer complexe en tijdrovende vorm om te maken, omdat het een vorm (uitgesneden met een lasercutter) is die laag voor laag aan elkaar geplakt is en daarna meer dan een uur geschuurd moet worden. De auto had ook een andere beperking; het was zeer gericht op jongens. Als 'breinspeelgoed'-maker wilden we discussies en opmerkingen over jongensgericht speelgoed voorkomen. We wilden neutraal blijven en wilden geen speelgoed ontwerpen speciaal voor jongens of meisjes. Daarom hebben we gekozen voor een zeer neutrale vorm, een doos.

Er werd een naam, persoonlijkheid en een glimlach gegeven aan het doosje, zodat het aantrekkelijker werd voor kinderen. De robot heet "Cubetto" (Italiaans voor "kleine kubus"). Het idee is ook om een basismodule te maken van Cubetto, dat later makkelijk uitgebreid en aangepast kan worden in de toekomst.

![cubetto]({{ site.baseurl }}images/photo/cubetto.jpg)

##3. Om te beginnen

###3.1 De basis

Primo bestaat uit drie delen: een interfacebord, Cubetto en een set instructieblokken. Door instructieblokken in het interfacebord te plaatsen, maken kinderen een instructieset (een programma) welke Cubette uitvoert.

Er zijn vier type instructieblokken. Hierdoor moeten 4 verschillende weerstandwaardes gebruikt worden; het liefst met een groot waardeverschil tussen elkaar.

De blokken worden in de gaten van het interfacebord geplaatst, waar de weerstandwaarde wordt herkent. Daarna worden de waarden verwerkt in een tekenreeks welke naar Cubetto worden gestuurd met behulp van twee XBee-modules. Cubette voert deze instructies vervolgens uit, één voor één.

Het brein van het prototype is gemaakt met twee Arduino's, een UNO (een Leonardo of Duemilanove kan ook) voor Cubetto en een Mega voor het interfacebord, waar 16 analoge inputs nodig zijn.

###3.2 Electronica

###Benodige gereedschappen

* Soldeerbout
* Soldeertin
* Draad
* Lijmpistool
* Houtlijm
* Kopertape (5mm breed)

###Materialen (prijzen in Euro)

Cubetto ~ 88 €

* Arduino UNO (of Leonardo) - 20 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=195#.UxC5nfTV_bA)
* Arduino Proto Wireless Shield - 14.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* SN754410 motor driver - 3.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_33&products_id=153#.UxC5-_TV_bB)
* XBee (serie 1 of 2, maakt niet uit welke) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* SolarBotics wielen x 2 : 4.74 € - [Solarbotics Store](https://solarbotics.com/product/gmpw/)
* SolarBotics Gear Motors GM3 x 2 : 8.36 € - [Solarbotics Store](https://solarbotics.com/product/gm3/)
* 2 ball casters : 5.79 € - [Solarbotics Store](https://solarbotics.com/product/23160/)
* CNY70 x 2 : 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Vishay/CNY70/?qs=%2fha2pyFaduj8YpDhNNtXszq4w32cl%2fAjUjdOwQUvJUM%3d)
* (optioneel) batterijhouder : 4 € - [Solarbotics Store](https://solarbotics.com/product/bholdaa_4_cell/)
* (optioneel) 4 x oplaadbare batterijen

Interfacebord ~ 88 € (puur toeval)

* Arduino Mega 2560 : 39.00 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=196#.UxC_gPTV_bA)
* Arduino Proto Wireless Shield : 14.90 - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* XBee (serie 1 of 2, maakt niet uit welke) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* 16 5mm rode LED's : 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Lite-On/LTL-4223/?Lite-On/LTL-4223/&qs=sGAEpiMZZMusoohG2hS%252b15J8d1kHl%252bvkJpzS4atZNEA=)
* 16 220 Ω weerstanden : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 16 10K Ω weerstanden : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 1 knop : 1 € 
* 50 male Headers : 1 € 
* 16 dubbele male headers : 0.50 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=294#.UxC_3fTV_bA)
* 50 female headers : 1 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=188#.UxDAAfTV_bA)
* 16 magneten ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

Instructie blokken ~ 4 €

* 4 x 4.7K Ω weerstand : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-47K-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2fbdyz6pU6a%252bvHlD5kaZWgo%3d)
* 4 x 100K Ω weerstand : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-100K-RC/?qs=sGAEpiMZZMu61qfTUdNhG81NIhcRRUJQxII5Nsctha8%3d)
* 4 x 220 Ω weerstand : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 4 x 10K Ω weerstand : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 16 magneten ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

###3.3 Spanning

Cubetto en (optioneel) het interfacebord worden gevoed door batterijen. Je kunt LiPo- of AA-batterijen gebruiken voor het prototype, die keuze is aan jou. Wij hebben beide gebruikt; LiPo-batterijen zijn erg goed, maar hebben extra producten nodig. Als je vanaf nul begint, raden we AA-batterijen aan. Ze raken wel snel leeg; daarom kun je het beste oplaadbare batterijen gebruiken, zoals NiMh.

###3.4 Ontwerp van het prototype

Het hele product is gemaakt van hout en uitgesneden met behulp van een lasercutter. Er is voornamelijk hout van 4 mm gebruikt, terwijl één laag 1 mm dik hout gebruikt. Je kunt deze onderdelen laten snijden door een dienst zoals Ponoko of in een FabLab bij je in de buurt. Het eerste prototype werd gemaakt in [FabLab Lugano](http://fablab.supsi.ch/). Het ontwerp werd verder ontwikkeld in [FabLab Torino](http://fablabtorino.org/), waar een deel van het Primo-ontwerpteam nog steeds zit.

Het maken van Cubetto en het interfacebord is een bewerkelijk, maar erg simpel proces. Hun buitenkant zijn in de basis dozen. De echte complexiteit ligt in de instructieblokken. Deze zijn gemaakt van een dubbele 4mm houten laag met een magneet en een gesoldeerde weerstand binnenin.

##4. Het prototype maken

###[Download de bestanden voor de lasercutter](files/primo-prototype-laser.zip)

###4.1 Interfacebord

To make the interface board you have to laser cut two files: interface-board-4mm.dxf and interface-board-1mm.dxf: the first one is for 4mm plywood and the second one for 1mm plywood. As you can see from the files, the parts are numbered, to ease the assembly process. The numbers are stored on a different layer, so you can easily remove them before lasering. We recommend adjusting the hole for the push button, based on the size of the button you wish to use or have.

First of all, you have to glue parts 3 and 4 together, use the holes in the corners to align them with screws while gluing and let it rest for a night. 

Then take the copper tape, cut 32 pieces of 70mm each and put them inside the rectangular holes in the part that you just glued, they should be at least 30mm wide on each side. Once you finished, you can now glue all the remaining top layers of the interface board, this is the correct order:

Then take the copper tape, cut 32 pieces of 70mm each and put them inside the rectangular holes in the part that you just glued, they should be at least 30mm wide on each side. 

![copper connectors]({{ site.baseurl }}images/illustrations/board-1.jpg)
![copper connectors]({{ site.baseurl }}images/illustrations/board-2.jpg)

Once you finished, you can now glue the previously glued parts, 1+2 with 3+4.

![copper connectors]({{ site.baseurl }}images/illustrations/board-esploso.jpg)

Once the glue has dried, put the magnets in the little holes. Turn your top layer upside-down and fill the little holes with the magnets, make sure they are all in the same direction, doesn't matter if north or south. Seal the hole with a drop of hot glue.

Now the electronics. Start by making rails for the 5V and the GND, all along the hole lines like in the picture. The first ever prototype never had copper strips, it had wires (which you can also use), but in this prototype we used copper tape also for the rails. A real 100% time saver. It also makes things easier for creating connections.

![rails]({{ site.baseurl }}images/illustrations/board-3.jpg)

The next step is to wire one of the two connectors of every hole, to the ground rail. If you used copper tape, you can just use a tiny extra bit of it, just enough to touch both ends.

![rails]({{ site.baseurl }}images/illustrations/board-5.jpg)

Now we have to connect the other side of each connector to the 5V rail, but this time, with a 10KΩ resistor in-between. A cool thing of copper tape is that solder melts very well on top of it. This is the technique used:

![10k]({{ site.baseurl }}images/photo/diy-docs-1.jpg)

At the end of this process, you should have something like this:

![10k scheme]({{ site.baseurl }}images/illustrations/board-6.jpg)

Now it's time to put the LEDs; stick one red LED in each one of the 16 holes, then use a drop of hot glue to seal them to the wood. Once the glue is cold, we have to connect them. Just mind that LEDs have a polarity: the long leg is the anode and the short one the cathode. Connect each cathode to the ground rail, using a 220Ω Resistor.

![10k]({{ site.baseurl }}images/photo/diy-docs-6.jpg)

Connect each cathode to the ground rail, using a 220Ω Resistor.

![10k scheme]({{ site.baseurl }}images/illustrations/board-7.jpg)

The long leg of the LED, must be connected to a digital I/O pin on the Arduino Mega, these pins are numbered from 22 to 53. The LEDs must be connected in order, so that it will be much easier to access them later on in the code, in my prototype for example I started from pin number 30 up to 45 (there are 16 LEDs). 
The starting point is not important, as long as they are in the correct sequential order. This means for example that if we start from pin 30, the first LED must be attached to pin 30, the second to pin 31, the third to pin 32 and so on until LED 16 to pin 45. 

The cables are soldered to a rack of double male headers, as the digital pins on the Arduino Mega are laid out in a double line. In this way it's easy to plug and remove the Arduino from the board.

![rack]({{ site.baseurl }}images/photo/diy-docs-4.jpg)

Once all the LEDs are soldered, we have to solder our hand made connectors. These must be wired to the Arduino Mega analog pins, to read the different resistor values. Just like the LEDs, these must be connected in order, starting from A0 for hole 1 to A15 for hole 16. The wire has to start from the same point where we soldered previously the 10K resistor. See the illustration:

![analog input board connections]({{ site.baseurl }}images/illustrations/board-8.jpg)

<div class="cf">
<img class="float cf" src="{{ site.baseurl }}images/illustrations/button.jpg">

<p>
Here I used some single male headers, as the analog pins are all on a single line.
	
</p>

<p>
The last thing to connect is the button: take it and solder two cables to two opposite headers, then slip them trough the button hole, from the top, and push it all the way down, until it stops. Now flip the board, you should have the two wires coming out of the hole. Connect them as in the illustration: one straight to 5V, the other one to GND using a 10k Resistor. Then connect it to an Arduino digital pin from the button-end of the resistor, in this example we used pin number 50.
</p>
</div>


![photo]({{ site.baseurl }}images/photo/diy-docs-5.jpg)

Almost done with the board, now you just have to plug the Wireless Shield on top of the Arduino Mega and stick the headers in place in the board. To recap, 30 to 45 for the LEDs, A0 to A15 for the connectors and 50 for the button. Use the A0 to A5 pins on the Wireless Shield for the first 5 connectors. Don't forget to connect the ground rail to the GND pin and the 5V to the 5V pin.

![rack]({{ site.baseurl }}images/photo/diy-docs-3.jpg)

Now a little bit of fine-tuning: after that part 12 of the board has been painted, you can glue it with part 13 on top of the board.

Same for the red button: after part 14 has been painted, put something soft like cardboard on top of part 2, around the push button, then some hot glue on top of the push button and before the glue dries off, place the red button. See the illustration:

![photo]({{ site.baseurl }}images/illustrations/button-mechanics.jpg)

###INSTRUCTION BLOCKS

This is one instruction block, exploded:

<img class="float cf" src="{{ site.baseurl }}images/illustrations/instruction-esploso.jpg">

To make the Instruction Blocks, the first thing you have to do is laser cut the files, there's one for 4mm thick wood and one for 1mm wood. They are four layers, numbered from 1 to 4 and the drawings provided can be used to make 16 blocks, four of each kind.

Each block has a different resistor. These are the resistors used in the prototype:

FORWARD: 4.7K Ω<br>
LEFT: 100K Ω<br>
RIGHT: 220 Ω<br>
FUNCTION: 10K Ω

To make blocks, first you have to glue part 4 with part 3. 

After the glue has dried, you can start painting. See the illustration below to see what part should be colored:

![image]({{ site.baseurl }}images/illustrations/colors.jpg)

Now you have to cut two pieces of copper tape, 40mm long. Slip them in the holes of the two blocks that you just glued, making a ring around it using the upper and lower fissure, the ring must be quite tight.

![photo]({{ site.baseurl }}images/illustrations/instruction-block-guide.jpg)

After that, you have to put the magnet in the hole. While doing this, BE SURE THAT IT IS CORRECTELY ORIENTED, so that the block 'sticks' into the hole. If you put it the other way, it's going to be repelled by the other magnet, a funny outcome but not what we want to achieve.

Fix the magnet with a drop of hot glue and before the glue gets cold, put the right resistor on top, with the 'legs' laying on the copper tape. After that, the resistor must be soldered on the two pieces. After soldering, cut the extra leg length and glue part 2 on top of the resistor.

Finish your block by gluing the last layer, part number 1, on the top, then repeat the entire process for every single block :)

###CUBETTO

Electronics:

The prototype for Cubetto can be built using an Arduino Uno or Leonardo, with a Proto Wireless Shield on top. The reason for the Proto Shield is because it has a small prototyping area, that is wide enough to put the motor driver, the connectors for the optical encoders, motors and power. 

Cubetto has to spin 90 degrees left and right. A very inaccurate way is to use timing event, like "spin right for one second" and you can expect more or less the same result. "More or less" because it depends a lot from different factors, such as the floor, the battery power and so on. The way I solved this problem, is by detecting the amount of rotation from the wheel using two CNY70 optical encoders in combination with a sticker. The round sticker goes in the inner wheel and it's something like this:

![photo]({{ site.baseurl }}images/photo/diy-docs-14.jpg)

The sticker is split into black and white slices, this is because the CNY70 is able to detect the variation between a white slice and a black one. Basically inside it has an infrared LED that is always on and a phototransistor that is reading the amount of infrared light. When a black material is facing the component, almost no light is relfected, as the black color tends to absorb it. On the contrary, if the material is white, it reflects all the light, so the value read from the sensor it's very high. The difference between readings is used to count the rotation steps.

![photo]({{ site.baseurl }}images/illustrations/cny70-physycs.jpg)

The prototyping area of the Wireless Proto Shield is where the motor driver and other connectors for the other parts are soldered. For these, simply use male headers as connector and female headers on the other part.


![photo]({{ site.baseurl }}images/illustrations/wireless-shield-connections.jpg)

For these I used simple male headers as connector and female headers on the other part.

![photo]({{ site.baseurl }}images/photo/diy-docs-12.jpg)

![photo]({{ site.baseurl }}images/illustrations/wireless-shield-connections-1.jpg)

The SN754410 motor driver has 16 pins that must be connected following this scheme:

![photo]({{ site.baseurl }}images/illustrations/motor-driver.jpg)

The CNY70 scheme:

<img style="width:50%" src="{{ site.baseurl }}images/illustrations/cny70-wiring.jpg">

Design:

Start by lasering cubetto.dxf; All Cubetto parts are cut from 4mm plywood, follow these visual instructions to build the base:

![photo]({{ site.baseurl }}images/illustrations/cubetto-guide.jpg)

Don't mount the motors for now, first you have to mount the ball casters.

![photo]({{ site.baseurl }}images/illustrations/ball-caster.jpg)

![photo]({{ site.baseurl }}images/photo/diy-docs-9.jpg)

Now the CNY70. Solder the two opposite headers, that must be connected to 5V, together with a wire; then solder three wires to the remaining headers of the CNY70. At the end of these wires solder a row of three female headers. They will later be connected on to the headers of the proto shield.

The two cny70 must be placed on the edge of the bottom layer, with the LED and the photoransistot horizontally aligned. To fix them you can use some hot glue (or other types of glue). 

See the picture to understand the location.

![photo]({{ site.baseurl }}images/photo/diy-docs-11.jpg)

Just like for the CNY70, solder two wires to the little flaps that come out of each motor. You can twist the two wires to make them more resistent, then at the end, solder a row of two female header, just like in the illustration.

Now print the inner drawing with the black and white slices, glue them on a piece of cardboard (or laser cut wood, that's up to you), cut the perimeter and make a hole in the middle, as they will be inserted between the motor and the wheel. The white and black slices must point towards the inner side of Cubetto and the distance between the print and the CNY70 must be between 1 and 3 millimeters for the CNY70 to work properly.

![photo]({{ site.baseurl }}images/photo/diy-docs-10.jpg)

Now you can put the wheels on the motors, if you used the Solarbotics wheels, you can fasten them with the screw provided, don't make it too tight. 

Glue three out of the four 'walls' of Cubetto, parts 5, 7 and 8. We are going to leave the back removable, just in case we want to modify something. 

Take the battery holder and solder the black and red cable to other 2 female connectors. The headers on the shield will go to VIN and ground. A switch that breaks the red wire is heavily suggested.

![photo]({{ site.baseurl }}images/photo/diy-docs-13.jpg)

Now you can place the Arduino + Proto shield on top of the motors, plug all the headers on the shield and you have finished making Cubetto.
</div>

##Arduino

###[Download Arduino-bestanden](https://github.com/primo-io/arduino-sketches/raw/master/primo-prototype-arduino.zip)

De instructies staan als commentaar in de sketches.