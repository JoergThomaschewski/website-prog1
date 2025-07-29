# 4 Python Grundlagen

## Gliederung

[4.1 Syntax und Variablen](4.1SyntaxUndVariablen.md)<br>
[4.2 Schleifen](4.2Schleifen.md)<br>
[4.3 Bedingte Anweisungen](4.3BedingteAnweisungen.md)<br>
[4.4 Ein- und Ausgabe](4.4EinUndAusgabe.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.4.1 Konsolenein-/ausgabe](4.4.1KonsoleneinAusgabe.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.4.2 GPIO: Ein- und Ausgang mit `Pin`](4.4.2GPIO-EinAusgang.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.4.3 Netzwerk-Ein-/Ausgabe (Webserver, HTTP)](4.4.3Netzwerk.md)<br>
[4.5 Fertige Funktionalitäten verwenden](4.5FertigeFunktionalitaeten.md)<br>
[4.6 Funktionen, Klassen und Methoden](4.6FunktionenKlassenMethoden.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.6.1 Funktionen definieren und verwenden](4.6.1Funktionen.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.6.2 Rekursion – Funktionen, die sich selbst aufrufen](4.6.2Rekursion.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.6.3 Klassen und Methoden: Grundlagen der OOP](4.6.3KlassenGrundlagen.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.6.4 Objektstruktur & Kapselung mit privaten Attributen](4.6.4Objektstruktur.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.6.5 Methoden sauber aufteilen: Verantwortung und Klarheit](4.6.5MethodenVerantwortung.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.6.6 Fehler vermeiden: Prüfungen und Absicherung](4.6.6FehlerAbsicherung.md)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[4.6.7 Zwei Klassen im Zusammenspiel (z. B. Horse & Student)](4.6.7ZweiKlassen.md)<br>
[4.7 Bibliotheken](4.7Bibliotheken.md)<br>
[4.8 Daten speichern](4.8DatenSpeichern.md)<br>
[4.9 Verzeichnisse bearbeiten](4.9Verzeichnissebearbeiten.md)<br>
[4.10 MicroPython-spezifische Funktionen](4.10UebersichtMicroPythonSpezifischeFunktionen.md)<br>
[4.11 Dies und Das](4.11DiesUndDas.md)<br>

---

---

## 📜 Überblick: Was erwartet dich?

In diesem Kapitel lernst du die **wichtigsten Grundlagen der Programmierung** mit Python und MicroPython kennen – Schritt für Schritt und praxisnah.

Wir starten mit **Syntax und Variablen**, dann folgen **Schleifen**, **Bedingungen** und die **Ein-/Ausgabe** über Konsole, GPIO oder Netzwerk.

Danach vertiefen wir die Strukturierung mit **Funktionen, Klassen und Methoden**, inklusive Fehlerbehandlung und objektorientierter Programmierung.

Im Anschluss erfährst du, wie man **Bibliotheken verwendet**, **Daten speichert** und **Verzeichnisse per Code verwaltet**. Ein Blick auf **MicroPython-spezifische Funktionen** rundet das Kapitel ab.

---

## 📊 Was zeichnet eine Programmiersprache aus?

Eine Programmiersprache ist ein Werkzeug, das es uns ermöglicht, Anweisungen an einen Computer zu geben, um bestimmte Aufgaben zu erfüllen. Programmiersprachen wie Python, PHP, Java oder JavaScript ermöglichen es, logische Abläufe zu erstellen (notwendig sind hierfür **Variablen**), Entscheidungen zu treffen (z. B. durch **bedingte Anweisungen**), wiederholende Aufgaben durchzuführen (z. B. mittels **Schleifen**) und Daten zu **verarbeiten** und zu **speichern**.

Im Gegensatz dazu sind Nicht-Programmiersprachen wie HTML, CSS oder Markdown statisch und deklarativ. Sie beschreiben, wie etwas dargestellt wird, aber sie enthalten keine Logik oder Anweisungen zur Verarbeitung von Daten. HTML zum Beispiel dient zur Strukturierung von Inhalten auf einer Webseite, aber es führt keine Berechnungen durch und trifft keine Entscheidungen.

**Beispiele für Programmiersprachen**

- Python
- PHP
- Java
- JavaScript

**Beispiele für Nicht-Programmiersprachen**

- HTML (HyperText Markup Language)
- CSS (Cascading Style Sheets)
- Markdown


