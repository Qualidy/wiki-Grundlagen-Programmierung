# Kapitel 5 – Lasten- und Pflichtenheft

<div class="kurs-progress">
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step active"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
</div>

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was Lastenheft und Pflichtenheft sind und wie sie sich voneinander unterscheiden
- Was Muss-, Kann- und Nicht-Anforderungen bedeuten
- Was Abnahmekriterien sind und warum sie wichtig sind
- Wie beide Dokumente als Brücke zwischen Auftraggeber und Auftragnehmer funktionieren
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und ordne die Konzepte den realen Dokumenten zu.
2. Bearbeite die **Kurzübungen** der Reihe nach – von Grundlagen bis Experte.
3. Arbeite die **Workshop-Aufgabe** durch. Sie vertieft das Gelernte an einem zusammenhängenden Szenario.

---

## 5.1 Einführung: Warum diese Dokumente?

Softwareprojekte scheitern häufig nicht an technischen Problemen, sondern an **Missverständnissen**: Der Auftraggeber hatte eine bestimmte Vorstellung, der Auftragnehmer hat etwas anderes gebaut – und niemand hat es rechtzeitig bemerkt.

**Lastenheft** und **Pflichtenheft** sind die wichtigsten Werkzeuge, um solche Missverständnisse zu vermeiden. Sie schaffen Verbindlichkeit, Klarheit und eine gemeinsame Sprache zwischen allen Beteiligten.

!!! info "Verbindung zu früheren Modulen"
    Lastenheft und Pflichtenheft wurden bereits in den Modulen „IT-Arbeitsplatz" und „Projektplanung" eingeführt. Dieses Kapitel vertieft die Inhalte im Kontext der Softwareentwicklung und ergänzt die Perspektive des Auftragnehmers.

---

## 5.2 Das Lastenheft

Das **Lastenheft** (englisch: *Requirements Document* oder *Customer Requirements*) wird vom **Auftraggeber** erstellt. Es beschreibt aus seiner Sicht, **was** das zu entwickelnde System leisten soll – **ohne** festzulegen, wie es technisch umgesetzt wird.

Das Lastenheft ist die Grundlage für die Ausschreibung. Mehrere Anbieter können auf Basis desselben Lastenhefts Angebote abgeben.

**Typische Inhalte eines Lastenhefts:**

| Abschnitt | Inhalt |
|---|---|
| **Ausgangssituation** | Warum wird das Projekt durchgeführt? Welches Problem soll gelöst werden? |
| **Ziele** | Was soll nach Projektabschluss besser sein? |
| **Funktionale Anforderungen** | Was soll das System tun? (Funktionen, Workflows) |
| **Nicht-funktionale Anforderungen** | Wie soll das System sein? (Geschwindigkeit, Sicherheit, Usability) |
| **Abgrenzung** | Was gehört explizit *nicht* zum Auftragsumfang? |
| **Rahmenbedingungen** | Budget, Zeitplan, Schnittstellen zu bestehenden Systemen |
| **Abnahmekriterien** | Woran erkennt der Auftraggeber, dass das System fertig ist? |

**Wichtige Merkmale:**
- Formuliert in der Sprache des Auftraggebers (nicht-technisch)
- Beschreibt das **Was**, nicht das **Wie**
- Muss vollständig, eindeutig und widerspruchsfrei sein

---

## 5.3 Das Pflichtenheft

Das **Pflichtenheft** (englisch: *Functional Specification* oder *System Specification*) wird vom **Auftragnehmer** erstellt – als Antwort auf das Lastenheft. Es beschreibt, **wie** die Anforderungen des Auftraggebers technisch umgesetzt werden sollen.

Das Pflichtenheft ist die Grundlage des Vertrags. Mit seiner Unterzeichnung verpflichtet sich der Auftragnehmer zur Lieferung des beschriebenen Systems.

**Typische Inhalte eines Pflichtenhefts:**

| Abschnitt | Inhalt |
|---|---|
| **Systemübersicht** | Welche Komponenten hat das System? |
| **Funktionale Spezifikation** | Genaue Beschreibung jeder Funktion |
| **Technische Architektur** | Welche Technologien, Frameworks, Datenbanken? |
| **Schnittstellen** | Wie kommuniziert das System mit anderen Systemen? |
| **Datenbankdesign** | Datenbankstruktur (ER-Modell) |
| **Benutzeroberfläche** | Wireframes, Beschreibung der UI-Elemente |
| **Test- und Abnahmeplan** | Wie wird das System abgenommen? |

**Wichtige Merkmale:**
- Formuliert in der Sprache des Entwicklers (technisch präzise)
- Beschreibt das **Wie**
- Dient als Grundlage für die Implementierung

---

## 5.4 Abgrenzung: Lastenheft vs. Pflichtenheft

