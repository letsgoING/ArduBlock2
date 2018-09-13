# ArduBlock 2 letsgoING #

Aktuelle ArduBlock Version 2.03 für das [letsgoING-Projekt](http://letsgoing.org).
Getestet mit Arduino 1.8.7.

## Neuerungen in der Version 2 ##

### Standard und Experten Modus ###
Die größte Neuerung ist die Einführung zweier verschiedener Block-Menüs.
#### Standard-Blöcke ####
Das Standard-Menü enthält nur die für den Einstieg wichtigsten Blöcke.
Die Blöcke sind auf den Grundlagenkurs von [letsgoING](http://letsgoing.org) zugeschnitten.
#### Experten-Blöcke ####
Die Experten-Blöcke beinhalten alle Standard-Blöcke und viele zusätzliche Funktionen.
Es können z.B. Unterprogramme erstellt, Interrupts genutzt und Servos oder Schrittmotoren angesteuert werden.
Die Variablen werden um neue Datentypen ergänzt, es gibt mehr Möglichkeiten für die serielle Kommunikation und es kann geschriebener Code eingefügt werden.

### Variablen-System ###
Es gibt seit dieser Version
- digitale Variablen (bool) *Standard*
- analoge Variablen (int16) *Standard*
- kurze analoge Variablen (int8)
- lange analoge Variablen (long)
- dezimale analoge Variablen (float)
- Tabellen für analoge Variablen (int16-Array)

Alle Variablen können als
1. globale Variable
2. lokale Variable
3. Konstante

verwendet werden.

Außerdem können die analogen Variablen in jeweils andere Variablen-Typen gewandelt werden (cast).

### Workspace zoomen ###
In unserer Version von ArduBlock ist es jetzt möglich die Programmierfläche zu vergrößern oder verkleinern.
So kann das Fenster immer der Programmgröße angepasst werden.

**Achtung:** Wenn Blöcke geklont werden, passen diese sich noch nicht automatisch dem Zoom-Faktor an. Durch erneutes Zoomen lassen sich die Blöcke aber anpassen.

### Bild-Export ###
Wird ein Programm als Bild gespeichert, wird das Bild auf die Programmgröße zugeschnitten und mit transparentem Hintergrund gespeichert.


## Installation in der Arduino IDE ##
1. [Arduino IDE](https://www.arduino.cc/en/Main/Software) für das eigene Betriebssystem herunterladen (Installations- oder Zip-Version)
2. ArduBlock2 als ZIP herunterladen und ArduBlockTool-Ordner entpacken
3.a INSTALLATION: Im Home-Verzeichnis (Sketchbook) der Arduino IDE "tools"-Ordner erstellen und ArduBlockTool-Ordner in das Verzeichnis kopieren
3.b ZIP-Version: ArduBlockTool-Ordner in das "tools"-Verzeichnis der Arduino IDE kopieren (der "tools"-Ordner liegt im Hauptverzeichnis der Arduino IDE)
4. *Wenn die Q-Touch-Funktionen verwendet werden sollen, wird die [LGI-QTouch Library](https://github.com/letsgoING/Libraries) benötigt.*
5. *Wenn die NeoPixel-Blöcke verwendet werden sollen, wird auch noch die [NeoPixel-Library](https://github.com/adafruit/Adafruit\_NeoPixel/archive/master.zip) von Adafruit benötigt.*