# 3 Raspberry Pi Pico W Anwendungen

## Gliederung

[3.1 LED blinken](3.1LEDBlinken)<br>
[3.2 LED dimmen](3.2LEDDimmen.md)<br>
[3.3 LED schalten](3.3LEDSchalten.md)<br>
[3.4 LED Fußgängerampel](3.4Fussgaengerampel.md)<br>

## Generelles Vorgehen

Hier stellen wir die Pi Pico-Anwendungen vor, die wir realisieren wollen. Jedes Unterkapitel hat folgende Struktur

- **Die Hardware- und Elektronikgrundlagen**: Alle neuen Hardwarekomponennten werden kurz vorgestellt.

- **Die Anwendungen**: Wir zeigen die Anwendungen mit vorgegebenen Sourcecode.

    Das Vorgehen bei allen Anwendungen ist immer
    
    1. Zuerst die Schaltung aufbauen

    2. Pi Pico per USB mit dem Computer verbinden

    3. Thonny starten und das Script kopieren/erstellen

    4. Programm ausführen

- **Die Aufgaben**: zu den Anwendungen werden Aufgaben gestellt, mit den Schwierigkeitsleveln: Level 1 (sehr leicht), Level 2 (ganz ok) oder Level 3 (schwer). 

- **Die Programmierung**: Im Endeffekt wollen wir die Anwendungen ausprobieren UND die Programmierung verstehen. In diesem Abschnitt wird auf den Sourcecode eingegangen. Oftmals wird nicht alles besprochen, sondern es wird mit einfacher Syntax begonnen und wir steigern uns langsam. Am Anfang verstehen wir also noch nicht alle Zeilen Sourcecode, sondern nehmen vieles als gegeben hin.

## Raspberry Pi Pico Pinout

Die Übersicht über die Pinbelegung des Raspberry Pi Pico [hier als PDF](https://datasheets.raspberrypi.com/picow/PicoW-A4-Pinout.pdf) ist bei umfangreicheren Projekten sinnvoll, wenn auch jetzt noch nicht notwendig.

![Raspberry Pi Pico W Pinout](media/picow-pinout.svg)