| Merkmal | Lastenheft | Pflichtenheft |
|---|---|---|
| **Erstellt von** | Auftraggeber | Auftragnehmer |
| **Inhalt** | Was soll das System leisten? | Wie wird es umgesetzt? |
| **Sprache** | Fachlich, nicht-technisch | Technisch, präzise |
| **Zeitpunkt** | Vor der Ausschreibung | Nach der Angebotsphase |
| **Zweck** | Grundlage für Angebote | Grundlage für Vertrag und Entwicklung |
| **Perspektive** | Außenperspektive (Nutzer) | Innenperspektive (System) |

**Eselsbrücke:** Das Lastenheft beschreibt die **Last** (Aufgabe) des Auftraggebers. Das Pflichtenheft beschreibt die **Pflicht** (Verpflichtung) des Auftragnehmers.

---

## 5.5 Muss-, Kann- und Nicht-Anforderungen

Anforderungen werden nach ihrer Verbindlichkeit in drei Kategorien eingeteilt:

### Muss-Anforderungen

**Muss-Anforderungen** (auch Pflichtanforderungen) sind **unverzichtbar**. Das System gilt als nicht abnahmefähig, wenn auch nur eine Muss-Anforderung nicht erfüllt ist.

> „Das System **muss** Benutzern ermöglichen, ihr Passwort selbst zurückzusetzen."

### Kann-Anforderungen

**Kann-Anforderungen** (auch Wunschanforderungen oder optionale Anforderungen) sind **wünschenswert**, aber nicht zwingend. Werden sie nicht umgesetzt, gilt das System trotzdem als fertig.

> „Das System **kann** eine Zwei-Faktor-Authentifizierung per SMS anbieten."

### Nicht-Anforderungen (Abgrenzung)

**Nicht-Anforderungen** definieren explizit, was das System **nicht** leisten soll. Dies verhindert Scope-Creep (schleichende Ausweitung des Projektumfangs).

> „Das System wird **keine** mobile App bereitstellen. Die Weboberfläche muss jedoch auf mobilen Geräten nutzbar sein."

!!! warning "Eindeutige Formulierung ist entscheidend"
    Vage Formulierungen wie „Das System soll schnell sein" oder „Die Oberfläche soll modern wirken" sind unbrauchbar. Gute Anforderungen sind **messbar und prüfbar**: „Das System muss die Suchanfrage in unter 2 Sekunden beantworten."

---

## 5.6 Abnahmekriterien

**Abnahmekriterien** definieren, wann ein Projekt als erfolgreich abgeschlossen gilt. Sie sind konkret, messbar und aus den Anforderungen abgeleitet.

Ohne Abnahmekriterien entstehen endlose Diskussionen darüber, ob das gelieferte System den Erwartungen entspricht. Mit klar definierten Kriterien ist die Abnahme ein objektiv prüfbarer Vorgang.

**Eigenschaften guter Abnahmekriterien:**

| Eigenschaft | Beispiel |
|---|---|
| **Messbar** | „Der Login-Vorgang dauert maximal 1,5 Sekunden" |
| **Eindeutig** | „Das System exportiert Daten im CSV-Format (UTF-8, Semikolon-getrennt)" |
| **Vollständig** | Alle Muss-Anforderungen haben zugehörige Abnahmekriterien |
| **Testbar** | Ein Testfall kann direkt aus dem Kriterium abgeleitet werden |

**Beispiel – Abnahmekriterien für eine Login-Funktion:**

| # | Anforderung | Abnahmekriterium |
|---|---|---|
| 1 | Benutzer können sich einloggen | Login mit gültigen Zugangsdaten führt zur Startseite |
| 2 | Falsche Passwörter werden abgewiesen | Nach 3 Fehlversuchen wird das Konto für 15 Minuten gesperrt |
| 3 | Passwort zurücksetzen | Passwort-Reset-Link wird an die hinterlegte E-Mail gesendet (≤ 1 Minute) |

---

## 5.7 Typischer Ablauf in der Praxis

```
Auftraggeber                    Auftragnehmer
     │                                │
     ├── Lastenheft erstellen ────────►│
     │                                │
     │◄─── Angebot + Pflichtenheft ───┤
     │                                │
     ├── Pflichtenheft prüfen ─────────►│
     │     und freigeben              │
     │                                │
     │        [Entwicklung]           │
     │                                │
     │◄─── System liefern ────────────┤
     │                                │
     ├── Abnahme anhand               │
     │   der Abnahmekriterien ────────►│
     │                                │
     ├── Abnahmeprotokoll ──────────────►│
```

---

## Kurzübungen

{{ task(file="tasks/tag5_01.yaml") }}

{{ task(file="tasks/tag5_02.yaml") }}

{{ task(file="tasks/tag5_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k5.yaml") }}
