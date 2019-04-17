# ArduBlock 2 letsgoING #

Aktuelle ArduBlock Version 2.10 für das [letsgoING-Projekt](http://letsgoing.org).
Getestet mit Arduino 1.8.9

## Neuerungen in der Version 2 ##

### Standard und Experten Modus ###
Seit Version 2 gibt es zwei verschiedene Block-Menüs.
#### Standard-Blöcke ####
Das Standard-Menü enthält die für den Einstieg wichtigsten Blöcke.
Die Blöcke sind auf den Grundlagenkurs von [letsgoING](http://letsgoing.org) zugeschnitten.
#### Experten-Blöcke ####
Die Experten-Blöcke beinhalten alle Standard-Blöcke und viele zusätzliche Funktionen.
Es können z.B. Unterprogramme erstellt, Interrupts genutzt und Servos oder Schrittmotoren angesteuert werden.
Die Variablen werden um neue Datentypen ergänzt, es gibt mehr Möglichkeiten für die serielle Kommunikation und es kann geschriebener Code eingefügt werden.

### Variablen-System ###
Es gibt
- digitale Variablen (bool) *Standard*
- analoge Variablen (int16) *Standard*
- kurze analoge Variablen (int8)
- lange analoge Variablen (long)
- dezimale analoge Variablen (float)
- Zeichen-Variablen (char) 
- Tabellen für (kurze/lange/dezimale) analoge Variablen (intX/float-Array)
- Zeichenketten (char-Array)

Alle Variablen können als
1. globale Variable
2. lokale Variable
3. Konstante
verwendet werden.
Außerdem können die Datentypen in jeweils andere Typen gewandelt werden (cast → im Experten-Menü).

### Workspace zoomen ###
In unserer Version von ArduBlock ist es möglich die Programmierfläche zu vergrößern oder verkleinern.
So kann das Fenster immer der Programmgröße und Auflösung angepasst werden.

### Bild-Export ###
Wird ein Programm als Bild gespeichert, wird das Bild auf die Programmgröße zugeschnitten und mit transparentem Hintergrund gespeichert.

### Copy-Paste ###
Über die Kopieren- und Einfügen-Schaltflächen lassen sich Programme zwischen verschiedenen ArduBlock-Fenstern übertragen.

### ShortKeys ###
Die wichtigsten Funktionen in ArduBlock sind nun über Shortkeys erreichbar (Strg+TASTE).
- Programm öffnen → Strg+O
- Programm speichern → Strg+S
- neues Programm → Strg+N
- Programm hochladen → Strg+U
- Seriellen Monitor öffnen → Strg+M
- Bild speichern → Strg+P
- Programm vergrößern → Strg+Plus
- Programm verkleinern → Strg+Minus
- Programmgröße zurücksetzen → Strg+Null
- Blöcke klonen → Strg+Rechtsklick

## Installation in der Arduino IDE ##
1. [Arduino IDE](https://www.arduino.cc/en/Main/Software) für das eigene Betriebssystem herunterladen (Installations- oder Zip-Version)
2. ArduBlock2 als ZIP herunterladen und ArduBlockTool-Ordner entpacken
3.a INSTALLATION: Im Home-Verzeichnis (Sketchbook) der Arduino IDE "tools"-Ordner erstellen und ArduBlockTool-Ordner in das Verzeichnis kopieren
3.b ZIP-Version: ArduBlockTool-Ordner in das "tools"-Verzeichnis der Arduino IDE kopieren (der "tools"-Ordner liegt im Hauptverzeichnis der Arduino IDE)
4. *Wenn die Q-Touch-Funktionen verwendet werden sollen, wird die [LGI-QTouch Library](https://github.com/letsgoING/Libraries) benötigt.*
5. *Wenn die NeoPixel-Blöcke verwendet werden sollen, wird auch noch die [NeoPixel-Library](https://github.com/adafruit/Adafruit\_NeoPixel/archive/master.zip) von Adafruit benötigt.*