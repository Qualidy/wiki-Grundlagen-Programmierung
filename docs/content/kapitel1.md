# Kapitel 1 – Programmiersprachen im Überblick

<div class="kurs-progress">
  <div class="step active"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
</div>

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was Programmiersprachen sind und wozu sie dienen
- Wie Programmiersprachen nach Paradigmen unterschieden werden (imperativ, objektorientiert, funktional, skriptbasiert)
- Welche typischen Einsatzszenarien es gibt
- Was der Unterschied zwischen Compiler- und Interpreter-Sprachen ist
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und präge dir die Kernbegriffe ein.
2. Bearbeite die **Kurzübungen** der Reihe nach – von Grundlagen bis Experte.
3. Arbeite die **Workshop-Aufgabe** durch. Sie vertieft das Gelernte an einem zusammenhängenden Szenario.

---

## 1.1 Was ist eine Programmiersprache?

Eine **Programmiersprache** ist eine formale Sprache, mit der Menschen einem Computer Anweisungen erteilen können. Computer selbst verstehen nur Maschinencode – Folgen von Nullen und Einsen. Programmiersprachen dienen als Brücke: Der Mensch schreibt lesbaren Quellcode, der anschließend in Maschinencode übersetzt wird.

Jede Programmiersprache besitzt eine **Syntax** (Grammatikregeln) und eine **Semantik** (Bedeutung der Anweisungen). Wer eine Programmiersprache beherrscht, kann damit Probleme in eine Abfolge präziser Anweisungen zerlegen – das nennt man **algorithmisches Denken**.

!!! info "Warum so viele Sprachen?"
    Es gibt heute über 700 aktiv genutzte Programmiersprachen. Jede entstand, weil bestehende Sprachen für bestimmte Anwendungsfälle ungeeignet waren – zu langsam, zu komplex, zu fehleranfällig oder einfach nicht vorhanden.

---

## 1.2 Programmierparadigmen

Ein **Paradigma** ist eine grundlegende Denkweise, nach der ein Programm aufgebaut wird. Die wichtigsten Paradigmen im Überblick:

### Imperatives Paradigma

Das Programm beschreibt **wie** etwas getan werden soll – Schritt für Schritt, in einer festen Reihenfolge. Der Programmablauf wird durch Anweisungen, Schleifen und Bedingungen gesteuert.

**Beispiele:** C, Pascal, frühe Versionen von BASIC

**Typischer Einsatz:** Systemnahe Programmierung, Mikrocontroller, Algorithmen

### Objektorientiertes Paradigma (OOP)

Das Programm wird als Zusammenspiel von **Objekten** modelliert. Jedes Objekt hat Eigenschaften (Attribute) und Fähigkeiten (Methoden). Objekte kommunizieren miteinander über Nachrichten (Methodenaufrufe).

**Beispiele:** Java, C#, Python, PHP (ab Version 5), Ruby

**Typischer Einsatz:** Unternehmensanwendungen, Desktop-Software, Web-Backends

| Konzept | Erklärung | Beispiel |
|---|---|---|
| Klasse | Bauplan für Objekte | `Klasse Auto` |
| Objekt | Konkretes Exemplar einer Klasse | `meinAuto` |
| Attribut | Eigenschaft eines Objekts | `Farbe = rot` |
| Methode | Funktion, die zu einem Objekt gehört | `fahren()` |
| Vererbung | Eine Klasse übernimmt Eigenschaften einer anderen | `Elektroauto` erbt von `Auto` |

### Funktionales Paradigma

Das Programm besteht aus **mathematischen Funktionen**, die Eingaben auf Ausgaben abbilden. Es gibt keine Zustände und keine Seiteneffekte – eine Funktion liefert bei gleicher Eingabe immer dasselbe Ergebnis.

**Beispiele:** Haskell, Erlang, Elixir; funktionale Elemente auch in JavaScript, Python, Scala

**Typischer Einsatz:** Datenverarbeitung, parallele Berechnungen, kritische Systeme

### Skriptbasiertes Paradigma

Skriptsprachen sind darauf ausgelegt, **bestehende Systeme zu steuern oder zu automatisieren**. Sie werden meist nicht kompiliert, sondern direkt ausgeführt. Oft werden sie in Kombination mit anderen Sprachen eingesetzt.

