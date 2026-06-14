# Kapitel 2 – Arten der Softwareanpassung

<div class="kurs-progress">
  <div class="step done"></div>
  <div class="step active"></div>
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

- Welche fünf Arten der Softwareanpassung es gibt
- Was der Unterschied zwischen Konfiguration, Customizing, Erweiterungen, Individualentwicklung und Refactoring ist
- Wie du für einfache Szenarien die geeignete Anpassungsform bestimmst
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und präge dir die fünf Anpassungsarten ein.
2. Bearbeite die **Kurzübungen** der Reihe nach – von Grundlagen bis Experte.
3. Arbeite die **Workshop-Aufgabe** durch. Sie vertieft das Gelernte an einem zusammenhängenden Szenario.

---

## 2.1 Warum Software angepasst werden muss

Fertige Software deckt selten alle Anforderungen eines Unternehmens ab. Zwischen dem, was ein Standardprodukt bietet, und dem, was ein Unternehmen benötigt, klafft fast immer eine Lücke. Diese Lücke muss geschlossen werden – auf die wirtschaftlichste und technisch sinnvollste Art.

Die Wahl der richtigen Anpassungsform ist keine rein technische, sondern vor allem eine **wirtschaftliche Entscheidung**: Wie viel Aufwand ist gerechtfertigt? Welche Risiken entstehen? Wie wartbar ist das Ergebnis?

---

## 2.2 Konfiguration und Parametrisierung

**Konfiguration** ist die einfachste Form der Anpassung. Die Software selbst wird nicht verändert – stattdessen werden **Einstellungen** geändert, die das Verhalten steuern. Jede Software sieht solche Anpassungspunkte explizit vor.

**Parametrisierung** ist ein Sonderfall: Bestimmte Werte (Parameter) werden beim Start oder in Konfigurationsdateien übergeben und beeinflussen den Ablauf des Programms.

**Typische Beispiele:**
- Sprache und Region eines Betriebssystems einstellen
- E-Mail-Server-Adresse in einem CRM-System hinterlegen
- Mehrwertsteuersatz in einer Buchhaltungssoftware konfigurieren
- Benutzerrechte und Rollen in einem ERP-System vergeben

**Merkmale:**

| Merkmal | Ausprägung |
|---|---|
| Aufwand | Gering |
| Risiko | Sehr gering |
| Reversibilität | Hoch (einfach rückgängig machbar) |
| Technische Kenntnisse | Keine Programmierung nötig |
| Wartung | Unproblematisch (Hersteller-Updates möglich) |

!!! tip "Immer zuerst prüfen"
    Bevor teurere Anpassungsformen gewählt werden, sollte geprüft werden, ob das gewünschte Verhalten bereits durch Konfiguration erreichbar ist.

---

## 2.3 Customizing

**Customizing** geht einen Schritt weiter als Konfiguration. Hier werden **vorgesehene Anpassungsmechanismen** des Systems genutzt, um Prozesse, Oberflächen oder Workflows gezielt auf die Bedürfnisse des Unternehmens zuzuschneiden – ohne den Kern der Software zu verändern.

Bekannte Beispiele sind ERP-Systeme wie SAP oder Microsoft Dynamics, die umfangreiche Customizing-Möglichkeiten bieten: Formulare anpassen, Felder hinzufügen, Prozessschritte ändern.

**Typische Beispiele:**
- Bestellworkflow in einem ERP-System an interne Genehmigungsstufen anpassen
- Benutzeroberfläche eines CRM auf relevante Felder reduzieren
- Berichte und Auswertungen auf das Corporate Design anpassen

**Abgrenzung zur Konfiguration:** Beim Customizing werden oft tabellarische Einträge in internen Customizing-Tabellen vorgenommen oder grafische Tools genutzt – es handelt sich also um strukturierte, aber umfangreichere Einstellungen.

**Merkmale:**

| Merkmal | Ausprägung |
|---|---|
| Aufwand | Mittel |
| Risiko | Gering bis mittel |
| Reversibilität | Mittel |
| Technische Kenntnisse | Systemkenntnis nötig, keine Programmierung |
| Wartung | Ggf. Anpassungen bei Systemupdates nötig |

---

## 2.4 Erweiterungen und Plug-ins

Wenn die vorhandenen Anpassungsmechanismen nicht ausreichen, können **Erweiterungen** (auch Add-ons, Module oder Plug-ins genannt) eingesetzt werden. Diese werden in die bestehende Software integriert und ergänzen deren Funktionsumfang.

