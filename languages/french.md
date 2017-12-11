---
layout: default
title: Documentation du Prototype Cubetto
language: Français
category: language
---

<br>

<div id="content" markdown="1">
## 0. C'est quoi ce document ?

![primo play set]({{ site.baseurl }}images/photo/maker-guide.jpg)
Ce document rassemble et organise toutes les informations nécessaires pour construire un prototype Primo.
Vous pouvez trouver plus d'informations à propos du projet sur le site web [primo.io](http://primo.io).

<h2>
<a href="#" id="translate-title">
	Comment traduire ce document
</a>
</h2>


<div markdown="1" id="translate">

Si vous voulez traduire cette page dans votre langue, vous avez plusieurs possibilités :

1. **très facile, aucune automatisation** Copiez et collez cette page dans votre éditeur de texte, traduisez-la puis envoyez-la nous par email à l'adresse [play@primo.io](mailto:play@primo.io)

2. **moyen, légère automatisation ** Créez un compte sur [GitHub](http://github.com), ouvrez ensuite le [dépôt de cette page](https://github.com/primo-io/prototype-documentation/blob/gh-pages/index.md) et cliquez sur 'EDIT', dans la barre de menu du haut :
![photo]({{ site.baseurl }}images/screenshots/edit-1.jpg)
Votre page bascule alors dans un éditeur de texte où vous pouvez modifier la source de la page. La page est écrite en [markdown](http://daringfireball.net/projects/markdown/syntax), très facile à comprendre.
![photo]({{ site.baseurl }}images/screenshots/edit-2.jpg)
Vous n'avez pas à modifier ce code mais copiez et collez simplement l'ensemble du texte dans votre éditeur de texte en local et traduisez ensuite la partie textuelle dans votre langue sans modifier les parties entre parenthèses et en HTML. Enregistrez le texte puis envoyez-le nous à l'adresse [play@primo.io](mailto:play@primo.io)

3. **expérimenté, automatisation complète** Ceci est légèrement poussé mais rien de trop compliqué, si vous n'êtes pas familiarisé avec GitHub vous avez là l'occasion d'apprendre quelque chose de nouveau :) <br>
Si vous êtes déjà familiarisé avec git vous devez créer une branche du dépôt, toutes les traductions se trouvant dans le répertoire 'languages'. Pour traduire la page, dupliquez-la simplement à partir d'une langue existante ("english.md" par exemple) dans le même répertoire puis changez le nom du fichier avec la langue finale (spanish.md). Modifiez dans l'en-tête les valeurs 'title' (le titre du document dans votre langue) et 'language' (la langue cible avec une majuscule) et ensuite traduisez le reste du document. Une fois terminé, faites une demande de soumission pour ajouter votre fichier dans le répertoire, il sera automatiquement ajouté au menu.<br><br>
Voici les étapes ci-dessus en détail :

  1. Créez un compte GitHub
  2. Téléchargez l'application GitHub([Mac](http://mac.github.com/), [Windows](http://windows.github.com/))
  3. Si c'est la première fois que vous l'utilisez, ouvrez-la et entrez vos paramètres d'identification
  4. Allez dans [le dépôt de documentation](https://github.com/primo-io/prototype-documentation)
  5. Cliquez sur le bouton "Fork" dans le coin en haut à droite afin de créer une branche de ce dépôt dans votre compte.
  6. Allez sur votre compte GitHub, ouvrez la page de la branche du dépôt et cliquez sur le bouton "Clone in Desktop" situé sur la barre latérale à droite. L'application GitHub va s'ouvrir automatiquement en demandant où enregistrer le dépôt local.
  7. Après avoir sélectionné le chemin du répertoire sur votre ordinateur, cliquez sur "clone".  
  8. Après avoir téléchargé les fichiers, accédez au répertoire local où le dépôt a été téléchargé.
  9. Ouvrez le répertoire 'languages' où se situent toutes les traductions. Sélectionnez la langue de départ ("english.md" par exemple) puis copiez le fichier dans le même répertoire et renommez-le avec votre langue finale ("spanish.md" par exemple).
  10. Ouvrez le fichier nouvellement créé, modifiez dans l'en-tête les valeurs 'title' (le titre du document dans votre langue) et 'language' (la langue finale avec une majuscule) et ensuite traduisez le texte en préservant le formatage markdown.
  11. Quand la traduction est terminée et enregistrée, il est temps de le re-télécharger sur GitHub. Ouvrez l'application GitHub et double-cliquez sur le dépôt. Sur la bare latérale à gauche cliquez sur l'onglet "Changes", la mention "Uncommitted Changes" devrait s'afficher.
  12. Donnez un titre à vos modifications, tel que "spanish translation", puis cliquez sur "commit" et ensuite sur le bouton "sync".
  13. Allez sur votre profile GitHub, sur la page de la branche du dépôt. Vous devriez pouvoir voir votre nouvelle page créée dans le répertoire 'languages'. En haut il devrait y avoir un bouton vert avec deux flèches : cliquez dessus pour effectuer une demande de soumission. (voir l'image ci-dessous)
  ![photo]({{ site.baseurl }}images/screenshots/pull-1.jpg)

  14. Ensuite cliquez sur "Create Pull Request"

  ![photo]({{ site.baseurl }}images/screenshots/pull-2.jpg)

  15. Ecrivez un message pour la demande de soumission et c'est tout ! A présent nous avons juste à approuver la demande.
</div>
<br>

## 1. C'est quoi Primo ?

![primo play set]({{ site.baseurl }}images/photo/primo.jpg)

Primo est une interface concrète conçue pour introduire la logique programmatique à des jeunes enfants (3 à 7 ans) sans avoir besoin de savoir lire ou écrire. Le but du jeu est de ramener un petit robot appelé Cubetto à sa maison. Pour ce faire, l'enfant doit programmer le petit robot en utilisant un jeu limité d'instructions : avant, gauche, droite et fonction. Alors que les trois premières sont relativement intuitives, la dernière fait appel à un sous-programme, une ligne supplémentaire d'instructions regroupées dans une commande unique.

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/82620072" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">        
    </iframe>
</div>

## 2. Recherche

Apprendre la programmation à des enfants est un sujet largement débattu. Nous sommes conscients qu'il existe un certain nombre de solutions qui tentent d'y parvenir pour des enfants à partir de 8 ans. Cependant, il y en a peu qui soient adaptées à des enfants plus jeunes et encore moins qui fonctionnent sans écran ou sans savoir lire ou écrire. Nous voyons un nombre croissant d'applications pour tablettes et ordinateurs qui fonctionnent de pair avec des robots physiques mais aucun n'est véritablement libéré du monde du pixel comme peu l'être l'ensemble de jeu Primo.

Le bois a été choisi comme matériau principal, tout d'abord parce que c'est naturel ; c'est un matériau chaleureux qui a une sonorité agréable. La deuxième raison est culturelle. Des observations ont été menées sur les jeux utilisés dans les crèches traditionnelles en Suisse (où le produit a été conçu à l'origine) pour découvrir que les jeux préférés des enfants étaient tous fabriqués en bois. Les jouets en bois ont une grande durée de vie et on peut voir dessus les marques et les chocs qu'ils ont reçus, signes de leur utilisation antérieure par d'autres enfants. C'est un matériau qui a de la mémoire. Le bois a également été choisi pour le fort contraste qu'il créée avec la technologie. A l'intérieur de Primo il y a un circuit imprimé mais nous voulions créer une expérience "magique" en cachant la complexité du jeu.

<img class="float" src="{{ site.baseurl }}images/photo/logo-turtle.jpg">

Le concept derrière Primo est largement inspiré du travail de Seymour Papert, un mathématitien qui a co-fondé le MIT Artificial Intelligence Laboratory avec Marvin Minsky dans les années 60 (si vous êtes intéressés par le sujet, nous vous conseillons de lire [Mindstorms](http://www.amazon.co.uk/Mindstorms-Children-Computers-Powerful-Ideas/dp/0465046746/ref=sr_1_1?ie=UTF8&qid=1393675158&sr=8-1&keywords=mindstorms+papert), son livre le plus connu). Il a dirigé l'équipe qui a inventé le [LOGO](http://en.wikipedia.org/wiki/Logo_(programming_language)), probablement la ressource la plus utilisée et cela depuis longtemps pour apprendre la programmation aux enfants. L'objectif de Seymour Papert n'était pas seulement d'enseigner un code, mais également d'aider les enfants à découvrir leur propre manière de résoudre les problèmes. Primo peut être considéré comme une simplification extrême du LOGO et de la tortue physique. Nous avons limité les instructions à leur forme la plus pure, évitant toute sorte de langage textuel ou numérique.

Le premier prototype a été réalisé à SUPSI Lugano par Matteo Loglio (co-fondateur de Primo.io et interaction designer) pendant le [MAInD - Master of Advanced Studies in Interaction Design](http://www.maind.supsi.ch/). La formation de Matteo est la conception de produit, et après avoir appris les bases en Arduino et un peu de code pour créer le prototype, il commença a rechercher des solutions techniques qui étaient abordables pour des novices, de façon à développer une application comme Primo. Les principales difficultés étaient au nombre de deux : fabriquer à partir de rien une voiture robot ainsi qu'un panneau de contrôle qui pourrait facilement reconnaitre différentes instructions.

La première difficulté a été résolue en utilisant le [panneau Oh_Oh](http://david.cuartielles.com/w/Maquila2/Ohoh) de David Cuartielles, un des fondateurs de Arduino qui a tenu une conférence à SUPSI. Le robot Oh_Oh est un projet libre, vous pouvez trouver les fichiers sources en suivant le lien ci-dessus. C'est essentiellement une carte Arduino en forme de voiture sur laquelle une carte XBee a été ajoutée pour la communication radio.

La deuxième difficulté était d'imaginer une manière fiable de détecter les blocs. Pour la solution on s'est inspiré d'un projet [CIID](http://ciid.dk/) appelé ["Barcode Piano"](http://ciid.dk/education/portfolio/idp11/courses/physical-computing/projects/barcode-piano/).

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/19704918" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">    
    </iframe>
</div>

L'idée est d'utiliser divers blocs qui peuvent être reconnus par le panneau en utilisant des résistances. C'est un diviseur de tension élémentaire, les entrées analogiques d'un Arduino pouvant lire les valeurs des résistances. C'est une méthode très simple mais assez efficace pour un prototype.

En matière de design, certains aspects ont eu besoin d'être testés ; Le design actuel est le résultat de plusieurs essais.

Le chemin en 'serpent' ou 'zig-zag' des séquences d'instruction a été choisi pour éviter les pré-concepts de lecture et d'écriture.

![left to right]({{ site.baseurl }}images/illustrations/left-to-right.jpg)

La forme en 'D' des connecteurs des blocs a été conçue de telle sorte que les blocs ne puissent être insérés que dans un sens afin d'être cohérents avec le chemin conçu et et la direction de la voiture. Plusieurs formes peuvent être utilisées pour cela, la forme en D a été choisie car c'est en gros un 'cercle orienté' et que sa forme rappelle les punaises des panneaux d'affichage.

![instruction blocks]({{ site.baseurl }}images/photo/instruction-blocks.jpg)

Le design pour la forme des blocs d'instruction est toujours en cours de test. Le design actuel fonctionne plutôt bien, les enfants comprennent facilement leur signification, ils ont juste quelques difficultés au début pour se familiariser avec les blocs droite et gauche. Cela est également dû au fait que les concepts "droite" et "gauche" sont généralement assez nouveaux pour eux. Nous sommes actuellement en train de tester d'autres designs de bloc pour améliorer davantage ce point.

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/50570097" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true"  allowfullscreen="true">

    </iframe>
</div>

A l'origine le robot était une voiture jouet. Une forme très compliquée et chronophage à produire car il s'agissait de multiples couches coupées au laser et collées entre elles puis poncées pendant des heures. La voiture avait un autre grand défaut, c'était très orienté garçon. Nous souhaitions éviter d'entrer dans le débat au sujet des fabricants de jouets critiqués pour leur production orientée garçon. Nous voulions rester neutres, sans créer un jouet spécialement pour garçon ou fille, et avons donc  opté pour une forme géométrique très neutre, une boite.

Un nom a été donné à cette petite boite, ainsi qu'une personnalité et une visage souriant, la rendant plus attrayante pour les enfants. Le robot s'appelle Cubetto (petit cube en italien). L'idée avec Cubetto est aussi de créer un module basique pouvant être développé et personnalisé facilement par la suite.

![cubetto]({{ site.baseurl }}images/photo/cubetto.jpg)

## 3. Pour commencer

### 3.1 Les bases

Primo est composé de trois parties : un panneau de contrôle, Cubetto et un jeu de blocs d'instruction. Les enfants interagissent avec le panneau de contrôle en plaçant des blocs d'instruction dans les trous pour créer une séquence (un programme) que Cubetto exécute.

Il y a quatre types d'instruction, ce qui signifie que 4 résistances de différentes valeurs peuvent être utilisées, potentiellement assez éloignées les unes des autres.

Les blocs sont insérés dans les trous du panneau de contrôle où la valeur de la résistance est identifiée. Ensuite les valeurs sont transformées en une chaine de caractère qui est envoyée à Cubetto en utilisant deux modules XBee. Cubetto exécute alors les instructions l'une après l'autre.

Le cerveau du prototype est composé de deux circuits Arduino, un Uno (un Leonardo ou un Duemilanove fera aussi l'affaire) pour Cubetto et un Mega pour le panneau de contrôle où 16 entrées analogiques sont nécessaires.

### 3.2 Electronique

### Les outils nécessaires

* Fer à souder
* Soudure
* Fils électriques
* Pistolet à colle
* Colle à bois
* Ruban en cuivre de 5mm de large

### Matériel (prix en euro, hors taxe)

Cubetto ~ 88 €

* Arduino UNO (ou Leonardo) - 20 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=195#.UxC5nfTV_bA)
* Arduino Proto Wireless Shield - 14.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* Circuit de commande moteur SN754410 - 3.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_33&products_id=153#.UxC5-_TV_bB)
* XBee (série 1 ou 2, ça ne fait aucune différence) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* Roues SolarBotics x 2 : 4.74 € - [Solarbotics Store](https://solarbotics.com/product/gmpw/)
* Moteur réducteur GM3 SolarBotics x 2 : 8.36 € - [Solarbotics Store](https://solarbotics.com/product/gm3/)
* 2 Roulettes à bille : 5.79 € - [Solarbotics Store](https://solarbotics.com/product/23160/)
* Capteur optique CNY70 x 2 : 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Vishay/CNY70/?qs=%2fha2pyFaduj8YpDhNNtXszq4w32cl%2fAjUjdOwQUvJUM%3d)
* (facultatif) Support de pile : 4 € - [Solarbotics Store](https://solarbotics.com/product/bholdaa_4_cell/)
* (facultatif) 4 x piles rechargeables

Panneau de contrôle ~ 88 € (pure coincidence)

* Arduino Mega 2560 : 39.00 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=196#.UxC_gPTV_bA)
* Arduino Proto Wireless Shield : 14.90 - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* XBee (série 1 ou 2, ça ne fait aucune différence) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* 16 LED rouge 5 mm : 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Lite-On/LTL-4223/?Lite-On/LTL-4223/&qs=sGAEpiMZZMusoohG2hS%252b15J8d1kHl%252bvkJpzS4atZNEA=)
* 16 Résistances 220 Ω : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 16 Résistances 10 KΩ : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 1 Bouton poussoir : 1 €
* 50 Têtes mâles : 1 €
* 16 Têtes doubles mâles : 0.50 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=294#.UxC_3fTV_bA)
* 50 Têtes femelles : 1 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=188#.UxDAAfTV_bA)
* 16 Aimants ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

Blocs d'instruction ~ 4 €

* Résistance 4 x 4.7 KΩ : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-47K-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2fbdyz6pU6a%252bvHlD5kaZWgo%3d)
* Résistance 4 x 100 KΩ : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-100K-RC/?qs=sGAEpiMZZMu61qfTUdNhG81NIhcRRUJQxII5Nsctha8%3d)
* Résistance 4 x 220 Ω : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* Résistance 4 x 10 KΩ : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 16 Aimants ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

### 3.3 Energie

Cubetto et (éventuellement) le panneau de contrôle sont alimentés par des piles. Pour le prototype vous pouvez utiliser une batterie Li-Po ou des piles AA courantes, c'est comme vous le souhaitez. Nous avons utilisé les deux, les batteries Li-Po sont bien mais nécessitent un équipement supplémentaire, si vous démarrez à partir de rien nous vous conseillons les piles AA. Gardez simplement à l'esprit qu'elles se déchargent assez vite donc le mieux serait d'utiliser des piles rechargeables telles que les piles NiMH.

### 3.4 Design du prototype

Le produit est entière constitué de bois découpé au laser, principalement de 4 mm d'épaisseur, avec seulement une couche de 1 mm d'épaisseur. Vous pouvez effectuer la découpe au laser en utilisant des services tels que Ponoko ou dans votre FabLab local. Le premier prototype a été découpé au laser au [FabLab Lugano](http://fablab.supsi.ch/) alors que le développement du produit s'est déroulé au [FabLab Torino](http://fablabtorino.org/) où une partie de l'équipe de développement de Primo réside toujours.

Construire Cubetto et le panneau de contrôle est un travail laborieux mais très simple, leur coque étant globalement des boites. La vrai difficulté réside dans les blocs d'instruction : il s'agit de deux couches en bois de 4 mm avec un aimant et une résistance soudés à l'intérieur.

## 4. Fabrication du prototype

### [Télécharger les fichiers source](files/primo-prototype-laser.zip)

### 4.1 Le Panneau de contrôle

Pour fabriquer le panneau de contrôle vous devez effectuer la découpe au laser de deux fichiers : interface-board-4mm.dxf et interface-board-1mm.dxf. Le premier est pour le contreplaqué de 4 mm et le deuxième pour le contreplaqué de 1 mm. Comme vous pouvez le voir dans les fichiers, les parties sont numérotées pour faciliter l'assemblage. Les numéros sont conservés sur une autre couche, de cette façon vous pouvez les effacer avant la découpe. Nous vous recommandons d'ajuster le trou du bouton poussoir en fonction de la taille du bouton que vous souhaiter utiliser ou obtenir.

Tout d'abord vous devez coller les parties 3 et 4 ensemble : utilisez les trous dans les coins pour les aligner à l'aide de vis pendant que vous encollez et laissez reposer une nuit.

Ensuite prenez le ruban de cuivre, coupez 32 morceaux de 70 mm chacun et insérez les dans les trous rectangulaires de la partie que vous venez de coller. Ils doivent dépasser d'au moins 30 mm de chaque côté. Une fois terminé vous pouvez coller les parties supérieures restantes du panneau. Voici l'ordre correct :

Prenez le ruban de cuivre, coupez 32 morceaux de 70 mm chacun et insérez les dans les trous rectangulaires de la partie que vous venez de coller. Ils doivent dépasser d'au moins 30 mm de chaque côté.

![copper connectors]({{ site.baseurl }}images/illustrations/board-1.jpg)
![copper connectors]({{ site.baseurl }}images/illustrations/board-2.jpg)

Une fois terminé, vous pouvez coller les parties précédemment collées, 1+2 avec 3+4.

![copper connectors]({{ site.baseurl }}images/illustrations/board-esploso.jpg)

Une fois que la colle a séché, posez les aimants dans les petits trous. Retournez votre planche supérieure et remplissez chaque trou avec un aimant en s'assurant qu'ils sont tous dans le même sens, qu'importe que ce soit le nord ou le sud. Bouchez le trou avec une goutte de colle.

Passons à l'électronique. Commencez par faire un rail pour le 5V et un rail pour la masse le long des lignes de trous comme sur le schéma. Le tout premier prototype n'avait pas de bande de cuivre mais des fils (que vous pouvez aussi utiliser) alors que dans ce prototype nous avons utilisé du ruban de cuivre pour les rails : un vrai gain de temps et cela facilite les connexions.

![rails]({{ site.baseurl }}images/illustrations/board-3.jpg)

L'étape suivante consiste à relier l'un des deux connecteurs de chaque trou au rail de la masse. Si vous avez utilisé du ruban de cuivre vous pouvez utiliser pour cela juste un petit bout supplémentaire, assez pour toucher les deux extrémités.

![rails]({{ site.baseurl }}images/illustrations/board-5.jpg)

A présent nous devons connecter l'autre partie de chaque connecteur au rail de 5V mais cette fois avec une résistance de 10 KΩ entre les deux. Un truc bien avec le ruban de cuivre c'est que la soudure fond très bien dessus, c'est donc la technique que nous avons utilisée :

![10k]({{ site.baseurl }}images/photo/diy-docs-1.jpg)

A l'issue de cette étape vous devriez obtenir quelque chose comme ça :

![10k scheme]({{ site.baseurl }}images/illustrations/board-6.jpg)

Maintenant il est temps de mettre les LEDs ; Placez une LED rouge dans chacun des 16 trous, ensuite utilisez une goutte de colle chaude pour les sceller au bois. Une fois la colle refroidie nous devons les connecter. Souvenez-vous que les LEDs sont polarisées : la tige longue est l'anode et la courte la cathode. Connectez chaque cathode au rail de la masse en utilisant une résistance de 220 Ω.

![10k]({{ site.baseurl }}images/photo/diy-docs-6.jpg)

Connectez chaque cathode au rail de la masse en utilisant une résistance de 220 Ω.

![10k scheme]({{ site.baseurl }}images/illustrations/board-7.jpg)

La tige longue des LEDs doit être connectée à une broche I/O numérique de l'Arduino Mega, ces broches sont numérotées de 22 à 53. Les LEDs doivent être connectées dans l'ordre, de cette manière ce sera plus facile d'y accéder plus tard dans le code ; Dans mon prototype par exemple je suis parti de la broche 30 jusqu'à la 45 (il y a 16 LEDs).
Le point de départ n'a pas d'importance tant qu'elles sont dans le bon ordre séquentiel. Cela signifie par exemple que si nous partons de la broche 30, la première LED doit être attachée à la broche 30, la deuxième à la 31, la troisième à la 32 et ainsi de suite jusqu'à la LED 16 à la broche 45.

Les câbles sont soudés à une rangée de têtes mâles doubles, puisque les broches numériques sur l'Arduino Mega sont implantées en double ligne. De cette façon il est facile de brancher et débrancher l'Arduino du panneau.

![rack]({{ site.baseurl }}images/photo/diy-docs-4.jpg)

Une fois que toutes les LEDs sont soudées nous devons souder nos connecteurs faits-main. Ceux-ci doivent être câblés aux broches analogiques de l'Arduino Mega afin de lire les différentes valeurs des résistances. De la même manière que les LEDs ils doivent être connectés dans l'ordre, en partant de la A0 pour le trou 1 à la A15 pour le trou 16. Le fil doit démarrer du même point où nous avons soudé précédemment la résistance de 10 KΩ. Voir l'illustration :

![analog input board connections]({{ site.baseurl }}images/illustrations/board-8.jpg)

<div class="cf">
<img class="float cf" src="{{ site.baseurl }}images/illustrations/button.jpg">

<p>
Ici j'ai utilisé des têtes mâles simples puisque les broches analogiques sont toutes sur une seule ligne.
</p>

<p>
La dernière chose à connecter est le bouton : prenez-le et soudez deux câbles sur deux têtes opposées, ensuite glissez-les au travers du trou du bouton, à partir du haut, et tirez jusqu'au bout. A présent retournez le panneau, vous devriez avoir les deux fils qui sortent du trou. Faites les connexions comme sur l'illustration : la première avec un des fils directement au 5V, l'autre en utilisant une résistance de 10 KΩ pour connecter le bouton à la masse. Connectez également le fil qui part du bouton avec la résistance à une broche numérique de l'Arduino, dans cet exemple nous avons utilisé la broche numéro 50.
</p>
</div>


![photo]({{ site.baseurl }}images/photo/diy-docs-5.jpg)

C'est presque fini avec le panneau. Maintenant vous avez simplement à brancher le Wireless Shield au dessus de l'Arduino Mega et à placer les têtes sur le circuit. Pour résumer : 30 à 45 pour les LEDs, A0 à A15 pour les connecteurs et 50 pour le bouton. Utilisez les broches de A0 à A5 du Wireless Shield pour les 5 premiers connecteurs. N'oubliez pas de connecter le rail de la masse à la broche GND et celui de 5V à la broche 5V.

![rack]({{ site.baseurl }}images/photo/diy-docs-3.jpg)

Maintenant un petit peu de mise au point : après que la partie 12 du plateau ait été peinte, vous pouvez la coller avec la partie 13 sur le dessus du plateau

Idem pour le bouton rouge : une fois la partie 14 peinte, mettez quelque chose de mou comme du carton sur la partie 2 autour du bouton rouge, puis appliquez un peu de colle chaude sur le bouton poussoir et placez le bouton rouge avant qu'elle n'ait séché. Voir l'illustration :

![photo]({{ site.baseurl }}images/illustrations/button-mechanics.jpg)

### LES BLOCS D'INSTRUCTION

Voici un bloc d'instruction, en vue éclatée:

<img class="float cf" src="{{ site.baseurl }}images/illustrations/instruction-esploso.jpg">

Pour fabriquer les blocs d'instruction, la première chose à faire est de découper au laser les fichiers, il y en a un pour le bois de 4 mm d'épaisseur et un pour le 1 mm. Il y a 4 couches, numérotées de 1 à 4 et les schémas fournis peuvent être utilisés pour fabriquer 16 blocs, 4 de chaque sorte.

Chaque bloc a une résistance différente. Voici les résistances utilisées pour le prototype :

AVANT : 4.7 KΩ<br>
GAUCHE : 100 KΩ<br>
DROITE : 220 Ω<br>
FONCTION : 10 KΩ

Pour fabriquer les blocs, tout d'abord vous devez coller la partie 4 avec la partie 3.

Une fois que la colle a séché vous pouvez démarrer la peinture. Voir l'illustration ci-dessous pour repérer quelle partie doit être colorée :

![image]({{ site.baseurl }}images/illustrations/colors.jpg)

A présent vous devez couper deux morceaux de ruban de cuivre de 40 mm  de long. Glissez les dans les trous des deux blocs que vous venez de coller, en faisant un anneau autour des fissures du haut et du bas. L'anneau doit être bien serré.

![photo]({{ site.baseurl }}images/illustrations/instruction-block-guide.jpg)

Après cela, vous devez poser l'aimant dans le trou. Ce faisant, VERIFIEZ BIEN QU'IL EST CORRECTEMENT ORIENTÉ, afin que le bloc s'aimante dans le trou. Si vous le mettez dans le mauvais sens il sera repoussé par l'autre aimant, plutôt amusant comme résultat mais ce n'est pas ce que nous souhaitons obtenir.

Fixez l'aimant avec une goutte de colle chaude et avant qu'elle ne refroidisse placez la bonne résistance dessus, avec les pieds couchés sur le ruban de cuivre. Ensuite, la résistance doit être soudée sur les deux morceaux. Après la soudure, coupez ce qui dépasse des pieds et collez la partie 2 par dessus la résistance.

Terminez votre bloc en collant la dernière couche, partie numéro 1, sur le dessus, puis répétez la procédure complète pour chaque bloc :)

### CUBETTO

Electronique:

Le prototype de Cubetto peut être fabriqué en utilisant un Arduino Uno ou Leonardo, avec un Proto Wireless Shield sur le dessus. La raison de ce Proto Shield est qu'il dispose d'une petite zone de prototypage assez grande pour y placer le pilote du moteur, les connecteurs pour les encodeurs optiques, les moteurs et l'alimentation.

Cubetto doit tourner à 90 degrés à gauche et à droite. Une très mauvaise manière de faire serait d'utiliser un évènement temporel, tel que "tourne à droite pendant une seconde", vous pourriez vous attendre à plus ou moins le même résultat si vous le jouez plusieurs fois. "Plus ou moins" car cela dépend de plusieurs facteurs, tels que la nature du sol, le niveau de charge des batteries, etc. J'ai résolu le problème en détectant le nombre de rotations de la roue en utilisant deux encodeurs optiques CNY70 en combinaison avec un autocollant. Le disque autocollant se place à l'intérieur de la roue, ce qui donne quelque chose comme ça :

![photo]({{ site.baseurl }}images/photo/diy-docs-14.jpg)

L'autocollant est divisé en tranches noires et blanches car le CNY70 est capable de détecter la variation entre une tranche noire et blanche. Pour faire simple à l'intérieur il y a une LED infrarouge qui est toujours allumée et un phototransistor qui lit la quantité de lumière infrarouge réfléchie. Quand un matériau noir est placé devant le composant, pratiquement aucune lumière n'est réfléchie puisque la couleur noire a tendance à l'absorber. A l'inverse, si le matériau est blanc, il réfléchit toute la lumière et donc la valeur lue par le capteur est très élevée. La différence entre les lectures est utilisée pour compter les pas de rotation.

![photo]({{ site.baseurl }}images/illustrations/cny70-physycs.jpg)

La zone de prototypage du Wireless Proto Shield est l'endroit où le pilote du moteur et d'autres connecteurs pour les autres parties sont soudées. Pour cela, utilisez simplement des têtes mâles comme connecteurs et des têtes femelles d'autre part.

![photo]({{ site.baseurl }}images/illustrations/wireless-shield-connections.jpg)

Pour cela, j'ai simplement utilisé des têtes mâles comme connecteurs et des têtes femelles d'autre part.

![photo]({{ site.baseurl }}images/photo/diy-docs-12.jpg)

![photo]({{ site.baseurl }}images/illustrations/wireless-shield-connections-1.jpg)

Le pilote de moteur SN754410 possède 16 broches qui doivent être connectées selon le schéma suivant :

![photo]({{ site.baseurl }}images/illustrations/motor-driver.jpg)

Le schéma du CNY70 :

<img style="width:50%" src="{{ site.baseurl }}images/illustrations/cny70-wiring.jpg">

Design:

Commencez par la découpe laser de cubetto.dxf. Toutes les parties de Cubetto sont découpées dans du contreplaqué de 4 mm. Suivez ces instructions visuelles pour construire la base :

![photo]({{ site.baseurl }}images/illustrations/cubetto-guide.jpg)

Ne montez pas les moteurs pour le moment, d'abord vous devez monter les roulettes à bille.

![photo]({{ site.baseurl }}images/illustrations/ball-caster.jpg)

![photo]({{ site.baseurl }}images/photo/diy-docs-9.jpg)

Maintenant le CNY70. Soudez  ensemble avec un fil les deux têtes opposées, qui doivent être connectées au 5V ; Ensuite soudez trois fils aux têtes restantes du CNY70. Au bout de ces films soudez une rangée de trois têtes femelles. Ils seront plus tard connectés aux têtes du Proto Shield.

Les deux CNY70 doivent être placés sur le bord de la couche du dessous, avec la LED et le phototransistor alignés horizontallement. Pour les fixer vous pouvez utiliser de la colle chaude (ou une autre colle).

Voir le dessin pour comprendre la localisation.

![photo]({{ site.baseurl }}images/photo/diy-docs-11.jpg)

De la même manière que pour le CNY70, soudez deux fils aux petits rabats qui sortent de chaque moteur. Vous pouvez enrouler les deux fils ensemble pour les rendre plus résistants, puis soudez au bout une rangée de deux têtes femelles, comme sur l'illustration.

Maintenant imprimez le dessin intérieur avec les tranches noires et blanches, collez-les sur un morceau de carton (ou coupez au laser du bois, c'est comme vous voulez), coupez autour et faites un trou au centre, pour être insérés entre le moteur et la roue. Les tranches noires et blanches doivent être orientés vers l'intérieur de Cubetto et la distance entre le dessin et le CNY70 doit être compris entre 1 et 3 mm pour que le CNY70 puisse fonctionner convenablement.

![photo]({{ site.baseurl }}images/photo/diy-docs-10.jpg)

A présent vous pouvez installer les roues et les moteurs. Si vous utilisez les roues Solarbotics, vous pouvez les attacher avec le tournevis fourni. Ne les serrez pas trop.

Collez trois des quatre côtés de Cubetto, partie 5, 7 et 8. Nous allons laisser l'arrière amovible, juste au cas où nous voudrions modifier quelque chose plus tard.

Prenez le support à pile et soudez les cables rouge et noir à 2 autres connecteurs femelles.

![photo]({{ site.baseurl }}images/photo/diy-docs-13.jpg)

Maintenant vous pouvez placer l'Arduino + Proto Shield par dessus les moteurs, branchez les têtes sur le shield et vous avez terminé de construire Cubetto.
</div>

## Arduino

### [Téléchargez les fichiers Arduino](https://github.com/primo-io/arduino-sketches/raw/master/primo-prototype-arduino.zip)

Les instructions sont dans les commentaires du croquis.
