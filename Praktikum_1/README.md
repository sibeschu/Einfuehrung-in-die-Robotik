# Praktikum 1 - Linux & Python

## Linux

### Hotkeys
<kbd>Strg</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd> - Öffnet ein Terminal
<kbd>Strg</kbd> + <kbd>C</kbd> - bricht Prozess ab
<kbd>Strg</kbd> + <kbd>D</kbd> - schließt das Terminal

### Befehle
`pwd`   - print working directory
`ls`    - list
`cd`    - change directory
`mkdir` - make directory
`touch` - make empty file
`rm`    - remove
`mv`    - move
`cp`    - copy
`man`   - manual

## eine Pythondatei ausführen
```bash
python3 Praktikum_1.py
```

## Python keywords
and, as, assert, async, await, break, case, class, continue, def, del, elif, else, except, False, finally, for, from, global, if, import, in, is, lambda, match, None, nonlocal, not, or, pass, raise, return, True, try, while, with, yield
[Was diese Keywords tun.](https://www.w3schools.com/python/python_ref_keywords.asp)


## Kommentare im Quellcode schreiben
```python
# Einzeiler

# mehrere
# Zeilen
```

## Variablen anlegen und zuweisen
```python
a = 1               # Integer
b = 3.4             # Float
c = "Hello World"   # String
d = None            # Empty
```

## Verzweigungen
### if else
```python
a = int(input("Enter an integer: "))

if a == 1:
    print("a is 1")
elif a == 2:
    print("a is 2")
elif a != 2 and a >= 0:
    print("a is not 2 but greater 0")
else:
    print("a is anything else")
```
### for Schleife

```python
a = ['Fischers', 'Fritz', 'fischt', 'frische', 'Fische']

for i in range(len(a)):
    print(i, a[i])
```

### while Schleife

```python
a = 10

while a > 0:
    print("a is greater 0")
    a -= 1
```


```python
i = 1

while True:
    print("loop running")
    i += 1
    if i > 100:
        break
```

## Funktionen

```python
def function(Parameter):
    EXECUTE CODE
    return RESULT
```