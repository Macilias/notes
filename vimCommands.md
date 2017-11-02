Delete all lines in file:

- gg (opt) to move the cursor to the first line
- dG to delete all the lines.

Speichern & Schließen:
:q	vi beenden
:q!	vi beenden, nicht gespeicherte Änderungen gehen verloren
:w	Datei speichern
:w!	Speichern der Datei erzwingen
:wq (oder) ZZ	Datei speichern und vi beenden
<Strg> + z	Shell starten; vi wird in Hintergrund geschoben; Rückkehr durch Eingabe von "fg"
Navigation:
G	an das Ende des Dokuments springen
1G	in die erste Zeile des Dokuments springen
0 (null)	an den Anfang der Zeile springen
^	an den Anfang der Zeile springen
$	an das Ende der Zeile springen
b	an den Anfang des letzten Wortes springen
w	an den Anfang des nächsten Wortes springen
e	an das Ende des nächsten Wortes springen
h	ein Zeichen nach links
j	ein Zeile nach unten
k	eine Zeile nach oben
l	ein Zeichen nach rechts
<Strg> + u	nach oben blättern
<Strg> + d	nach unten blättern
L	in die letzte Zeile der Bildschirmausgabe springen
Löschen:
x	Zeichen unter Cursor-Position löschen
r	Zeichen unter Cursor-Position ersetzen
s	Zeichen unter Cursor-Position ersetzen und in den Bearbeitungsmodus wechseln
dd	aktuelle Zeile ausschneiden (in Zwischenablage kopieren & löschen)
[ZAHL]dd	die nächsten [ZAHL] Zeilen ausschneiden
C	Zeile ab aktueller Cursor-Position löschen
V	Zeile markieren
v	Zeichen markieren
d	markierte Textstellen löschen
cw	aktuelles Wort ersetzen
dw	aktuelles Wort löschen (incl. angehängtem Leerzeichen)
de	aktuelles Wort löschen (über Zeile hinaus)
dl	Zeichen unter Cursor-Position löschen
dj	zwei Zeilen löschen (Cursor-Position ist 1. Zeile)
dk	zwei Zeilen löschen (Cursor-Position ist 2. Zeile)
:5,10d	Zeilen 5 bis 10 löschen
:.,$d	alle Zeilen löschen ("." = Anfang der Datei, "$" = Ende der Datei)
Einfügen:
p	Zwischenablage nach aktueller Zeile einfügen
P	Zwischenablage vor aktueller Zeile einfügen
R	Text ab Cursor-Position überschreiben
J	aktuelle Zeile an das Ende der vorhergehenden Zeile anhängen
o	eine Zeile nach der aktuellen einfügen und in den Bearbeitungsmodus wechseln
O	eine Zeile vor der aktuellen einfügen und in den Bearbeitungsmodus wechseln
a	ein Leerzeichen einfügen und in den Bearbeitungsmodus wechseln
A	zum Ende der Zeile springen und in den Bearbeitungsmodus wechseln
i	in den Bearbeitungsmodus wechseln
I	an den Anfang der Zeile springen und in den Bearbeitungsmodus wechseln
Suchen & Ersetzen:
/Linux	nach "Linux" suchen
/	letzte Suche wiederholen
n	letzte Suche wiederholen
:s/Suchen_nach/Ersetzen_durch/	in aktueller Zeile suchen & ersetzen
:1,7s/Suchen_nach/Ersetzen_durch/	in Zeile 1 bis 7 suchen & ersetzen
:%s/Suchen_nach/Ersetzen_durch/	in allen Zeilen suchen & ersetzen
Sonstiges:
u	UNDO der letzten Befehle
U	alle Änderungen der aktuellen Zeile rückgängig machen