# linuxtutorial

## Vortrag Outline

* Was ist linux?

1. linux(-kernel) vs. POSIX
![System\"uberblick](https://upload.wikimedia.org/wikipedia/commons/thumb/4/46/Linux_Kernel_Struktur.svg/800px-Linux_Kernel_Struktur.svg.png)

* Was ist Unix?

![History](https://upload.wikimedia.org/wikipedia/commons/7/77/Unix_history-simple.svg)
1. Everything is a file
2. Do One Thing only and do it good.

* Bootvorgang

> systemd-analyze plot > test.svg && firefox test.svg

* Shell

* Desktop

* Was macht eine Distribution aus?

1. Softwareverwaltung (paketmanagement)
2. Grundinstallation
3. Unterst\"utzte Hardware
4. Community (Wiki, Foren, Entwickler, User)
5. Softwaresupport

## Demo zum Mitmachen

Bevor es los geht: 
  Wechsel in dein Home-Verzeichnis: cd 
  Erstelle einen Ordner für github Projekte: mkdir github
  Wechsel in das Repository: cd linuxtutorial
  Clone dieses Repository : git clone https://github.com/jschroeder89/linuxtutorial
  
Aufgabe 1:
  a) Erstelle den Ordner ordner 001
  b) Kopiere die Datei datei001 in ordner001
  c) Erstelle die Ordner ordner002 bis ordner004 mit einem Befehl
  d) Kopiere den Ordner ordner005 in den ordner006
  e) Kopiere alle Dateien die mit datei00 anfangen in den ordner002
  f) Kopieren alle Dateien die mit einer 1 enden in den Ordner ordner003
  
  Überprüfe deine Ergebnisse in dem du dir den Inhalt des Ordners mit ls anzeigen lässt
  
Aufgabe 2:
  a) Verschiebe die Dateien datei020 bis datei030 in den ordner005 
  b) Verschiebe den Ordner ordner005 in den Ordner ordner006
  c) Benenne die Datei datei023 in datei123 um
  d) Liste alle Dateien die mit einer 2 anfagen
  
Aufgabe 3:
  a) Erstelle die Dateien datei001 bis datei300
  b) Schreibe "Hello World" mit Hilfe des nano Editors in die Datei datei001
  c) Schreibe "Windows Sucks" in die Datei datei002 mit Hilfe des echo Befehls
  d) Füge den Inhalt von datei001 und 002 zu einer neuen Datei datei_neu zusammengrep 
  e) Suche im Repository nach dem Inhalt "Hello World" in allen Ordnern und zeige die Zeilennummern an
  
Aufgabe 4:
  a) Schreibe ein kleines Bash Script welches 50 Dateien erstellt, diese im Ordner listet und schließend löscht
  b) Ergänze das Script so, dass es nicht mehr mit "bash [SCRIPTNAME]" ausgeführt werden muss
  c) Mache das Script ausführbar