Erweiterungen können **von Drittanbietern** bezogen oder **selbst entwickelt** werden. Viele Plattformen (CMS, Shops, IDEs) haben einen eigenen Marktplatz für Erweiterungen.

**Typische Beispiele:**
- WordPress-Plugin für SEO-Analyse installieren
- Browser-Erweiterung für Passwort-Manager
- VSCode-Extension für Python-Entwicklung
- Shopify-App für Buchungskalender

**Merkmale:**

| Merkmal | Ausprägung |
|---|---|
| Aufwand | Mittel (bei fertigen Plug-ins) bis hoch (bei Eigenentwicklung) |
| Risiko | Mittel – Qualität und Sicherheit des Plug-ins beachten |
| Reversibilität | Mittel |
| Technische Kenntnisse | Installation/Konfiguration bis Programmierung |
| Wartung | Abhängigkeit vom Plug-in-Hersteller |

!!! warning "Sicherheitsrisiken bei Drittanbieter-Erweiterungen"
    Jedes Plug-in eines externen Anbieters ist ein potenzielles Sicherheitsrisiko. Es sollte geprüft werden, ob der Anbieter vertrauenswürdig ist und das Plug-in regelmäßig gepflegt wird.

---

## 2.5 Individualentwicklung

**Individualentwicklung** (auch Neuentwicklung oder Eigenentwicklung) bedeutet, dass Software von Grund auf oder als eigenständiges Modul neu entwickelt wird – maßgeschneidert für die spezifischen Anforderungen.

Diese Form kommt zum Einsatz, wenn kein Standardprodukt die Anforderungen erfüllt oder wenn die Integration in bestehende Systeme so komplex ist, dass eine Eigenentwicklung wirtschaftlich sinnvoller ist.

**Typische Beispiele:**
- Entwicklung einer unternehmenseigenen Produktionsverwaltungssoftware
- Maßgeschneiderte Web-App für einen spezifischen Geschäftsprozess
- Integration zweier Systeme über eine selbst entwickelte Schnittstelle (API)

**Merkmale:**

| Merkmal | Ausprägung |
|---|---|
| Aufwand | Hoch bis sehr hoch |
| Risiko | Hoch (Projektrisiken, Budgetüberschreitungen) |
| Reversibilität | Gering – hohe Wechselkosten |
| Technische Kenntnisse | Vollständige Entwicklung nötig |
| Wartung | Vollständige Eigenverantwortung |

---

## 2.6 Refactoring

**Refactoring** ist eine besondere Anpassungsform: Dabei wird bestehender Quellcode **strukturell verbessert**, ohne das äußerliche Verhalten der Software zu ändern. Das Programm tut nach dem Refactoring dasselbe wie vorher – nur der interne Aufbau ist sauberer, lesbarer und wartbarer.

Refactoring ist kein Feature-Entwicklung und kein Bug-Fix. Es ist eine **Investition in die Codequalität**, die zukünftige Änderungen erleichtert.

**Typische Maßnahmen:**
- Lange Funktionen in kleinere, benannte Funktionen aufteilen
- Doppelten Code (Duplikate) in eine gemeinsame Funktion auslagern
- Variablen und Funktionen besser benennen
- Komplexe Bedingungen vereinfachen

**Merkmale:**

| Merkmal | Ausprägung |
|---|---|
| Äußeres Verhalten | Unverändert |
| Ziel | Verbesserte Codequalität, Wartbarkeit |
| Wann? | Regelmäßig, meist vor neuen Features oder nach Fertigstellung |
| Risiko | Gering, wenn gute Tests vorhanden |

---

## 2.7 Entscheidungshilfe: Welche Anpassungsform passt?

```
Kann das gewünschte Verhalten durch
Einstellungen im System erreicht werden?
       │
      Ja ──► Konfiguration / Parametrisierung
       │
      Nein
       │
Gibt es dafür einen vorgesehenen
Customizing-Mechanismus?
       │
      Ja ──► Customizing
       │
      Nein
       │
Gibt es ein fertiges Plug-in oder
eine geeignete Erweiterung?
       │
      Ja ──► Erweiterung / Plug-in
       │
      Nein
       │
Muss die Lösung von Grund auf
neu entwickelt werden?
       │
      Ja ──► Individualentwicklung
```

---

## Kurzübungen

{{ task(file="tasks/tag2_01.yaml") }}

{{ task(file="tasks/tag2_02.yaml") }}

{{ task(file="tasks/tag2_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k2.yaml") }}