## 🛠️ Hilfsmittel für eine effiziente Programmierung

Bisher haben wir mit Thonny gearbeitet. Aber nun möchte ich Ihnen zwei andere, sehr gute Entwicklungsumgebungen empfehlen. Damit können Sie noch effizienter arbeiten und haben nach einer kleinen Eingewöhnungszeit echte Vorteile, zumal gerade Visual Studio auch in etlichen anderen Lehrveranstaltungen genutzt werden kann (oder anders gesagt: irgendwann kommen Sie sowieso nicht drunm herum).


??? info "Visual Studio statt Thonny"

    Um von Thonny zu Visual Studio Code (VS Code) für die Programmierung des Raspberry Pi Pico mit MicroPython zu wechseln, folgen Sie diesen Schritten:

    1. **VS Code installieren**: [Visual Studio Code Download](https://code.visualstudio.com/download).

    2. **Pico-W-Go-Erweiterung in VS Code installieren**

        - Öffnen Sie VS Code.

        - Klicken Sie auf Erweiterungen (linke Leiste unteres Symbol mit 3+1 Vierecke).

        - Suchen Sie nach "Pico-W-Go" und installieren Sie die Erweiterung.

    3. **Projektordner einrichten**

        - Öffnen Sie den Ordner in dem die bisherigen .py-Dateien liegen oder erstellen Sie einen neuen Ordner für Ihr Projekt.
        
        - Öffnen Sie diesen Ordner in VS Code über `Datei` > `Ordner öffnen`.

    4. **Verbindung zum Raspberry Pi Pico herstellen**

        - Pi Pico mit dem Computer verbinden.

        - Pico-W-Go sollte den Pico automatisch erkennen und eine Verbindung herstellen: unten rechts muss dann ein Haken sein.

    5. **Code auf den Pico hochladen und ausführen**: Klicken Sie mit der rechten Maustaste auf die Datei und wählen Sie "Pi-W-Go > Upload project", um den Code auf den Pico zu übertragen.

    6. **Weitere Ressourcen**: Run-Button unten links benutzen.

    Hier der Link zur [offizielle Dokumentation von Pico-W-Go](https://pico-go.net/docs/start/quick/).


??? info "PyCharm statt Thonny"

    Anleitungen auf der [offiziellen Dokumentation von MicroPython](https://docs.micropython.org/). Ich habe es bei mir nicht zum Laufen bekommen.

    Um von Thonny zu PyCharm für die Programmierung des Raspberry Pi Pico mit MicroPython zu wechseln, folgen Sie diesen Schritten:

    1. **PyCharm installieren**: [PyCharm Community Edition Download](https://www.jetbrains.com/pycharm/download/). Pycharm ist für Studierende kostenlos.

    2. **MicroPython-Plugin in PyCharm installieren**:

        - Öffnen Sie PyCharm.

        - Gehen Sie zu `Datei` > `Einstellungen` (oder `PyCharm` > `Einstellungen` auf macOS).

        - Wählen Sie im linken Menü `Plugins` aus.

        - Suchen Sie im Marketplace nach "MicroPython" und installieren Sie das Plugin.

        - Starten Sie PyCharm neu, um die Installation abzuschließen.

    3. **Projektordner einrichten**:

        - Öffnen Sie den Ordner, in dem die bisherigen `.py`-Dateien liegen, oder erstellen Sie einen neuen Ordner für Ihr Projekt.

        - Öffnen Sie diesen Ordner in PyCharm über `Datei` > `Ordner öffnen`.

    4. **MicroPython-Unterstützung im Projekt aktivieren**

        - Gehen Sie zu `Datei` > `Einstellungen` > `Sprachen & Frameworks` > `MicroPython`.

        - Aktivieren Sie das Kontrollkästchen `MicroPython-Unterstützung aktivieren`.

        -...

    5. **Code auf den Pico hochladen und ausführen**:

        - Klicken Sie mit der rechten Maustaste auf die Datei und wählen Sie `Run 'Flash <Dateiname>'`, um den Code auf den Pico zu übertragen.

        - Die Konsole zeigt den Fortschritt des Uploads und eventuelle Ausgaben Ihres Programms an.

### Python Online-Interpreter

- [https://www.w3schools.com/python/trypython.asp?filename=demo_compiler](https://www.w3schools.com/python/trypython.asp?filename=demo_compiler)

- [https://www.online-python.com/](https://www.online-python.com/) 





