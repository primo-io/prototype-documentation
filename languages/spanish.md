---
layout: default
title: Documentación Prototipo de Cubetto
---

<div id="edit"> <a href="http://github.com/primo-io/prototype-documentation/blob/gh-pages/index.md">Editar este documento</a></div>

## 0. Que hay en este documento

![primo play set](images/photo/maker-guide.jpg)
Este documento acopia y organiza toda la información necesaria para construir un prototipo de primo
Puedes encontrar información adicional acerca del proyecto en el sitio [primo.io](http://primo.io) (En inglés)

## IMPORTANTE
La documentación e instrucciones incluidas en este documento le permitirá producir un prototipo de primo como el mostrado en este video, el cual es diferente al de producción final. Sin embargo, liberaremos también la documentación necesaria para actualizaciones y nuevas versiones del set Primo, incluyendo archivos para el producto final, así como y cuando nosotros los hemos ensayado y probado.

## MAS IMPORTANTE
La licencia bajo la cual liberamos el set Primo le da la libertad de construir su propio prototipo. Sin embargo **No esta usted autorizado para venderlo como Primo**, bajo ninguna circunstancia. También, si usted hace un producto derivado del nuestro, debe usted citar el proyecto original (tal como nosotros hacemos con todas nuestras fuentes), además de usar la misma licencia: [CC by-nc-sa 4.0 International](http://creativecommons.org/licenses/by-nc-sa/4.0/). <br>
Esta política no se justifica solo por proteger la propiedad intelectual, sino también para mantener el rastro del flujo de ideas. Como nosotros gastamos un montón de tiempo y recursos para mantener esta documentación libre y accesible, nosotros también lo animamos a "dar algo a cambio" y publicar sus derivados, resultados, sugerencias, insultos y elogios. Estaremos mas que felices en escuchar y responder sus feedbacks y de poner en el blog nuestro las cosas interesantes.

### Como traducir este documento

Si usted desea traducir este documento a su idioma, usted tiene múltiples opciones:

1. (Super fácil, ninguna automatización) La manera más fácil es copiar y pegar este página en su editor de texto, traducirla y luego enviarnos por email a la dirección: [play@primo.io](mailto:play@primo.io)

2. (medium, automatización ligera) Otra manera muy fácil es crear una cuenta en [GitHub](http://github.com), luego abrir el [repositorio en ésta página](https://github.com/primo-io/prototype-documentation/blob/gh-pages/index.md) dar click en 'EDIT', en la barra del menú superior:
![photo](images/screenshots/edit-1.jpg)
Luego, su página se convierte en un editor de texto, en donde usted puede modificar el código de la página. La página se escribe en [markdown] (http://daringfireball.net/projects/markdown/syntax), muy fácil de entender.
![photo](images/screenshots/edit-2.jpg)
Usted no tiene que modificar este código, solo copie y pegue el texto entero en su editor de texto local, luego traduzca las partes textuales en su idioma, sin modificar las partes con paréntesis y HTML. Guarde el texto a continuación y envíenosla por correo a nosotros en [play@primo.io] (mailto: play@primo.io)
3. (avanzada, automatización completa) Este método es ligeramente avanzado, pero nada que sea difícil, si usted no está familiarizado con GitHub usted tiene la oportunidad de aprender algo nuevo :) <br>

Si ya está familiarizado con git, usted tiene hacer fork al repositorio, todas las traducciones están ubicadas en la carpeta _pages. Para traducir la página, sólo tienes que copiar el archivo con el idioma inicial ("english.md", por ejemplo) en la misma carpeta, a continuación, cambie el nombre del archivo con el idioma final (spanish.md) luego traduzcalo. Una vez terminado, realice un pull request para agregar el archivo a la carpeta, se añadirá automáticamente al menú. <br><br>
Los pasos anteriores, en detalle:

    1. Cree una cuenta de git
    2. Descargue el software de GitHub ([Mac](http://mac.github.com/), [Windows](http://windows.github.com/))
    3. Si es la primera vez que usted lo usa, ábralo e ingrese los detalles de login
    4. Ingrese a la sección [this documentation repository](https://github.com/primo-io/prototype-documentation)
    5. Haga clic en el botón "Fork" en la esquina superior derecha, para hacer el "fork" de este repositorio en su cuenta.
    6. Ingrese a su cuenta de gitHub, abra la página del repositorio al que le ha hecho "fork" y haga click en el botón "Clone in Desktop", en la barra lateral de la derecha. Esta automáticamente abrirá la aplicación de GitHub preguntando donde debe almacenar el repositorio en su computador.
    7. Después selecciones un directorio destino en su computador, de clic en "clone"
    8. Luego de descargar los archivos, navegue hacia su directorio local donde el repositorio ha sido descargado.
    9. Abra el directorio _pages, donde todas las traducciones estan localizadas. Seleccione el idioma de origen ("english.md" por ejemplo), luego copie el archivo y cambiele el nombre al de su idioma de destino ("spanish.md" por ejemplo), en el mismo directorio.
	10. Abra el archivo recien creado y realice la traducción en su idioma, manteniendo el formato de las etiquetas.
    11. Después de que la traducción este completa y guardada, es el momento de recargarla en GitHub. abara la aplicación de GitHub y de doble clic en el repositorio. Sobre la barra lateral izquierda, de clic en el tabulador "Changes". Este debería decir "Uncommited Changes".
    12. DE un pequeño título a sus ediciones, por ejemplo "spanish translation", luego de clic en "commit" y luego en el boton "sync"
    13. Vaya a su perfil de GitHub, en la página del repositorio al que realizó "fork". Usted debería estar en capacidad de ver su página recientemente creada en el folder _pages. En la parte de arriba, debería estar un boton verde con dos flechas. de clic en este para iniciar un requerimiento de "pull". (Vea la imagen abajo)
    ![photo](images/screenshots/pull-1.jpg)

	14. Luego de clic en "Create Pull Request"
	![photo](images/screenshots/pull-2.jpg)

	15. Escriba un mensaje para el requerimiento de pull y eso es todo!. Ahora usted solo que aprobar el requerimiento.

<br>

## 1. Que es Primo

![primo play set](images/photo/primo.jpg)

Primo es una interfaz tangible diseñada para introducir a los niños pequeños (3 a 7 años) en la programación lógica, sin la necesidad de que ellos sepan leer aún. El objetivo del juego es conducir un pequeño robot llamado Cubetto de regreso a su casa. Para llevar a cabo la misión, los niños deben programar el robot usando un limitado juego de instrucciones: adelante, izquierda, derecha y función. Mientras que las primeras tres instrucciones son muy intuitivas, la cuarta llama a una subrutina, una linea de instrucciones extra empacadas en un solo comando.

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/82620072" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>

## 2. Investigación y desarrollo

La enseñanza de la programación para los niños es un tema ámpliamente debatido. Conocemos un número limitado de soluciones que tratan de lograr esto para niños mayores de 8 años de edad. Sin embargo, no hay muchas de estas soluciones adecuadas para los niños más pequeños, y no hay ninguno que funcione sin una pantalla o sin la necesidad de que el niño sepa leer. Vemos un número creciente de aplicaciones para las tabletas y los ordenadores que también trabajan en combinación con robots físicos, pero ninguno de ellos son completamente de dominio libre de la misma forma que el Juego Primo lo es.

La madera ha sido escogida como el material principal, en primer lugar porque es natural; da una cálida sensación y hace un sonido agradable. La segunda razón es cultural. Las observaciones que se realizaron en juegos utilizados en las guarderías tradicionales Suizas (donde el producto fue diseñado originalmente) descubrieron que los juegos más queridos por los niños estaban hechos de madera. Los juguetes de madera son muy durables,  se pueden ver las marcas y arañazos en ellos, signos de su uso en el pasado por otros niños. Es un material con memoria. La madera también fue elegida como material debido al fuerte contraste que crea con la tecnología. Dentro de Primo hay una placa de circuito, pero queríamos crear una experiencia "mágica", ocultando la complejidad del sistema del juego.

<img class="float" src="images/photo/logo-turtle.jpg">

El concepto detrás de Primo está fuertemente inspirado por el trabajo de Seymour Papert, matemático quien co-fundó el Laboratorio de Inteligencia Artificial del MIT con Marvin Minsky, en los años sesenta (si usted está interesado en el tema, le recomendamos que lea [Mindstorms](http://www.amazon.co.uk/Mindstorms-Children-Computers-Powerful-Ideas/dp/0465046746/ref=sr_1_1?ie=UTF8&qid=1393675158&sr=8-1&keywords=mindstorms+papert), su libro más famoso). Él estaba dirigiendo el equipo que inventó [LOGO] (http://en.wikipedia.org/wiki/Logo_ (lenguaje de programación)), probablemente el recurso más utilizado y por más tiempo usado para enseñar programación a los niños. El objetivo de Seymour Papert no era sólo enseñar código, sino también para ayudar a los niños a descubrir su propia forma de resolver problemas. Primo se puede considerar una simplificación extrema de LOGO y una tortuga física. Hemos limitado las instrucciones, a su forma más pura, evitando cualquier tipo de texto o lenguaje numérico.

El primer prototipo fue realizado en SUPSI Lugano por Matteo Loglio (co-fundador de Primo.io y diseñador de interacción), durante la [MAInD - Máster de Estudios Avanzados en Diseño de Interacción] (http://www.maind.supsi.ch/) . Los conocimientos de Matteo están basados en el diseño del producto,  después de aprender los conceptos básicos de Arduino y un poco de código para crear el prototipo, empezó a buscar soluciones técnicas accesibles para un novato, con el fin de desarrollar una aplicación como Primo. Los principales temas fueron dos: hacer un coche robot desde cero y una interfaz que pudiera reconocer fácilmente las diferentes instrucciones.

El primer problema del proyecto se resolvió mediante el uso de un [placa Oh_Oh] (http://david.cuartielles.com/w/Maquila2/Ohoh) de David Cuartielles, uno de los fundadores de Arduino quién ofreció una conferencia en SUPSI. El robot Oh_Oh es un proyecto abierto, se pueden encontrar los archivos de origen en el enlace de arriba. Se trata básicamente de un coche con forma de Arduino, sólo se añadió un XBee para la comunicación de radio.

El segundo problema fue el diseño de un método confiable para detectar los bloques. Una solución fue inspirada por un proyecto [CIID] (http://ciid.dk/) llamado ["Barcode Piano"](http://ciid.dk/education/portfolio/idp11/courses/physical-computing/projects/barcode-piano/ )

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/19704918" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>

La idea es utilizar múltiples bloques que pueden ser reconocidos por una tablero mediante resistencias. Es un divisor de tensión básica, con los pines analógicos de un Arduino leyendo los valores de resistencia. Es un método muy simple, pero también muy eficaz para un prototipo.

Design-wise, algunas características requieren pruebas; el diseño actual es el resultado de varias iteraciones.

La ruta 'culebra' o 'zig-zag' se eligió para evitar preconcepciones debidas a saber leer.

![left to right](images/illustrations/left-to-right.jpg)

Los bloques conectores en forma de "D", fueron diseñados para que estos se puedan insertar de sólo una forma también para ser coherentes con el diseño de recorrido y la dirección del robot coche "cubetto". Múltiples diseños pueden ser utilizados para este propósito. La forma "D" fue escogida ya que es básicamente un "círculo orientado" , también recuerda los diseños de juguetes similares.

![instruction blocks](images/photo/instruction-blocks.jpg)

El diseño de la forma de los bloques de instrucciones aún está siendo probado. El diseño actual funciona bastante bien, los niños captan fácilmente su significado, en lo único que tienen dificultades es para familiarizarse primero con el bloque de izquierda y derecha. Esto también es debido a que el concepto de "derecha" e "izquierda" en general es bastante nuevo para ellos. Actualmente estamos probando otro diseño de bloques, para mejorar aún más.

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/50570097" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>

Al principio el robot era un coche de juguete. Una forma muy complicada y que requería mucho tiempo para su producción, ya que consistía en cortes de láser pegados capa por capa, y posteriormente lijada durante más de una hora. El coche tenía otro problema importante, que era muy orientado hacia los varones. Queríamos evitar entrar en discusiones sobre si los fabricantes solo producían juguetes para el cerebro únicamente orientados hacia los varones. Queríamos permanecer neutrales en ese aspecto, no queríamos crear un juguete específicamente para niños o niñas, y en su lugar optamos por una geometría muy neutral, una caja.

Le dimos un nombre a la pequeña caja, junto con una personalidad y una cara sonriente, lo que lo hace aún más atractivo para los niños. El robot se llama Cubetto (pequeño cubo en italiano). La idea con Cubetto es también crear un módulo básico que se puede ampliar y personalizar fácilmente en el futuro.

![cubetto](images/photo/cubetto.jpg)

## 3. Primeros pasos

### 3.1 Los básico

Primo se compone de tres partes: una tablero de interfaz, CUBETTO y un conjunto de bloques de instrucciones. Los niños interactúan con el tablero de interfaz mediante la colocación de bloques de instrucciones en los agujeros, para crear una secuencia (un programa) que Cubetto ejecuta.

Hay cuatro tipos de bloques de instrucciones, esto significa que las resistencias de 4 valores diferentes se pueden utilizar, con valores distantes entre sí.

Los bloques se insertan en los agujeros del tablero de interfaz, donde se identifica el valor de la resistencia. Después de eso, los valores son procesados ​​en una cadena de caracteres que se envía a Cubetto usando dos módulos XBee. Cubetto a continuación, ejecuta las instrucciones, una después de la otra.

El cerebro del prototipo está hecho de dos placas Arduino, un arduino UNO (puede ser un Leonardo o un Duemilanove) para Cubetto y un Mega para la placa de interfaz, donde se requieren 16 entradas analógicas.

### 3.2 Electrónica

### Herramientas requeridas

* Soldador
* Soldadura
* Alambres
* Pistola de pegamento caliente
* Pegamento de madera
* Cinta de cobre de 5mm ancho

### Materiales (Precios en euros)

Cubetto ~ 88 €

* Arduino UNO (o Leonardo) - 20 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=195#.UxC5nfTV_bA)
* Arduino Proto Wireless Shield - 14.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* SN754410 Motor Driver - 3.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_33&products_id=153#.UxC5-_TV_bB)
* XBee (serie 1 o 2, no hace ninguna diferencia) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* Ruedas solarbotics x 2 : 4.74 € - [Solarbotics Store](https://solarbotics.com/product/gmpw/)
* Motores para ruedas solarbotics GM3 x 2 : 8.36 € - [Solarbotics Store](https://solarbotics.com/product/gm3/)
* 2 Ruedas de bolas : 5.79 € - [Solarbotics Store](https://solarbotics.com/product/23160/)
* CNY70 x 2 : 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Vishay/CNY70/?qs=%2fha2pyFaduj8YpDhNNtXszq4w32cl%2fAjUjdOwQUvJUM%3d)
* (opcional) Soporte de baterias: 4 € - [Solarbotics Store](https://solarbotics.com/product/bholdaa_4_cell/)
* (opcional) 4 x Baterias recargables

Tablero de interfaz ~ 88 € (pura coincidencia)

* Arduino Mega 2560 : 39.00 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=196#.UxC_gPTV_bA)
* Arduino Proto Wireless Shield : 14.90 - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* XBee (serie 1 o 2, no hace ninguna diferencia) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* 16 5mm LED Rojo: 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Lite-On/LTL-4223/?Lite-On/LTL-4223/&qs=sGAEpiMZZMusoohG2hS%252b15J8d1kHl%252bvkJpzS4atZNEA=)
* 16 resistencias de 220 Ω : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 16 Resistencias de 10K Ω : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 1 Push Button : 1 €
* 50 conectores macho : 1 €
* 16 conectores macho dobles : 0.50 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=294#.UxC_3fTV_bA)
* 50 conectores hembra : 1 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=188#.UxDAAfTV_bA)
* 16 Magnetos ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

Bloques de instrucción ~ 4 €

* 4 Resistencias de 4.7K Ω : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-47K-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2fbdyz6pU6a%252bvHlD5kaZWgo%3d)
* 4 Resistencias de 100K Ω: 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-100K-RC/?qs=sGAEpiMZZMu61qfTUdNhG81NIhcRRUJQxII5Nsctha8%3d)
* 4 Resistencias de 220 Ω Resistor : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 4 Resistencias de 10K Ω Resistor : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 16 Magnetos de ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

### 3.3 Energía

Cubetto y (opcionalmente) la tarjeta de interface, funcionan con baterías. Para el prototipo se puede utilizar una batería de Li-Po o pilas AA normales, depende de usted. Nosotros utilizamos ambas, las baterías de Li-Po son buenas, pero necesitan un equipo adicional, si usted está comenzando desde cero, recomendamos baterías AA. Sólo recuerde que se agotan muy rápidamente, así que lo mejor sería utilizar baterías recargables, como las de NiMh.

### 3.4 Diseño de prototipo

Todo el producto se construye con madera cortada con láser, principalmente de 4 mm de espesor, con una capa adicional de 1 mm de espesor. Usted puede solicitar el servicio de corte de las partes en sitios como Ponoko, o en su FabLab local. El primer prototipo fue cortado con láser en el interior [FabLab Lugano] (http://fablab.supsi.ch/), mientras que el desarrollo de productos avanzados en [FabLab Torino] (http://fablabtorino.org/), donde todavía reside parte del equipo de desarrollo de Primo.

Construir a Cubetto y el tablero de interfaz es un procedimiento laborioso, pero muy simple, sus carcasas son básicamente cajas. La verdadera complejidad radica en los bloques de instrucciones. Consisten en una capa de madera de 4 mm doble con imanes y resistencias soldadas en el interior.

## 4. Construcción del prototipo

### [Descargar ARchivos fuentes](files/primo-prototype-laser.zip)

### 4.1 Tablero de Interfaz

Para construir la tablero de interfaz usted tiene que cortar dos archivos laser: interface-board-4mm.dxf y interface-board-1mm.dxf: la primera es para la madera contrachapada de 4 mm y la segunda para la madera contrachapada de 1 mm. Como se puede ver en los archivos, las piezas están numeradas, para facilitar el proceso de montaje. Los números se almacenan en una capa diferente, por lo que puede eliminar fácilmente antes del tratamiento con láser. Se recomienda ajustar la perforación para el botón pulsador, en función del tamaño del botón que desee utilizar.

Primero que todo, usted tiene que pegar juntas las partes 3 y 4, utilizar los agujeros en las esquinas para alinearlos con tornillos mientras el pegado dejar reposar durante una noche.

Luego tome la cinta de cobre, corte 32 piezas de 70 mm cada una y pongalas dentro de las perforaciones rectangulares en la parte que usted acaba de pegar,  debe tener al menos de 30 mm de ancho a cada lado. Una vez terminado, ahora se puede pegar todos las capas superiores restantes del tablero de interfaz, este es el orden correcto:


![copper connectors](images/illustrations/board-1.jpg)
![copper connectors](images/illustrations/board-2.jpg)

Una vez que usted haya finalizado, usted puede pegar las partes pegadas previamente, 1+2 con 3+4.

![copper connectors](images/illustrations/board-esploso.jpg)

Una vez que el pegamento ha secado, ponga los magnetos en los agujeros pequeños. De vuelta hacia abajo a la tapa superior y rellene los agujeros pequeños con los magnetos, asegúrese que todos estén en la misma dirección, no importa si esta es norte o sur. Selle el agujero con un poco de pegamento caliente.

Ahora la electrónica. Comience haciendo carriles para los 5V y la tierra, todo a través de los agujeros como aparece en la imagen. El primer prototipo nunca tuvo tiras de cobre, este tenia alambres (los que todavía se pueden usar). pero en este prototipo usamos cinta de cobre para los carriles. Con ellos ahorramos un 100% de tiempo. Esta técnica también hace las cosas mucho mas fáciles para crear conexiones.

![rails](images/illustrations/board-3.jpg)

El siguiente paso es cablar uno de los dos conectores de cada agujero al carril de conexión a tierra. Si usted usa cinta de cobre, usted solo necesita usar una pequeña tira mas de ella, solo so suficientemente lar para que toque ambos terminales.

![rails](images/illustrations/board-5.jpg)

Ahora tenemos que conectar el otro lado de cada conector al carril de 5V. pero esta vez, con una resistencia intermedia de 10KΩ. Una cosa atractiva de la cinta de cobre es que la soldadura funciona bastante bien en la parte de arriba de esta. ESta es la técnica usada:

![10k](images/photo/diy-docs-1.jpg)
Al final de este proceso, usted debería tener algo como esto:

![10k scheme](images/illustrations/board-6.jpg)

Ahora es momento de poner los LEDs; pegue un LED rojo en cada uno de los 16 agujeros, luego use una gota de pegamento caliente para pegarlo a la madera. Una vez que el pegamento esté frió, proceda a conectarlo. Tenga en mente que los LED tiene polaridad: La terminal larga es el ánodo y la corta el cátodo. Conecte cada cátodo a carril de terminal de tierra usando una resistencia de 220Ω.

![10k](images/photo/diy-docs-6.jpg)

Conecte cada cátodo al carril de conexión a tierra, usando una resistencia de 220Ω


![10k scheme](images/illustrations/board-7.jpg)

La terminal larga del LED, debe estar conectada a un terminal I/O en el Arduino Mega, estos pines están numerados desde el 22 hasta el 53. Los LEDs deben estar conectados en orden, esto hará mucho mas fácil luego el acceso a estos en el código, en mi prototipo por ejemplo Inicié desde el pin 30 hasta el 45 (Son 16 LEDs)
El punto de inicio no es importante, siempre y cuando estén en el orden secuencial correcto. Esto significa que si nosotros comenzamos desde el pin 30. el primer LED debería estar conectado al pin 30, el segundo al pin 31, el tercero al pin 32 así hasta que el pin 16 esté conectado en el pin 45.

Los cables se sueldan a un rack macho doble, dado que los pines digitales en el Arduino mega están dispuestos en una doble línea. De esta forma es mas fácil conectar y remover el Arduino del tablero.

![rack](images/photo/diy-docs-4.jpg)

Una vez que todos los LEDs están soldados, tenemos que soldar los conectores hechos a mano. Estos deben ser conectados a los pines análogos del Arduino Mega, para leer los diferentes valores de resistencia. Al igual que los LEDs, éstos deben conectarse en orden, empezando por A0 para el agujero 1 y A15 para el agujero 16. El cable tiene que empezar desde el mismo punto en el que previamente fue soldada la resistencia de 10K. Véase la ilustración:

![analog input board connections](images/illustrations/board-8.jpg)

<div class="cf">
<img class="float cf" src="images/illustrations/button.jpg">

<p>
Aquí he utilizado algunos conectores macho individuales, ya que los pines analógicos están todos en una sola línea.

</p>

<p>
La última cosa a conectar es el botón: tome y suelde dos cables a las dos cabeceras opuestas, entonces deslicelos hacia el agujero del botón, desde la parte superior, y empújela hasta el fondo, hasta que se detenga. Ahora de vuelta al tablero, usted debería tener los dos cables que salen del agujero. Conéctelos como se ve en la ilustración: uno directamente a 5V, el otro a GND utilizando una resistencia de 10K. Luego conéctelo a un pin digital Arduino desde desde las terminales de la resistencia, en este ejemplo hemos utilizado el pin número 50.
</p>
</div>


![photo](images/photo/diy-docs-5.jpg)

Ya casi hemos terminado con el tablero, ahora sólo hay que enchufar el Wireless Shield en la parte superior del Arduino Mega y poner las terminales en su lugar correspondiente del tablero. Para recapitular, de 30 a 45 para los LEDs, A0 a A15 para los conectores y 50 para el botón.  Utilice desde A0 hasta el A5 en los pines del Wireless Shield durante los primeros 5 conectores.  No olvide conectar el carril de tierra al pin GND y el carril de 5V al pin de 5V.

![rack](images/photo/diy-docs-3.jpg)

Ahora algo de ajuste fino: después de que la parte 12 del tablero ha sido pintada usted puede pegar la parte 13 en la parte superior del tablero.

Lo mismo para el botón rojo: después de que la parte 14 halla sido pintada, ponga algo suave como cartón en la parte superior de la parte 2, alrededor del botón, a continuación, use un poco de pegamento caliente en la parte superior del pulsador y antes de que el pegamento se seque, coloque el botón rojo. Consulte la ilustración:

![photo](images/illustrations/button-mechanics.jpg)

### BLOQUES DE INSTRUCCIONES

Este es el detalle de un bloque de instrucciones explotado:

<img class="float cf" src="images/illustrations/instruction-esploso.jpg">

Para hacer los bloques de instrucciones, lo primero que tiene que hacer es cortar los archivos laser,  hay uno para madera de 4 mm de espesor y uno para madera de 1 mm. Son cuatro capas, numeradas de 1 a 4 y los dibujos proporcionados pueden ser utilizados para hacer 16 bloques, cuatro de cada tipo.

Cada bloque tiene una resistencia diferente. Estas son las resistencias utilizadas en el prototipo:

ADELANTE: 4.7K Ω<br>
IZQUIERDA: 100K Ω<br>
DERECHA: 220 Ω<br>
FUNCIÓN: 10K Ω

Para hacer los bloques, primero tiene que pegar la parte 4 con la parte 3.

Después de que el pegamento se haya secado, se puede empezar a pintar. Consulte la siguiente ilustración para ver de que color es cada parte:

![image](images/illustrations/colors.jpg)

Ahora tiene que cortar dos trozos de cinta de cobre, de 40 mm de largo. deslizar los en los agujeros de los dos bloques en los que aplico el pegamento, haciendo un anillo alrededor de ellos usando la fisura superior e inferior, el anillo debe ser muy apretado.

![photo](images/illustrations/instruction-block-guide.jpg)

Después de eso, usted tiene que poner el imán en el agujero. Mientras hace esto, ASEGURESE DE QUE ESTE ORIENTADO CORRECTAMENTE,de manera que el bloque 'pegue' en el agujero. si se pone de la forma contraria, va a ser repelido por el otro imán, un resultado gracioso, pero no es lo que queremos lograr.

Fije el imán con una gota de pegamento caliente y antes de que el pegamento se enfríe, coloque la resistencia de la derecha en la parte superior, con las patas sobre la cinta de cobre. Después de eso, la resistencia debe ser soldada en las dos piezas. Luego de soldar, corte la longitud de la pata extra y pegue la parte 2 en la parte superior de la resistencia.

Termine su bloque pegando la última capa, la parte numero 1 en la parte superior, luego repita el proceso para cada bloque :)




### CUBETTO

Electronica:

El prototipo para Cubetto se puede construir utilizando un Arduino Uno o Leonardo, con un Wireless Shield Proto en la parte superior. Se usa la Proto Shield porque tiene una pequeña área de la creación de prototipos, lo suficientemente amplia como para poner el controlador del motor, los conectores para los codificadores ópticos, motores y alimentación eléctrica.

Cubetto tiene que girar 90 grados a la izquierda y derecha. Una forma muy inexacta es utilizar eventos temporizados, como "giro a la derecha por un segundo" y usted puede esperar más o menos el mismo resultado. "Más o menos", ya que depende mucho de diferentes factores, tales como el suelo, la energía de la batería y otros más. La forma en que resolvió este problema, es mediante la detección de la cantidad de rotación de la rueda utilizando dos codificadores ópticos CNY70 en combinación con un adhesivo. La pegatina va en la rueda interior y es algo como esto:

![photo](images/photo/diy-docs-14.jpg)

La etiqueta se divide en franjas en blanco y negro, esto se debe a que el CNY70 es capaz de detectar la variación entre una franja blanca y una negro. Básicamente su interior tiene un LED de infrarrojos que está siempre encendido y un fototransistor que está leyendo la cantidad de luz infrarroja. Cuando un material negro se enfrenta al componente, casi no hay luz reflejada, debido a que el color negro tiende a absorber la luz. Por el contrario, si el material es de color blanco, se refleja toda la luz, por lo que el valor leído por el sensor es muy alto. La diferencia entre las lecturas se utiliza para contar los pasos de rotación.

![photo](images/illustrations/cny70-physycs.jpg)

El área de prototipo del Proto Shield Wireless es donde se sueldan el driver del motor y otros conectores para las otras partes. Para este propósito simplemente use conectores macho como conectores y conectores hembra en la otra parte.


![photo](images/illustrations/wireless-shield-connections.jpg)

Para estos simplemente usé conectores macho como conectores y conectores hembra en la otra parte.

![photo](images/photo/diy-docs-12.jpg)

![photo](images/illustrations/wireless-shield-connections-1.jpg)

El controlador de motor SN754410 tiene 16 pines que deben conectarse siguiendo este esquema:

![photo](images/illustrations/motor-driver.jpg)

Diseño:

Comience por grabar y cortar con la laser el archivo cubetto.dxf; Todas las partes CUBETTO se cortan de la madera contrachapada de 4 mm, siga estas instrucciones visuales para construir la base:

![photo](images/illustrations/cubetto-guide.jpg)

No monte los motores, por ahora, primero hay que montar las ruedas de bolas.

![photo](images/illustrations/ball-caster.jpg)

![photo](images/photo/diy-docs-9.jpg)

Ahora el componente CNY70. Soldar las dos terminales opuestas, que deben ser conectadas a 5V, junto con un cable; luego soldar tres cables a los conectores restantes del CNY70. Al final de estos cables soldar una fila de tres conectores hembra. Que posteriormente se conectan a las terminales del proto shield.

Los dos cny70 deben ser colocados en el borde de la capa inferior, con el LED y el fototransistor alineados horizontalmente. Para fijarlos se puede utilizar un poco de pegamento caliente (u otros tipos de pegamento).

Ver la imagen para entender la ubicación.

![photo](images/photo/diy-docs-11.jpg)

Al igual que para el CNY70, soldar dos cables a las pequeñas terminales que salen de cada motor. Usted puede entretejer los dos cables para que sean más resistentes, luego, al final, solde una fila de dos conectores hembra, al igual que en la ilustración.

Ahora imprima el dibujo interior con las franjas en blanco y negro, péguelas en un pedazo de cartón (o de madera de corte por láser, eso depende de usted), corte el perímetro y haga un agujero en el medio, ya que se insertan entre el motor y la rueda. Las franjas de blanco y negro deben apuntar hacia el lado interno del Cubetto y la distancia entre el el impreso y el CNY70 debe estar entre 1 y 3 milímetros para que funcione correctamente.

![photo](images/photo/diy-docs-10.jpg)

Ahora usted puede poner las ruedas en los motores, si usted usa las ruedas Solarbotics, se puede sujetar con el tornillo suministrado, sin hacer demasiada presión.

Pegue tres de las cuatro "paredes" de Cubetto, partes 5, 7 y 8. Vamos a dejar la parte trasera extraíble, por si acaso queremos modificar algo.

Tome el soporte de la batería y suelde el cable negro y rojo para los dos conectores hembra. Los conectores en el shield irán a VIN y a tierra. Un interruptor que interrumpa el cable rojo es muy sugerido.

![photo](images/photo/diy-docs-13.jpg)

Ahora puede colocar el Arduino + Proto shield en la parte superior de los motores, conecte todos las terminales en el shield y usted ha terminado de construir el Cubetto.
