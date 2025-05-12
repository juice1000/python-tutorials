# Vorläufige Python-Übungen (Windows)

Diese Übungen bilden das Fundament unseres Workshops und sorgen dafür, dass alle Teilnehmer über ein gemeinsames Basiswissen in Python verfügen. Mit diesem Set an Aufgaben stellen wir sicher, dass jeder Teilnehmende dieselben Grundlagen beherrscht, um im weiteren Verlauf des Kurses effizient und zielgerichtet arbeiten zu können.

---

## Aufgabe 1: Umgebung einrichten

**Task 1.1: Python installieren**

- Windows-Installer von [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/) herunterladen.
- Während der Installation „Add Python to PATH“ aktivieren.
- Überprüfen im PowerShell/Terminal:

  ```powershell
  python --version
  ```

  Erwarten: `Python 3.x.x`

**Task 1.2: VS Code einrichten**

- Windows-Installer von [https://code.visualstudio.com/](https://code.visualstudio.com/) herunterladen und installieren.
- VS Code öffnen, Extensions-Tab öffnen und **Python**-Erweiterung von Microsoft installieren.

**Task 1.3: Erstes Skript ausführen**

- Ordner `C:\Users\<DeinName>\python-exercises` anlegen und in VS Code öffnen.
- Datei `hello.py` mit folgendem Inhalt erstellen:

  ```python
  print("Hallo, Welt!")
  ```

- Im VS Code-Terminal (`Strg+Ö`) ausführen:

  ```powershell
  python hello.py
  ```

- Ausgabe prüfen: `Hallo, Welt!`

---

## Aufgabe 2: Variablen & Datentypen

**Task 2.1: Datei erstellen**

- `types_demo.py` im Projektordner anlegen.

**Task 2.2: Zahlen & Strings**

- In `types_demo.py`:

  ```python
  alter = 30
  preis = 19.99
  name = "Alice"
  print(alter, preis, name)
  ```

- Ausführen: `python types_demo.py`

**Task 2.3: Typ-Überprüfung**

- Ergänzen in `types_demo.py`:

  ```python
  print(type(alter), type(preis), type(name))
  ```

- Erneut ausführen: `python types_demo.py`

---

## Aufgabe 3: Listen & Dictionaries

**Task 3.1: Listen erstellen und bearbeiten**

- Datei `collections_demo.py` erstellen.
- Definition:

  ```python
  zahlen = [10, 20, 30, 40, 50]
  ```

- Füge mit `append(60)` hinzu.
- Entferne mit `remove(30)`.
- Gib mit `print(zahlen[:3])` die ersten drei Elemente aus.

**Task 3.2: Dictionary anlegen und verwenden**

- In derselben Datei:

  ```python
  laender = {
      "DE": "Deutschland",
      "US": "Vereinigte Staaten",
      "JP": "Japan"
  }
  ```

- Lass dir den Wert ausgeben von `laender["US"]`.
- Füge `"FR": "Frankreich"` hinzu.
- Iteriere mit:

  ```python
  for code, name in laender.items():
      print(code, "=", name)
  ```

---

## Aufgabe 4: Schleifen

**Task 4.1: For-Schleife**

- Datei `loops.py` erstellen.
- Schreibe:

  ```python
  for i in range(1, 6):
      print(i)
  ```

- Passe an, damit nur ungerade Zahlen (1,3,5) ausgegeben werden.

**Task 4.2: While-Schleife**

- Ergänze in `loops.py` oder neuer Datei:

  ```python
  count = 5
  while count > 0:
      print(count)
      count -= 1
  ```

- Erweitere, dass nach der Schleife `print("Fertig!")` ausgegeben wird.

**Task 4.3: Verschachtelte Schleifen**

- In `loops.py`:

  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          print(f"{i} × {j} = {i * j}")
  ```

- Modifiziere, um Multiplikationstabelle 1×1 bis 3×3 auszugeben.

---

## Aufgabe 5: Funktionen schreiben

**Task 5.1: Funktion definieren und aufrufen**

- Datei `functions.py` erstellen.
- Schreibe:

  ```python
  def begruessung(name):
      return f"Hallo, {name}!"
  print(begruessung("Maria"))
  ```

**Task 5.2: Docstring & Type Hints**

- Erweitere in `functions.py`:

  ```python
  def begruessung(name):
      """Gibt eine persönliche Begrüßung für den übergebenen Namen zurück."""
      return f"Hallo, {name}!"
  ```

- Füge Typ-Hinweise hinzu:

  ```python
  def begruessung(name: str) -> str:
      """Gibt eine persönliche Begrüßung für den übergebenen Namen zurück."""
      return f"Hallo, {name}!"
  ```

---

## Empfohlene Windows-taugliche Ressourcen

- **Offizielle Python-Doku** (Windows Install-Guide):
  [https://docs.python.org/3/using/windows.html](https://docs.python.org/3/using/windows.html)

- **Automate the Boring Stuff with Python** (Deutsch):
  [https://automatetheboringstuff.com/](https://automatetheboringstuff.com/)

- **Real Python** – Windows-Tutorials:
  [https://realpython.com/](https://realpython.com/)

- **freeCodeCamp** YouTube (Windows-Setup):
  [https://www.youtube.com/freecodecamp](https://www.youtube.com/freecodecamp)

- **Codecademy** – Windows-Umgebung:
  [https://www.codecademy.com/learn/learn-python-3](https://www.codecademy.com/learn/learn-python-3)

- **Buch: „Python Crashkurs“** von Eric Matthes – Kapitel Windows-Installation

Viel Erfolg und Spaß beim Lernen!
