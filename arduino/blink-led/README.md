# Blink led

## Montage

![](schema-arduino-blink-led.png)

## Code

```java
/*
  Blink led

  Allume une LED pendant une seconde, puis l'éteint une seconde, puis recommence.

  Extrait de :
  http://www.arduino.cc/en/Tutorial/Blink
*/

// La fonction setup() est exécutée au lancement de la carte Arduino (une seule fois)

void setup() {
  // On définit le pin digital d'une LED par défaut (PIN 13) comme une valeur à envoyer.
  pinMode(LED_BUILTIN, OUTPUT);
}

// La fonction loop() est exécutée en boucle, indéfiniment

void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // Allume la LED (HIGH est le voltage maximal)
  delay(1000);                       // Attend une seconde
  digitalWrite(LED_BUILTIN, LOW);    // Éteint la LED (LOW est le voltage minimal, donc 0)
  delay(1000);                       // Attend une seconde
}
```