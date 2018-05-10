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

  * a) Erstelle den Ordner ordner001
  * b) Kopiere die Datei datei001 in ordner001
  * c) Erstelle die Ordner ordner002 bis ordner006 mit einem Befehl
  * d) Kopiere den Ordner ordner005 in den ordner006
  * e) Kopiere alle Dateien die mit datei00 anfangen in den ordner002
  * f) Kopieren alle Dateien die mit einer 1 enden in den Ordner ordner003
  
  Überprüfe deine Ergebnisse in dem du dir den Inhalt des Ordners mit ls anzeigen lässt
  
Aufgabe 2:

  * a) Verschiebe die Dateien datei020 bis datei030 in den ordner001 
  * b) Verschiebe den Ordner ordner005 in den Ordner ordner002
  * c) Benenne die Datei datei023 in datei123 um
  * d) Liste alle Dateien die mit einer 02 anfagen
  * e) Entferne die Dateien datei003 bis datei005 und den Ordner ordner002 in einem Befehl
  
Aufgabe 3:

  * a) Erstelle die Dateien datei001 bis datei300
  * b) Schreibe "Hello World" mit Hilfe des nano Editors in die Datei datei001
  * c) Schreibe "Windows Sucks" in die Datei datei002 mit Hilfe des echo Befehls
  * d) Überschreibe den Inhalt der Datei datei002 mit "Hello" mit Hilfe des echo Befehls
  * e) Füge den Inhalt von datei001 und 002 zu einer neuen Datei datei_neu zusammen
  * f) Suche im Repository nach dem Inhalt "Hello World" in allen Ordnern und zeige die Zeilennummern an
  
Aufgabe 4:

  * a) Schreibe ein kleines Bash Script welches 50 Dateien erstellt, diese im Ordner listet und schließend löscht
  * b) Ergänze das Script so, dass es nicht mehr mit "bash [SCRIPTNAME]" ausgeführt werden muss (ausführbar machen)


Lösungen Aufgabe 1:

  * a) mkdir ordner001
  * b) cp datei001 ordner001
  * c) mkdir ordner{002..004}
  * d) cp -r ordner005 ordner006
  * e) cp datei00* ordner002
  * f) cp datei*1 ordner003

Lösungen Aufgabe 2:
  * a) mv datei{020..030} ordner001
  * b) mv -r ordner005 ordner002
  * c) mv datei023 datei123
  * d) ls datei02*
  * e) rm datei{002..005} -r ordner002

Lösungen Aufgabe 3:
  * a) touch datei{001..300}
  * b) nano datei001, "Hello World" ergänzen, Strg+O zum speichern, mit Enter bestätigen, mit Strg+X nano verlassen 
  * c) echo 'Windows Sucks' >> datei002
  * d) echo 'Hello' > datei002
  * e) cat datei001 datei002 > datei_neu
  * f) grep 'hello world' -rn *

Lösungen Aufgabe 4:
  * a) touch script | echo '#!/usr/bin/bash \ntouch datei{01..50} \nls \nrm datei*' > script, ausführen mit "bash script"
  * b) chmod u+x script, mit ./script ausführen