**Beispiele:** PHP, JavaScript, Python, Bash, PowerShell

**Typischer Einsatz:** Webentwicklung, Systemautomatisierung, Dateiverarbeitung, Glue-Code

!!! tip "Paradigmen schließen sich nicht aus"
    Viele moderne Sprachen unterstützen mehrere Paradigmen. PHP z. B. ist skriptbasiert und gleichzeitig objektorientiert. Python wird imperativ, objektorientiert und funktional eingesetzt.

---

## 1.3 Einsatzszenarien

Welche Sprache wählt man für welches Projekt? Eine Orientierung:

| Einsatzbereich | Typische Sprachen | Begründung |
|---|---|---|
| Webentwicklung (Frontend) | JavaScript, TypeScript | Laufen direkt im Browser |
| Webentwicklung (Backend) | PHP, Python, Java, Node.js | Serverseitige Logik, Datenbankzugriff |
| Mobile Apps | Swift (iOS), Kotlin (Android), Flutter | Native Performance oder plattformübergreifend |
| Desktop-Software | C#, Java, C++ | Zugriff auf Betriebssystem-Ressourcen |
| Datenwissenschaft / KI | Python, R | Umfangreiche Bibliotheken (NumPy, pandas, TensorFlow) |
| Systemsoftware / Treiber | C, C++, Rust | Direkter Hardwarezugriff, maximale Performance |
| Automatisierung / Scripting | Bash, PowerShell, Python | Schnelle Ausführung, kein Build-Schritt nötig |
| Datenbanken | SQL | Deklarative Abfrage- und Manipulation von Daten |

---

## 1.4 Compiler vs. Interpreter

Der wesentliche technische Unterschied zwischen Programmiersprachen liegt darin, **wie Quellcode ausgeführt wird**.

### Compiler-Sprachen

Ein **Compiler** übersetzt den gesamten Quellcode **vor der Ausführung** in Maschinencode (oder Bytecode). Das Ergebnis ist eine ausführbare Datei, die ohne den Compiler läuft.

```
Quellcode → [Compiler] → ausführbare Datei → Ausführung
```

**Vorteile:** Sehr schnell in der Ausführung, Fehler werden vor dem Start erkannt  
**Nachteile:** Übersetzungsschritt nötig, für jede Plattform neu compilieren  
**Beispiele:** C, C++, Rust, Go, Java (zu Bytecode), C#

### Interpreter-Sprachen

Ein **Interpreter** liest den Quellcode **Zeile für Zeile** und führt ihn direkt aus – ohne vorherige Kompilierung.

```
Quellcode → [Interpreter] → direkte Ausführung (Zeile für Zeile)
```

**Vorteile:** Keine Build-Phase, plattformunabhängig, leicht testbar  
**Nachteile:** Langsamer, Fehler treten erst zur Laufzeit auf  
**Beispiele:** PHP, Python, JavaScript (im Browser), Ruby, Bash

### Hybride Ansätze

Manche Sprachen kombinieren beide Ansätze:

- **Java** compiliert zu Bytecode, der dann von der Java Virtual Machine (JVM) interpretiert wird
- **Python** compiliert intern zu `.pyc`-Bytecode, bevor der Interpreter diesen ausführt

| Merkmal | Compiler | Interpreter |
|---|---|---|
| Übersetzungszeitpunkt | Vor der Ausführung | Zur Laufzeit |
| Ausführungsgeschwindigkeit | Schneller | Langsamer |
| Fehlerkennung | Beim Kompilieren | Erst bei Ausführung |
| Typische Sprachen | C, C++, Rust, Go | PHP, Python, JavaScript |
| Build-Schritt nötig? | Ja | Nein |

!!! warning "Fehlerzeitpunkt ist prüfungsrelevant"
    Ein häufiger Prüfungspunkt: Bei Compiler-Sprachen werden Syntaxfehler **vor** der Ausführung erkannt. Bei Interpreter-Sprachen **erst beim Ausführen** der betreffenden Zeile.

---

## Kurzübungen

{{ task(file="tasks/tag1_01.yaml") }}

{{ task(file="tasks/tag1_02.yaml") }}

{{ task(file="tasks/tag1_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k1.yaml") }}
