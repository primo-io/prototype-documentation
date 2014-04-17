---
layout: default
title: Primo prototype documentatie
language: Nederlands (in bewerking)
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
* 16 220Ω-weerstanden : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 16 10KΩ-weerstanden : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 1 knop : 1 € 
* 50 male Headers : 1 € 
* 16 dubbele male headers : 0.50 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=294#.UxC_3fTV_bA)
* 50 female headers : 1 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=188#.UxDAAfTV_bA)
* 16 magneten ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

Instructie blokken ~ 4 €

* 4 x 4.7KΩ-weerstand : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-47K-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2fbdyz6pU6a%252bvHlD5kaZWgo%3d)
* 4 x 100KΩ-weerstand : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-100K-RC/?qs=sGAEpiMZZMu61qfTUdNhG81NIhcRRUJQxII5Nsctha8%3d)
* 4 x 220Ω-weerstand : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 4 x 10KΩ-weerstand : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 16 magneten ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

###3.3 Spanning

Cubetto en (optioneel) het interfacebord worden gevoed door batterijen. Je kunt LiPo- of AA-batterijen gebruiken voor het prototype, die keuze is aan jou. Wij hebben beide gebruikt; LiPo-batterijen zijn erg goed, maar hebben extra producten nodig. Als je vanaf nul begint, raden we AA-batterijen aan. Ze raken wel snel leeg; daarom kun je het beste oplaadbare batterijen gebruiken, zoals NiMh.

###3.4 Ontwerp van het prototype

Het hele product is gemaakt van hout en uitgesneden met behulp van een lasercutter. Er is voornamelijk triplex van 4 mm gebruikt, terwijl één laag 1 mm dik hout (vliegtuigtriplex) gebruikt. Je kunt deze onderdelen laten snijden door een dienst zoals Ponoko of in een FabLab bij je in de buurt. Het eerste prototype werd gemaakt in [FabLab Lugano](http://fablab.supsi.ch/). Het ontwerp werd verder ontwikkeld in [FabLab Torino](http://fablabtorino.org/), waar een deel van het Primo-ontwerpteam nog steeds zit.

Het maken van Cubetto en het interfacebord is een bewerkelijk, maar erg simpel proces. Hun buitenkant zijn in de basis dozen. De echte complexiteit ligt in de instructieblokken. Deze zijn gemaakt van een dubbele 4mm houten laag met een magneet en een gesoldeerde weerstand binnenin.

##4. Het prototype maken

###[Download de bestanden voor de lasercutter](files/primo-prototype-laser.zip)

###4.1 Interfacebord

Om het interfacebord te maken heb je twee bestanden nodig: interface-board-4mm.dxf en interface-board-1mm.dxf: het eerst is voor het triplex van 4 mm dik en de tweede voor het triplex van 1 mm dik. De onderdelen zijn genummerd, zodat je ze makkelijk kunt samenvoegen. De nummer zitten in een aparte laag in het bestand, dus je kunt ze makkelijk verwijderen voordat je gaat snijden. We raden je aan om het gat voor de knop aan te passen aan de grootte van de knop die je gaat gebruiken.

Lijm de delen 1 en 2 aan elkaar. Lijm ook de delen 3 en 4 aan elkaar. Je kunt de gaten in de hoeken gebruiken om de delen te positioneren met behulp van boutjes en moertjes terwijl de lijm een nachtje droogt.

Knip daarna 32 stukken kopertape van 70 mm lang per stuk en plak deze in de rechthoekige gaten in het deel (laag 3+4) dat je zojuist gelijmd hebt; aan beide zijden moet minimaal 30 mm zitten.

![copper connectors]({{ site.baseurl }}images/illustrations/board-1.jpg)
![copper connectors]({{ site.baseurl }}images/illustrations/board-2.jpg)


Zodra je klaar bent, kun je de twee delen aan elkaar plakken, 1+2 aan 3+4.

![copper connectors]({{ site.baseurl }}images/illustrations/board-esploso.jpg)

Zodra de lijm droog is, plaats je de magneten in de kleine gaten. Leg de toplaag op de kop en plaats de magneten in de kleine gaten, zorg ervoor dat de polariteit van de magneten allemaal gelijk is, het maakt niet uit dat noord of zuid is. Lijm de magneten vast met een druppel lijm.

Nu verder met de electronica. Maak twee sporen voor 5V en GND, zoals je hieronder ziet in de afbeelding. Het eerste prototype had geen kopersporen, het had draden (dat kun je ook gebruiken), maar in dit prototype hebben we kopertape gebruikt voor de sporen. Dat scheelt je 100% van de tijd. Het maakt het maken van verbindingen ook makkelijker.

![rails]({{ site.baseurl }}images/illustrations/board-3.jpg)

De volgende stap is het verbinden van één van de connectoren van elk gat aan het GND-spoor. Als je kopertape hebt gebruikt, kun je een extra stukje toevoegen, zodat deze beide uiteinden raakt.

![rails]({{ site.baseurl }}images/illustrations/board-5.jpg)

Nu gaan we de andere connector verbinden aan het 5V-spoort, maar nu met een 10KΩ-weerstand ertussen. Een mooie bijkomstigheid van kopertape is dat het soldeertin makkelijk erop smelt. Deze techniek is gebruikt:

![10k]({{ site.baseurl }}images/photo/diy-docs-1.jpg)

Dit is wat je ongeveer moet hebben als je klaar bent:

![10k scheme]({{ site.baseurl }}images/illustrations/board-6.jpg)

Nu kun je de LED's plaatsen; stop één rode LED in elk van de 16 gaten en zet deze vast m.b.v. het lijmpistool. Zodra de lijm koud is, kun je 'm verbinden. Houd er rekening mee dat LED's polariteit hebben: de lange draad is de anode en de korte de cathode.

![10k]({{ site.baseurl }}images/photo/diy-docs-6.jpg)

Verbind elke cathode aan het GND-spoor met een 220Ω-weerstand ertussen in.

![10k scheme]({{ site.baseurl }}images/illustrations/board-7.jpg)

De lange draad van een LED wordt verbonden aan een digitale I/O-pin van de Arduino Mega; deze pinnen zijn genummerd van 22 t/m 53. De LED's moeten in volgorde aangesloten worden, zodat het makkelijker wordt om ze in de code aan te sturen. In mijn prototype heb ik, bijvoorbeeld, de pinnen 30 t/m 45 gebruikt (er zijn 16 LED's).
Het startpunt is niet belangrijk, zolang je ze maar in de juiste volgorde aansluit. Dit betekent dat als we, bijvoorbeeld, beginnen met pin 30, de eerste LED aan pin 30 verbonden moet worden, de tweede aan pin 31, de derde aan pin 32 enzovoorts, tot en met LED 16 aan pin 45.

