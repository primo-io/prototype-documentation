---
layout: default
title: Cubetto prototip dokumentacija
language: Hrvatski
category: language
---

<br>

<div id="content" markdown="1">
## 0. Što se nalazi u ovom dokumentu?

![primo play set]({{ site.baseurl }}images/photo/maker-guide.jpg)
U ovom dokumentu se nalaze prikupljene sve informacije i uputstva potrebna da biste izgradili Primo prototip. Više o samom projektu možete naći na stranicama [primo.io](http://primo.io).

<h2>
<a href="#" id="translate-title">
    How to translate this document
</a>
</h2>


<div markdown="1" id="translate">

If you want to translate this page in your language, you have multiple options:

1. **super easy, no automation** Copy and paste this page in your text editor, translate it then mail it to us at [play@primo.io](mailto:play@primo.io)

2. **medium, light automation** Create an account on [GitHub](http://github.com), then open the [repository of this page](https://github.com/primo-io/prototype-documentation/blob/gh-pages/index.md) and click on 'EDIT', in the top menu bar:
![photo]({{ site.baseurl }}images/screenshots/edit-1.jpg)
Then your page turns into a text editor, where you are able to modify the page source. The page is written in [markdown](http://daringfireball.net/projects/markdown/syntax), very easy to understand.
![photo]({{ site.baseurl }}images/screenshots/edit-2.jpg)
You don't have to modify this code, but just copy and paste the whole text in your local text editor, then translate the textual parts in your language, without modifying the parenthesis and HTML parts. Save the text then mail it to us at [play@primo.io](mailto:play@primo.io)

3. **advanced, full automation** This is slightly advanced, but nothing too hard, if you are not familiar with GitHub you have the chance to learn something new :) <br>
If you are already familiar with git, you have to fork the repository, all the translations are located in the 'languages' folder. To translate the page, just copy it with the starting language ("english.md" for example) in the same folder, then change the file name with the final language (spanish.md). Change the page header values 'title' (title in your language) and 'language' (the destination language with Capital letter) then translate the rest of the document. Once finished, make a pull request to add your file to the folder, it will be automatically added to the menu.<br><br>
The steps above, expanded:

  1. Make a GitHub account
  2. Download the GitHub application ([Mac](http://mac.github.com/), [Windows](http://windows.github.com/))
  3. If it's the first time you use it, open it and input your GitHub login details
  4. Go to [this documentation repository](https://github.com/primo-io/prototype-documentation)
  5. Click on the "Fork" button in the top right corner, to fork this repository into your account.
  6. Go to your giHub account, open the forked repository page and click on the "Clone in Desktop" button, on the right-hand sidebar. It will automatically open the GitHub application, asking where to save the local repository.
  7. After selecting a folder path in your computer, click on "clone"
  8. After downloading the files, navigate to your local folder where the repository has been downloaded.
  9. Open the 'languages' folder, where all the translations are located. Select the starting language ("english.md" for example), then copy the file and rename it to your destination language ("spanish.md" for example), in the same folder.
  10. Open the newly created file, change the page header values 'title' (title in your language) and 'language' (the destination language with Capital letter), then translate it to your language, keeping the markdown formatting
  11. After the translation is completed and saved, it's time to re-upload it on GitHub. Open the GitHub application and double click on the repository. On the left sidebar, click on the "Changes" tab. It should say "Uncommitted Changes".
  12. Give a title to your edits, like "spanish translation", then click on "commit" and then on the "sync" button.
  13. Go to your GitHub profile, on the forked repository page. You should be able to see your newly created page in the 'languages' folder. On the top, there should be a green button with two arrows, click on it to issue a pull request. (see picture below)
  ![photo]({{ site.baseurl }}images/screenshots/pull-1.jpg)

  14. Then click on "Create Pull Request"

  ![photo]({{ site.baseurl }}images/screenshots/pull-2.jpg)

  15. Write a message for the pull request and that's it! Now we just have to approve the request.
</div>
<br>

## 1. Što je Primo?
![primo play set]({{ site.baseurl }}images/photo/primo.jpg)

Primo je opipljivo sučelje, dizajnirano s ciljem približavanja i upoznavanja mlađe djece (od 3 do 7 godina starosti) s logikom programiranja, bez potrebe za pismenošću. Cilj igre je navesti malog robota, koji se zove Cubetto, do njegove kuće. Da bi se ostvario cilj, djeca moraju programirati kretanje robota koristeći ograničen skup naredbi: "naprijed", "lijevo", "desno" i "funkcija". Dočim su prve tri naredbe prilično intuitivne, naredba "funkcija" poziva potprogram (podrutinu) - dodatnu liniju naredbi povezane u jednu naredbu.

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/82620072" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">        
    </iframe>
</div>

## 2. Istraživanje

Podučavanje djece programiranju je naširoko raspravljana tema. Poznat nam je umjeren broj rješenja koja pokušavaju ostvariti cilj za djecu iznad 8 godina starosti. Međutim, ne postoje brojna rješenja koja su pogodna za mlađu djecu, a uopće ne postoje ona koja ne zahtijevaju ekran ili potrebu za pismenošću. Zamjećujemo sve veći broj programa za tablete i računala koji također rade u kombinaciji sa stvarnim robotima, ali niti jedan od njih nije potpuno oslobođen pikselastog okružja kao što je to slučaj s Primo Play setom.

Kao glavni materijal odabrali smo drvo, prije svega zato što je prirodno; drvo puža ugodan osjećaj i proizvodi privlačan zvuk. Drugi razlog je kulturološki. Promatranjem igranja, obavljenih u tradicionalnim vrtićima u Švicarskoj gdje je Primo izvorno dizajniran, zamijećeno je da su djeca više voljela igračke od drveta. Drvene igračke su otporne i dugotrajne te se na njima mogu vidjeti oznake i ogrebotine, znamenje prethodnog igranja s drugom djecom. Drvo je materijal koji pamti. Osim toga, drvo je izabrano kao materijal i zato što predstavlja potpunu suprotnost modernoj tehnologiji. Unutar Prima nalazi se elektronika, ali mi smo željeli stvoriti "magično" iskustvo, skrivajući izvornu kompleksnost same igračke.

<img class="float" src="{{ site.baseurl }}images/photo/logo-turtle.jpg">

Značajna inspiracija za Primo je rad Seymoura Paperta, matematičara i suosnivača s Marvinom Minskyjem, u šezdesetima, Laboratorija za umjetnu inteligenciju na MIT (ako vas zanima područje, preporučamo vam da pročitate njegovu najslavniju knjigu - [Mindstorms](http://www.amazon.co.uk/Mindstorms-Children-Computers-Powerful-Ideas/dp/0465046746/ref=sr_1_1?ie=UTF8&qid=1393675158&sr=8-1&keywords=mindstorms+papert).
On je upravljao timom koji je izmislio programski jezik [LOGO](http://en.wikipedia.org/wiki/Logo_(programming_language), vjerojatno najkorišteniji izvor za podučavanje djece programiranju (možda u svijetu, ali ne i u HR, op.pr.)  Njegov cilj nije bio samo podučiti programiranje, nego također pomoći djeci da razviju svoj osobni način rješavanja problema. Primo može biti smatran ektremnim pojednostavljenjem programskog jezika LOGO. Ograničili smo instrukcije na njihovu suštinu, izbjegavajući pritom bilo kakav tekstualni ili brojčani jezik.

Prvi prototip je stvorio Matteo Loglio (Primo.io suosnivač i dizajner sučelja) u SUPSI Lugano za vrijeme [MAInD - Master of Advanced Studies in Interaction Design](http://www.maind.supsi.ch/). Matteovo obrazovanje je iz područja dizajna proizvoda i nakon što je naučio osnove Arduino platforme i dovoljno programiranja da stvori prototip, počeo je tražiti rješenja koja su dostupna početnicima kako bi razvili aplikaciju kao što je Primo. Postojala su dva glavna problema: napraviti auto-robota od nule i upravljačko sučelje u kojem će biti jednostavno razabrati različite naredbe.

Prvi problem je rješen koristeći [Oh_Oh ploču](http://david.cuartielles.com/w/Maquila2/Ohoh) Davida Cuartiellesa, jednog od Arduinovih osnivača koji je držao predavanje na SUPSIu. Oh_Oh robot je otvoreni projekt, možete naći izvorni kod u prethodnom linku. U suštini, to je Arduino u obliku auta s dodatkom XBee ploče za radio komunikaciju.

Drugi problem je bio dizajniranje pouzdanog načina raspoznavanja naredbi. Rješenje je inspirirano [CIID](http://ciid.dk/) pojektom zvanim ["Barcode Piano"](http://ciid.dk/education/portfolio/idp11/courses/physical-computing/projects/barcode-piano/).

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/19704918" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">    
    </iframe>
</div>

Ideja je koristiti raznovrsne blokove umjesto naredbi. Procesor može razaznati blokove pomoću otpornika. U svojoj osnovi, sustav je djelitelj napona te analogni ulazi Arduino ploče mogu očitati vrijednosti otpornika. Metoda je vrlo jednostavna, ali i vrlo prikladna za prototip.

U pogledu dizajna, neke pojedinosti su zahtijevale testiranje; trenutni dizajn je rezultat nekoliko iteracija.

Zmijoliki ili "zig-zag" slijed naredbi je odabran da bi se izbjegle predrasude izvedene iz pismenosti.

![left to right]({{ site.baseurl }}images/illustrations/left-to-right.jpg)

"D" oblik naredbi je dizajniran tako da naredbe mogu biti umetnute na samo jedan način, dosljedan s nizom naredbi i smjerom kretanja auta. Postoje višestruki načini kako se to moglo izvesti. D oblik je izabran zato što je to u svojoj osnovi usmjereni krug.

![instruction blocks]({{ site.baseurl }}images/photo/instruction-blocks.jpg)

Dizajn oblika naredbi još se uvijek testira. Trenutni dizajn je prilično zadovoljavajući te djeca s lakoćom shvaćaju njihovo značenje. U početku postoje manje poteškoće u prepoznavanju naredbi "lijevo" i "desno". To je posljedica i činjenice da su koncepti "lijevo" i "desno" općenito novost za njih. Trenutno testiramo drugačije dizajne kako bi i taj aspekt unaprijedili.

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/50570097" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">

    </iframe>
</div>

U početku, robot je bio auto igračka te je njegova izrada bila vrlo komplicirana i vremenski zahtijevna jer je laserski izrezane komade trebalo zalijepiti sloj po sloj i nakon toga preko sat vremena brusiti. Auto je imao još jednu manu. Bio je izrazio dječački orjentiran. Željeli smo ostati neutralni i stvoriti igračku koja nije specifično igračka za dječake ili za djevojčice te smo se odlučili za vrlo neutalan geometrijski oblik - kvadar (kutiju).

Maloj kutiji smo zatim dali ime, zajedno s osobnošću i nasmješenim lice, čineći ju tako još privlačnijom za djecu. Mali robot nazvan je Cubetto (talijanska riječ za malu kocku). Ideja s Cubettom je također napraviti osnovni modul koji može lagano biti proširen i nadograđen u budućnosti.

![cubetto]({{ site.baseurl }}images/photo/cubetto.jpg)

## 3. Početak

### 3.1 Osnove

Primo se sastoji od tri dijela: upavljačke ploče, Cubetta i skupa naredbi. Djeca upravljaju Cubettom stavljajući blokove (naredbe) u rupe na upravljačkoj ploči, stvarajući pritom niz naredbi (program) koji zatim Cubetto izvrši.

Postoje četri vrste blokova, što znači da trebamo koristiti otpornike s četri različite vrijednosti, po mogućnosti poprilično različite jedne od drugih.

Blokovi se umeću u rupe na upravljačkoj ploči, gdje se razluči vrijednost otpornika. Nakon toga, vrijednosti se obrade u tekst koji se pošalje Cubettu koristeći dva XBee bežična modula te Cubetto izvrši niz naredbi, jednu po jednu.

Mozak prototipa su dvije Arduino ploče; UNO (mogu poslužiti i Leonardo ili Duemilanove) za Cubetto i Mega za upravljačku ploču, gdje nam treba 16 analognih ulaza.

### 3.2 Elektronika

### Potreban alat

* lemilica
* žica za lemljenje (tinol)
* vodiči
* pištolj za ljepilo (vruće)
* ljepilo za drvo
* bakrena traka široka 5mm

### Materijal (cijene u eurima)

Cubetto ~ 88 €

* Arduino UNO (ili Leonardo) - 20 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=195#.UxC5nfTV_bA)
* Arduino Proto Wireless Shield - 14.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* SN754410 Motor Driver - 3.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_33&products_id=153#.UxC5-_TV_bB)
* XBee (serija 1 ili 2, ne čini nikakvu razliku) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* SolarBotics kotači x 2 : 4.74 € - [Solarbotics Store](https://solarbotics.com/product/gmpw/)
* SolarBotics Gear Motors GM3 x 2 : 8.36 € - [Solarbotics Store](https://solarbotics.com/product/gm3/)
* 2 Ball Casters : 5.79 € - [Solarbotics Store](https://solarbotics.com/product/23160/)
* CNY70 x 2 : 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Vishay/CNY70/?qs=%2fha2pyFaduj8YpDhNNtXszq4w32cl%2fAjUjdOwQUvJUM%3d)
* (optional) držač za baterije : 4 € - [Solarbotics Store](https://solarbotics.com/product/bholdaa_4_cell/)
* (optional) 4 x punjive baterije

Upravljačka ploča ~ 88 € (puka slučajnost)

* Arduino Mega 2560 : 39.00 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=196#.UxC_gPTV_bA)
* Arduino Proto Wireless Shield : 14.90 - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* XBee (series 1 or 2, doesn't make any difference) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* 16 5mm LED (crvene): 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Lite-On/LTL-4223/?Lite-On/LTL-4223/&qs=sGAEpiMZZMusoohG2hS%252b15J8d1kHl%252bvkJpzS4atZNEA=)
* 16 220 Ω otpornika : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 16 10 KΩ otpornika : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 1 kontaktni prekidač : 1 €
* 50 jednorednih muških pin kontaktata  (male headers) : 1 €
* 16 dvorednih muških pin kontakata (double male headers) : 0.50 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=294#.UxC_3fTV_bA)
* 50 jednorednih ženskih pin kontakata (female headers) : 1 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=188#.UxDAAfTV_bA)
* 16 magneta promjera 4mm i visine 3mm : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

Naredbe ~ 4 €

* 4 x 4.7 KΩ otpornika : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-47K-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2fbdyz6pU6a%252bvHlD5kaZWgo%3d)
* 4 x 100 KΩ otpornika : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-100K-RC/?qs=sGAEpiMZZMu61qfTUdNhG81NIhcRRUJQxII5Nsctha8%3d)
* 4 x 220 Ω otpornika : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 4 x 10 KΩ otpornika : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 16 magneta promjera 4mm i visine 3mm : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

### 3.3 Napajanje

Cubetto se napaja pomoću baterija, a upravljačka ploča može, ali i ne mora - već prema izboru. Za prototip možete koristiti LiPo baterije ili obične AA baterije, prema želji. Mi smo koristili obje, LiPo baterije su dobre, ali vam treba dodatna oprema. Ako počinjete "od nule" preporučamo vam AA baterije. Imajte na umu da se baterije potroše prilično brzo, tako da je puno bolje koristiti punjive baterije poput NiMh.

### 3.4 Dizajn prototipa

Cijeli proizvod je napravljen od laserski izezanog drveta (šperploče), uglavnom debljine 4 mm sa samo jednim slojem od 1mm. Laserski možete izrezati ove dijelove koristeći servis kao što je Ponoko, ili u lokanom FabLabu (nažalost u HR još uvijek ne postoji FabLab podružnica, ali postoje komercijalni servisi). Prvi prototip je bio laserski izrezan u [FabLabu Lugano](http://fablab.supsi.ch/), dok je daljnji razvoj nastavljen u [FabLabu Torino](http://fablabtorino.org/), gdje dio razvojnog tima još uvijek boravi.

Pravljenje Cubetta i upravljačke ploče je dugotrajna ali vrlo jednostavna procedura, njihove ljuske su u osnovi kutije. Malo kompliciranije je pravljenje naredbenih blokova. Oni se sastoje od drvenih slojeva od 4mm s magnetima i otpornicima zalemljenim unutra.

## 4. Izgradnja prototipa

### [Download Source Files](files/primo-prototype-laser.zip)

### 4.1 Upravljačka ploča

Za konstrukciju upravljačke ploče prvo je potrebno izrezati drvene dijelove iz dviju datoteka: interface-board-4mm.dxf i interface-board-1mm.dxf: prva je za dijelove od šperploče debljine 4mm, a druga za dijelove od šperploče debljine 1mm.
Kao što se može vidjeti iz priloženih datoteka, dijelovi su označeni brojevima da bi se olakšalo slaganje. Brojevi su spremljeni u različitom sloju (layer) tako da se mogu jednostavno ukloniti prije samog laserskog rezanja. Preporučamo da podesite veličinu rupe za startni gumb, baziran na veličini gumba koji želite koristiti.

Prvo morate zalijepiti zajedno dijelove "3" i "4" pri čemu iskoristite rupe u kutevima da bi pomoću vijaka uskladili ploče te ih ostavite da se zalijepe preko noći.

Zatim uzmite bakrenu traku i izrežite 32 komada od 70mm postavite ih unutar pravokutnih rupa na komadu koji ste upravo zalijepili. Trake trebaju imati najmanje 30mm sa svake strane. Jednom kad ste to završili, možete nastaviti i zalijepiti ostale slojeve koji dolaze iznad (prema skici):

![copper connectors]({{ site.baseurl }}images/illustrations/board-1.jpg)
![copper connectors]({{ site.baseurl }}images/illustrations/board-2.jpg)

Jednostavnije je ako ujedno prvo zalijepite komade "1" i "2" zajedno te ih onda zalijepite s komadima "3" i "4" obrađenim na prethodno opisani način.

![copper connectors]({{ site.baseurl }}images/illustrations/board-esploso.jpg)

Nakon što se ljepilo osušilo, stavite magnete u male, za njih predviđene rupice. Okrenite zaljepljene ploče i jednostavno popunite rupice magnetima pri čemu obratite pozornost da svi magneti imaju istu orijentaciju, nije važno sjever ili jug. Začepite rupice pištoljem za ljepilo.

Potom na red dolazi elektronika. Započnite postavljanjem vodova za fazu (5V) i nulu duž rupa kao na slici. Za prvi prototip nismo koristili bakrenu traku nego obične vodljive žice (koje dakako možete i sami koristiti), ali za ovaj prototip smo također uporabili bakrenu traku i za vodove. Puno je jednostavnije spajati komponente uz znatnu uštedu vremena.

![rails]({{ site.baseurl }}images/illustrations/board-3.jpg)

U sljedećem koraku električki povežite jednu od bakrenih konektora na svakoj rupi sa granom "nula". Ako ste koristili bakrenu traku, najjednostavnije je iskoristiti još mali komad iste trake, dovoljan da dotakne oba kraja.

![rails]({{ site.baseurl }}images/illustrations/board-5.jpg)

Nakon toga spojite drugu stranu svakog konektora sa granom od 5V (faza), ali ovaj put, koristeći otpornik od 10kΩ. Vrlo korisno svojstvo bakrene trake je da izvrsno prihvaća lemljenje. Na slici možete vidjeti korištenu tehniku:

![10k]({{ site.baseurl }}images/photo/diy-docs-1.jpg)

Na kraju ovog dijela trebali biste imati nešto poput ovog:

![10k scheme]({{ site.baseurl }}images/illustrations/board-6.jpg)

Sad je vrijeme da postavite svijetleće diode (LED) - stavite diodu u svaku od 16 rupica. Imajte na umu da diode imaju polaritet i već sad ih prikladno orijentirajte. Koristeći vruće ljepilo zaljepite ih za drvo. Nakon što se ljepilo ohladi spojite katodu (kraći kontakt) sa otpornikom od 220Ω kojeg zatim spojite na nultu granu.

![10k]({{ site.baseurl }}images/photo/diy-docs-6.jpg)

Spojite svaku katodu na nultu granu preko 220Ω otpornika.

![10k scheme]({{ site.baseurl }}images/illustrations/board-7.jpg)

Dulji kontakt diode treba spojiti na Arduinov (Mega) digitalni I/O kontakt (pin). Ovi pinovi su označeni brojevima od 22 do 53. Da bi vam život bio lakši i kasnije bilo jednostavnije pristupiti svakoj diodi, spojite diode u nizu: u prototipu smo počeli sa pinom 30 za završili sa pinom 45 (ukupno 16 dioda). Početna vrijednost nije bitna, samo to da diode slijede jedna drugu.

Jedan od jednstavnijih načina je da se vodiči zaleme na dvoredne muške kontakte. Konektori na Aruino Mega ploči su posloženi u dvoredu te je ovim rješenjem jednostavno spojiti i odspojiti Arduino ploču.

![rack]({{ site.baseurl }}images/photo/diy-docs-4.jpg)

Nakon što završite lemljenje dioda, zalemite i ručno izrađene konektore. Oni moraju biti spojeni na Arduinove analogne pinove da bi mogli očitati vrijednosti otpornika. Kao i pri spajanju dioda, konektori moraju biti povezani u nizu; počevši od kontakta A0 za prvu rupu pa do kontakta A15 za rupu 16. Žice moraju biti spojene na istom mjestu gdje smo prethodno zalemili 10kΩ otpornik (prema ilustraciji):

![analog input board connections]({{ site.baseurl }}images/illustrations/board-8.jpg)

<div class="cf">
<img class="float cf" src="{{ site.baseurl }}images/illustrations/button.jpg">

<p>
Ovdje smo koristili jednoredne kontakte zato što su analogni kontakti na Aruduinu posloženi u jednoj liniji.

</p>

<p>
Na kraju spojite startni prekidač; zalemite dvije žice na suprotne kontakte i nakon toga ih s gornje strane provucite kroz rupe na ploči i pritisnite prekidač do kraja. Zatim okrnite ploču i trebali biste imati dvije žice koje spojite prema shemi: jednu izravno na na 5V, a drugu preko otpornika od 10kΩ na nulu. Nakon toga spojite Arduinov digitalni pin na prekidač. U našem primjeru iskoristili smo pin 50.

</p>
</div>


![photo]({{ site.baseurl }}images/photo/diy-docs-5.jpg)

Sad smo skoro gotovi s upravljačkom pločom, još samo trebate spojiti štit za bežičnu komunikaciju (wireless shield) povrh Arduino Mega ploče te spojiti kontakte za naredbe, diode i prekidač u za to odgovarajuća mjesta na Arduino ploči: 30-45 za diode, A0-A15 za naredbe i 50 za startni prekidač. Iskoristite A0 do A5 kontakte na bežičnom štitu. Ne zaboravite spojiti nulu na GND pin i 5V na 5V pin.

![rack]({{ site.baseurl }}images/photo/diy-docs-3.jpg)

Zatim je potrebno malo podešavanja: nakon što je dio broj 12 obojan, možete ga zalijepiti s dijelom broj 13 na vrhu ploče. Isto vrijedi i za startni "crveni" gumb: nakon što je dio broj 14 obojan, postavite nešto mekano poput kartona povrh ploče broj 2 - oko startnog prekidača. Nakon toga stavite malo vrućeg ljepila povrh prekidača i prije nego se ljepilo ohladi postavite crveni disk (prema slici).

![photo]({{ site.baseurl }}images/illustrations/button-mechanics.jpg)

### Naredbeni blokovi

Ovo je jedan blok, rastavljen u sastavne dijelove:

<img class="float cf" src="{{ site.baseurl }}images/illustrations/instruction-esploso.jpg">

Da biste složili blok, prvo je potrebno izrezati dijelove prema nacrtima u datotekama; postoji jedna za 4mm debelu drvenu ploču (šperploču) i jedna za 1mm debelu (tanku) ploču. Poželjno je ploče izrezati laserskim rezačem. Ukupno se nalaze četiri sloja, označeni brojevima od 1 do 4 i prema priloženim nacrtima može se napraviti 16 naredbi - četiri od svake vrste.

Svaka vrsta naredbi ima svoj određeni otpornik:

NAPRIJED: 4.7 KΩ<br>
LIJEVO: 100 KΩ<br>
DESNO: 220 Ω<br>
FUNKCIJA: 10 KΩ

Slaganje bloka započinje se sljepljivanjem slojeva 3 i 4.

Nakon što se ljepilo osušilo, možete obojati ploču. Na ilustraciji ispod su označeni dijelovi koji se trebaju obojati.

![image]({{ site.baseurl }}images/illustrations/colors.jpg)

Sada odrežite dva komada bakrene trake, svaki dugačak 40mm. Provucite ih kroz rupe u komadima koje ste upravo zalijepili, praveći ovojnicu  oko njih. Ovojnica mora biti poprilično zategnuta.

![photo]({{ site.baseurl }}images/illustrations/instruction-block-guide.jpg)

Nakon toga, stavite magnet u rupu. OPREZ, PROVJERITE DA JE MAGNET PRAVILNO ORIJENTIRAN, tako da se blok privlači u rupu. Ako magnet stavite naopako, naredbeni blokovi će biti izbacivani iz rupa što može biti zabavno, ali nije uporabljivo u našem slučaju.

Učvrstite magnet s kapljicom vrućeg ljepila i prije nego se ljepilo ohladi prislonite otpornik na vrh s "krakovima" oslonjenim na bakrene vrpce. U sljedećem koraku zalemite krajeve otpornika na bakrene vrpce, zatim odrežite višak krakova i zalijepite drveni dio broj 2 povrh otpornika.

Završite blok ljepljenjem posljednjeg sloja, označenog brojem 1 te ponovite proceduru za svaki naredbeni blok :)

### CUBETTO

Elektronika:

Cubetto prototip možete izgraditi oko Arduino Uno ili Leonardo ploče, s proto bežičnim štitom povrh. Razlog za korištenje proto štita je taj što ima i mali razvojni dio, doboljno velik da se na njega učvrsti motor driver te konektori za optičke encodere, motore i napajanje.

Cubetto se mora okretati 90 stupnjeva na lijevo i desno. Nažalost, korištenje vremenskog intervala poput "okreći se nadesno jednu sekundu" je vrlo nepouzdana metoda. Razlog leži skriven u brojnim parametrima o kojima operacija ovisi kao što su vrsta poda, snaga baterije, itd. Način na koji smo to riješili je razaznavanjem okreta kotača korištenjem optičkih encodera u paru sa naljepnicama. Naljepnica je okrugla i zaljepi se na unutrašnju stranu kotača gdje se nalazi CNY70 optički encoder (prema slici)...

![photo]({{ site.baseurl }}images/photo/diy-docs-14.jpg)

Naljepnica je podijeljena u crne i bijele kriške. CNY70 u sebi sadrži infracrvenu diodu koja je stalno upaljena i fototranzistor koji očitava količinu infracrvenog svjetla koja se odbija od naljepnice na kotaču te pada na njega. Budući da se svjetlost različito odbija od bijele i crne površine (bijela odbija skoro svu svjetlost dok crna apsorbira skoro svu svjetlost), varijacija signala koji izlazi iz fototranzistora je povezana s rotacijom kotača.

![photo]({{ site.baseurl }}images/illustrations/cny70-physycs.jpg)

Razvojni dio bežičnog proto štita na kojem se nalaze motor driver i ostali konektori za druge dijelove (zalemljeni na ploču). Za konektore jednostavno koristite muške i ženske pin konektore.


![photo]({{ site.baseurl }}images/illustrations/wireless-shield-connections.jpg)

Za ove konektore smo iskoristili muške i ženske pin konektore.

![photo]({{ site.baseurl }}images/photo/diy-docs-12.jpg)

![photo]({{ site.baseurl }}images/illustrations/wireless-shield-connections-1.jpg)

SN754410 motor driver ima 16 kontakata koji moraju biti spojeni prema slijedećoj shemi:

![photo]({{ site.baseurl }}images/illustrations/motor-driver.jpg)

CNY70 shema kontakata:

<img style="width:50%" src="{{ site.baseurl }}images/illustrations/cny70-wiring.jpg">

Dizajn:

Započnite laserskim rezačem datoteke cubetto.dxf. Svi dijelovi Cubetta su izrezani od 4mm debele šperploče. Slijedite vizualne upute za izgradnju osnove:

![photo]({{ site.baseurl }}images/illustrations/cubetto-guide.jpg)

Nemojte još staviti motore, prvo trebate pričvrstiti kuglice na podnožje (ball casters).

![photo]({{ site.baseurl }}images/illustrations/ball-caster.jpg)

![photo]({{ site.baseurl }}images/photo/diy-docs-9.jpg)

Zatim slijede CNY70 encoderi. Zalemite na žicu dva suprotna pin konektora koji moraju biti spojeni na 5V. Zatim zalemite tri žice na preostale konektore CNY70 encodera s jedne strane te na niz od 3 ženska pin konektora. Oni će kasnije biti spojeni na pinove na proto štitu.

Dva CNY70 encodera moraju biti postavljena na rub donjeg sloja, s LED i fototranzistorom u vodoravnom položaju. Da biste ih pričvrstili možete koristiti vruće ljepilo (ili neko drugo ljepilo).

Pogledajte sliku da biste bolje razumjeli položaj CNY70 encodera...

![photo]({{ site.baseurl }}images/photo/diy-docs-11.jpg)

Isto kao i pri CNY70, zalemite dvije žice na mala kontaktna krilca koja izviruju iz svakog motora. Možete i uplesti dvije žice kako biste ih napravili čvršćima te na kraju zalemite par ženskih pin kontakata, kao na ilustraciji:

Sada isprintajte nacrt s bijelim i crnim kriškama, zalijepite ih na komad kartona (ili laserski izrezanog drveta/šperploče, što god vam se više sviđa) i napravite rupu u sredini budući da će biti umetnuti između motora i kotača. Crno-bijele kriške moraju biti okrenute prema unutrašnjosti Cubetta te udaljenost između crteža i CNY70 encodera mora biti između 1 i 3 milimetra da bi CNY70 encoder radio ispravno.

![photo]({{ site.baseurl }}images/photo/diy-docs-10.jpg)

Sad možete staviti kotače na motore, ukoliko ste koristili Solarbotics kotače, možete ih pričvrstiti priloženim vijkom - ne zatežite vijak prejako.

Zalijepite tri od četiri zida Cubetta, dijelove označene s 5, 7 i 8. Ostavite stražnju stranu sobodnu, za slučaj da želite nešto promijeniti.

Uzmite kućište za baterije i zalemite dva ženska pin kontakta na crnu i crvenu žicu. Kontakti će na štitu biti spojeni na VIN i GND. Vrlo je poželjno ugraditi i prekidač kojim možete isključiti Cubetta.

![photo]({{ site.baseurl }}images/photo/diy-docs-13.jpg)

Sad možete staviti Arduino i proto štit povrh motora, spojite sve konektore i završili ste pravljenje svog Cubetta.
</div>

## Arduino

### [Download Arduino dokumente](https://github.com/primo-io/arduino-sketches/raw/master/primo-prototype-arduino.zip)

Upute su na engleskom u komentarima crteža.
