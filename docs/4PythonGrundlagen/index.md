# 4 Python Grundlagen

## Gliederung

[4.1 Syntax und Variablen](4.1SyntaxUndVariablen.md)<br>
[4.2 Schleifen](4.2Schleifen.md)<br>
[4.3 Bedingte Anweisungen](4.3BedingteAnweisungen.md)<br>
[4.4 Ein- und Ausgabe](4.4EinUndAusabe.md)<br>
[4.5 Funktionen, Klassen und Methoden](4.5FunktionenKlassenMethoden.md)<br>
[4.6 Bibliotheken](4.6Bibliotheken.md)<br>
[4.7 Daten speichern](4.7DatenSpeichern.md)<br>
[4.8 Übersicht MicroPython-spezifische Funktionen](4.8UebersichtMicroPythonSpezifischeFunktionen.md)<br>


## Generelles Vorgehen in diesem Kapitel

In diesem Kapitel werden wir uns systematisch mit den **grundlegenden Konzepten der Programmierung** am Beispiel von Python bzw. MicoPython vertraut machen. Die gewählte Kapitelstruktur bildet eine Metaebene, die Ihnen hilft, die Kernprinzipien einer Programmiersprache strukturiert zu erlernen und zu verstehen.

### Wie wir vorgehen

Unsere Reise durch die Python-Grundlagen beginnt mit den wesentlichen Bausteinen, auf denen alle Programme aufbauen: der **Syntax und den Variablen** (Kapitel 4.1). Hier lernen Sie, wie Daten in einem Programm zur weiteren Verarbeitung zwischengespeichert werden können.

Im nächsten Schritt untersuchen wir die **Schleifen** (Kapitel 4.2), die es ermöglichen, Anweisungen mehrfach auszuführen. Schleifen sind ein zentrales Element jeder Programmiersprache, da sie es ermöglichen, wiederkehrende Aufgaben effizient zu bewältigen.

Danach beschäftigen wir uns mit den **Bedingten Anweisungen** (Kapitel 4.3), die es dem Programm ermöglichen, Entscheidungen zu treffen und verschiedene Pfade basierend auf bestimmten Bedingungen zu verfolgen. Bedingte Anweisungen sind in jeder Programmiersprache unverzichtbar, um komplexe Entscheidungslogiken zu realisieren.

Anschließend betrachten wir die **Ein- und Ausgabe** (Kapitel 4.4), ein zentraler Aspekt jeder Programmiersprache. Hier erfahren Sie, wie Programme mit der Außenwelt interagieren, sei es durch das Erfassen von Benutzereingaben oder das Anzeigen von Ergebnissen.

Ein weiteres zentrales Thema sind **Funktionen, Klassen und Methoden** (Kapitel 4.5). Diese Konzepte ermöglichen die Strukturierung und Wiederverwendung von Code, was die Effizienz und Lesbarkeit Ihrer Programme erheblich verbessert.

Im Kapitel **Bibliotheken** (Kapitel 4.6) lernen Sie, wie Sie wiederverwendbare Code-Bausteine in Bibliotheken auslagern und in Ihren Projekten verwenden können. Sie erstellen eine eigene Bibliothek und erfahren, wie Sie externe Bibliotheken einbinden.

Im Kapitel **Daten speichern** (Kapitel 4.7) lernen Sie, wie Sie Daten dauerhaft speichern und verwalten können, was insbesondere für Anwendungen wichtig ist, die Informationen über einen längeren Zeitraum hinweg benötigen.

Abschließend erhalten Sie in **MicroPython-spezifische Funktionen** (Kapitel 4.8) eine Übersicht über die Besonderheiten und spezifischen Funktionen von MicroPython, die für die Arbeit mit Hardware und eingebetteten Systemen relevant sind.



### Was zeichnet eine Programmiersprache aus?

Eine Programmiersprache ist ein Werkzeug, das es uns ermöglicht, Anweisungen an einen Computer zu geben, um bestimmte Aufgaben zu erfüllen. Programmiersprachen wie Python, PHP, Java oder JavaScript ermöglichen es, logische Abläufe zu erstellen (notwendig sind hierfür **Variablen**), Entscheidungen zu treffen (z.B. durch **bedingte Anweisungen**), wiederholende Aufgaben durchzuführen (z.B. mittels **Schleifen**) und Daten zu **verarbeiten** und zu **speichern**. 

Im Gegensatz dazu sind Nicht-Programmiersprachen wie HTML, CSS oder Markdown statisch und deklarativ. Sie beschreiben, wie etwas dargestellt wird, aber sie enthalten keine Logik oder Anweisungen zur Verarbeitung von Daten. HTML, zum Beispiel, dient zur Strukturierung von Inhalten auf einer Webseite, aber es führt keine Berechnungen durch und trifft keine Entscheidungen.

**Beispiele für Programmiersprachen**:
- Python
- PHP
- Java
- JavaScript

**Beispiele für Nicht-Programmiersprachen**:
- HTML (HyperText Markup Language)
- CSS (Cascading Style Sheets)
- Markdown
