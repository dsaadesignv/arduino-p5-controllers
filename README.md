# Arduino

### Qu'est-ce que Arduino ?

En quelques mots, [Arduino](https://fr.wikipedia.org/wiki/Arduino) est une plateforme permettant de prototyper de manière assez simple des objets dits intelligents ou des dispositifs interactifs et/ou automatiques. Il s’agit d’[un ensemble de cartes électroniques](https://www.arduino.cc/en/Main/Products) pouvant être programmées afin de recevoir des données de [capteurs](https://fr.wikipedia.org/wiki/Capteur) (de lumière, de choc, de température, de distance, etc.) et envoyer des instructions à des [actionneurs](https://fr.wikipedia.org/wiki/Actionneur) (moteurs, leds, enceintes, etc.) ou à des programmes. Ces cartes se pilotent grâce à une [IDE](https://www.arduino.cc/en/Main/Software) (_integrated development environment_), logiciel permettant d’écrire des programmes et de les envoyer sur les différentes cartes par liaison USB.

### Qu'est-ce que p5.js ?

p5.js est une librairie Javascript qui permet de générer des visuels à partir de codes, de variables, de fonctions et d'algorithmes. p5.js reprend la logique du logiciel libre Processing en exécutant le code dans une page web : il est donc possible d'intégrer du langage web (HTML, CSS, Javascript) avec un script p5.js.

### Opportunités du duo Arduino + p5.js

D'un côté, Arduino est capable de recevoir des données de capteurs physiques réels, et peut stimuler des moteurs et des actionneurs. De l'autre, p5.js peut générer des visuels et interagir avec une interface web. Donc en reliant p5.js à Arduino, on peut facilement piloter une interface avec des contrôleurs tangibles, et on peut piloter des éléments tangibles via une interface. Bref, le futur.



-----



## Partie 1 : Arduino
Assurez-vous que [**l'IDE Arduino**](https://www.arduino.cc/en/Main/Software) soit installé sur votre ordinateur.

- [**Récupérer la valeur d'un bouton**](arduino/get-digital-value-of-button)
- [**Récupérer la valeur d'un potentiomètre**](arduino/get-analog-value-of-potentiometer)
- [**Récupérer la valeur d'un capteur de lumière**](arduino/get-analog-value-of-light-sensor)
- [**Faire clignoter une LED**](arduino/blink-led)
- [**Allumer ou éteindre une LED avec un bouton**](arduino/toggle-led-with-button)

## Partie 2 : Arduino + p5.js

Pour créer une connexion entre Arduino et p5.js, vous aurez besoin de [**l'application p5.serialcontrol**](https://github.com/p5-serial/p5.serialcontrol/releases/tag/0.1.2).

1. Téléversez un programme Arduino sur votre board via le logiciel Arduino ([**récupérer la valeur d'un bouton**](arduino/get-digital-value-of-button) par exemple), et fabriquez le montage associé
2. [**Ouvrez le script p5.js comme base**](https://editor.p5js.org/kevinvennitti/sketches/1NRTI6rhG) et dupliquez-le
3. Lancez le programme : l'écran affiche "Serial Port is Closed"
4. Ouvrez l'application p5.serialcontrol
5. Une fois ouverte, retournez dans votre script p5.js et lancez le programme : un "0" s'affiche
6. Avec votre doigt, appuyez sur le bouton de votre montage électronique : un "1" apparaît lorsque le bouton est pressé

-----




**Pour approfondir :**

- [Lire les 3 premiers chapitres du manuel _Floss_ dédié à Arduino](https://fr.flossmanuals.net/arduino/historique-du-projet-arduino/)
- [Regarder le _TED talk_ de Massimo Banzi, créateur d’Arduino](https://www.ted.com/talks/massimo_banzi_how_arduino_is_open_sourcing_imagination)
- [Aller voir plein de chouettes projets pilotés par Arduino sur l’excellent _CreativeApplications_](https://www.creativeapplications.net/category/arduino-2/)
- [Aller voir d’autres projets mis en avant sur le blog d’Arduino](https://blog.arduino.cc/category/featured/)



**Aller plus loin :**

- [Comprendre la différence entre analogique et digital](https://blog.robotiq.com/whats-the-difference-between-digital-and-analog-i/o)