De draden zijn gesoldeerd aan de dubbele male headers, omdat de digitale pinnen van de Arduino Mega in een dubbele lijn zijn gepositioneerd. Op deze manier is het makkelijk om de LED's aan te sluiten en om de Arduino uit het bord te verwijderen.

![rack]({{ site.baseurl }}images/photo/diy-docs-4.jpg)

Zodra alle LED's zijn gesoldeerd, moeten we onze handgemaakte connector solderen. Deze worden aangesloten op de analoge pins van de Arduino Mega, om de verschillende weerstandwaardes uit te lezen. Net zoals bij de LED's moeten deze in de juiste volgorde worden aangesloten, te beginnen bij A0 voor gat 1 t/m A15 voor gat 16. De draad begint op dezelfde plek als waar we de 10K-weerstand hebben vastgemaakt. Zie deze illustratie:

![analog input board connections]({{ site.baseurl }}images/illustrations/board-8.jpg)

<div class="cf">
<img class="float cf" src="{{ site.baseurl }}images/illustrations/button.jpg">

<p>
Hier heb ik enkele male headers gebruikt, omdat de analoge pinnen op één lijn staan.
	
</p>

<p>
Het laatste om te verbinden is de knop: pak het en soldeer twee draden aan de tegen overelkaar gelegen headers. Plaats de knop dan in het bijbehorende gat vanaf de bovenkant en druk het helemaal naar beneden, totdat het niet verder kan. Draai nu het bord om; er moeten nu twee draden uit de gaten komen. Verbind deze zoals je in de afbeelding ziet: één direct naar het 5V-spoor, de andere naar het GND-spoor met een 10K-weerstand ertussen. Verbind het dan met een digitale pin van de Arduino vanaf de 'knop'-kant van de weerstand. In dit voorbeeld gebruiken we pin 50.
</p>
</div>


![photo]({{ site.baseurl }}images/photo/diy-docs-5.jpg)

Het bord is nu bijna klaar, we hoeven nu alleen nog maar het Wireless Shield op de Arduino Mega te plaatsen en de headers op de juiste plaats in het bord te steken. Ter herinnering, 30 t/m 45 zijn voor de LED's, A0 t/m A15 voor de blokconnectoren en 50 voor de knop. Gebruik de A0 t/m A5-pinnen voor het Wireless Shield voor de eerste 5 connectoren. Vergeet niet om het GND-spoor te verbinden aan de GND-pin en het 5V-spoor aan de 5V-pin.

![rack]({{ site.baseurl }}images/photo/diy-docs-3.jpg)

Nu een beetje afwerking: nadat je deel 12 van het bord hebt geverfd, kun je het vastlijmen aan deel 13 van het bord.

Hetzelfde geldt voor de rode knop: nadat deel 14 is geverfd, bevestig je iets zachts (zoals karton) op deel 2 rondom de knop en dan wat lijm op de knop en, voordat de lijm droog is, bevestig je de drode knop. Zie de afbeeldingen:

![photo]({{ site.baseurl }}images/illustrations/button-mechanics.jpg)

###INSTRUCTIEBLOKKEN

Dit is één van de instructieblokken, in onderdelen:

<img class="float cf" src="{{ site.baseurl }}images/illustrations/instruction-esploso.jpg">

Om de instructieblokken te maken, begin je met het snijden van het hout (m.b.v. een lasercutter). Er zijn twee bestanden nodig: één voor het 4 mm triplex en één voor het 1 mm triplex. De blokken bestaan uit 4 lagen, genummerd 1 t/m 4. Met de onderdelen uit de twee bestanden, kun je precies 16 blokken maken, vier van elk type.

Elk blok heeft een andere weerstand. Dit zijn de weerstanden die gebruikt zijn in het prototype:

VOORUIT: 4.7K Ω<br>
LINKSOM: 100K Ω<br>
RECHTSOM: 220 Ω<br>
FUNCTIE: 10K Ω

Lijm eerst de delen 3 en 4 aan elkaar.

Zodra de lijm droog is, kun je gaan verven. In de afbeelding hieronder zie je de kleuren die elk onderdeel moet krijgen:

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