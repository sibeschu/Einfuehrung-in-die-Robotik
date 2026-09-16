# Aufgaben Praktikum 1 - Python
Lege im Ordner "Praktikum_1" für jede Aufgabe eine eigene Pythondatei an. Zum Beispiel `aufgabe_1.py` für die Aufgabe 1.

## Aufgabe 1 - Datei anlegen
- Öffne das Terminal mit <kbd>Strg</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd>. 
- Du solltest nun eine Prompt sehen die sich so zusammensetzt: `Nutzername` `@` `Computername` `:` `Ordner/Verzeichnis` `$`. 
( ~/Tilde ist dabei das /home/Nutzer/ Verzeichnis )
#### Teilaufgabe 1.1
- Zeige das aktuelle Verzeichnis an in dem du `pwd` in die Prompt eingibst und absendest.
( Erwartet: /home/{Nutzername} )
#### Teilaufgabe 1.2
- Lege in deinem Homeordner einen Ordner für deine Gruppe an, indem du den Befehl `mkdir {Ordnername}` verwendest.
#### Teilaufgabe 1.3
- Prüfe ob der Ordner angelegt wurde indem du mit `ls` das aktuelle Verzeichnis auflisten lässt.
#### Teilaufgabe 1.4
<kbd>Tab</kbd><kbd>Tab</kbd> ist die automatische Vervollständigung im Terminal, probiere sie bei dieser Aufgabe aus, indem du nach den ersten zwei Buchstaben des Ordnernamens <kbd>Tab</kbd><kbd>Tab</kbd> drückst.
- Wechsle vom $HOME-Verzeichnis in den frisch angelegten Ordner indem du den Befehl `cd {Ordnername}` nutzt.
#### Teilaufgabe 1.5
- Nutze nun den Befehl `git clone https://github.com/sibeschu/Einfuehrung-in-die-Robotik` um den Praktikumsordner von Github in dein Verzeichnis zu kopieren. 

[Linux command line for beginners (ubuntu.com)](https://ubuntu.com/tutorials/command-line-for-beginners#3-opening-a-terminal)

## Aufgabe 2 - Hallo Welt!
- Wechsle (`cd`) in das Verzeichnis /Einfuehrung_Robotik/Praktikum_1 und lege eine Datei an mit dem Namen `aufgabe_hello.py` ( `touch {Dateiname}` )
- Öffne die Datei mit VS Code ( `code {Dateiname}` )
- Schreibe `print("Hello python!")` in die Datei und speichere sie
- Führe nun die Datei aus indem du im Terminal `python3 aufgabe_2.py` eingibst

## Aufgabe 3 - "Hallo Welt"-String
- Lege eine Variable an, die den String "Hello" enthält.
- Lege eine Variable an, die den String "World!" enthält.
- Nutze die Printfunktion um mithilfe der Variablen "Hello World!" auszugeben.

## Aufgabe 4 - Zinssatz
$K_n = K_0 ( 1 + \frac{p}{100})^n$

$K_0$ - aktuelles Anfangskapital in Euro
$p$ - Zinssatz in %
$n$ - Anzahl der Jahre


- Lege eine Datei `aufgabe_zins.py`an
- Schreibe ein Programm, welches das Anfangskapital, den Zinssatz und die Anzahl der Jahre als Input nimmt und das Endkapital ausgibt.
- für die Eingabe von Variablen verwende `Variable_a = input()`
- für das Potenzieren kann die Funktion Math.pow(a, b) aus dem Modul `math`benutzt werden.

_Testbeispiele:_
$ K_0 = 1000.00, n = 5, p = 2.0 \qquad => K_5 = 1104.08 $
$ K_0 = 1000.00, n = 5, p = −2.0 \quad => K_5 = 903.92 $

## Aufgabe 5 - Quadratische Gleichung
$ax^2 + bx + c = 0$

 Nullstellen über:
$x_1,_2 = \frac{-b \; \pm \; \sqrt{b^2 - 4ac} }{2a}$


- Erstelle eine Datei `aufgabe_quad.py`
- Lese drei Zahlen a, b und c ein
- Die Nullstellen sollen auf 4 Nachkommastellen genau ausgegeben werden
- **_Tipp:_** Erst feste Werte für a, b und c verwenden spart Zeit beim Testen, später kann man diese auf input() umstellen
- Erstelle zwei Testbeispiele und dokumentiere die Ergebnisse

## Aufgabe 6 - Modulo
- Lege eine Datei mit dem Namen `aufgabe_modulo.py` an
- Recherchiere die Verwendung des Modulo-Operators in Python  z.B. [Modulo operator (%) in Python (geeksforgeeks.org)](https://www.geeksforgeeks.org/python/what-is-a-modulo-operator-in-python/)
- Schreibe ein Programm welches eine Zahl als Nutzereingabe nimmt und über eine Printfunktion ausgibt, ob diese gerade oder ungerade ist
- **_Tipp:_** if-else Anweisung mit Vergleich auf Modulo 2

## Aufgabe 7 - Münzwurf
- Du kannst die Datei `aufgabe_modulo.py` weiterverwenden
- Importiere am Beginn deiner Datei das Modul mit dem Namen "random".
- Recherchiere online, wie man die Funktion randint() vom Modul "random" nutzt. 
- Schreibe mit der Funktion randint() eine zufällige Zahl in eine Variable. Die Zahl soll dabei nur 1 oder 2 betragen.
- Gib nun über die print()-Funktion "Kopf" aus wenn die Zahl gerade ist und "Zahl" wenn sie ungerade ist.

## Aufgabe 8 - Definition mathematische Funktion
$$ 
v = \left\{
\begin{array}{l}
100, \qquad \qquad t < 0\\
100-5t, \qquad 0 \leq t < 20\\
0, \qquad \qquad \quad sonst.
\end{array}
\right.
$$

- Erstelle eine Datei mit dem Namen `aufgabe_mathedef.py`
- Schreibe ein Programm welches if, elif und else nutzt, um für die Eingabewerte t den entsprechenden Wert auszugeben.

_**Tipp (Pseudocode):**_ 
```python
Ausgabe "Temperatur eingeben"

Eingabe Variable t

Wenn t kleiner 0 dann
    Ausgabe v ist 100
oder wenn t größer gleich 0 und kleiner 20
    Ausgabe v ist 100 minus 5 mal t 
sonst
    Ausgabe v ist 0
```