# Stage-Gate-Assistent

**Kursbezug:** CIM Modul 1, Tag 3 – Innovationsprozesse und Innovationskultur (Dr. Frederik Maibaum)
**Stand:** 2026-11-18

## Zweck

Führt durch ein Gate-Meeting nach dem Stage-Gate-Modell von Cooper (1990, 2008) und erzeugt daraus ein Gate-Protokoll als Markdown-Datei.

## Bedienung

`index.html` im Browser öffnen (keine Installation nötig). Sechs Schritte:

1. **Projekt** – Stammdaten, TRL, Unsicherheit Technik/Markt → Prozessempfehlung
2. **Gate & Deliverables** – Gate 1–5 oder Post-Launch-Review; gate-spezifische Deliverables
3. **Must-meet** – K.-o.-Kriterien (Ja / Nein / Offen)
4. **Should-meet** – gewichtetes Scoring 1–5, Gewichte anpassbar
5. **Entscheidung** – Vorschlag Go / Kill / Hold / Recycle, Gatekeeper-Entscheidung, Maßnahmen, nächster Termin
6. **Dokument** – Vorschau, Download `.md`, Kopieren

Eingaben werden als Entwurf im Browser (localStorage) gehalten.

## Alte Projekte laden & weiterführen

- **Projekt laden (.md / .json)** liest ein früher erzeugtes Gate-Protokoll ein. Neue Protokolle enthalten die Daten unsichtbar als Kommentar; ältere Protokolle ohne diesen Kommentar werden aus den Tabellen und Abschnitten rekonstruiert (bitte kurz prüfen).
- **Projekt speichern (.json)** sichert den Stand als Datei.
- **Nächstes Gate vorbereiten** übernimmt Projektdaten und offene Maßnahmen, setzt Bewertung und Entscheidung zurück und hängt das abgeschlossene Gate an die Historie („Bisherige Gates“ im Protokoll).

## Entscheidungslogik (Vorschlag)

- Ein Must-meet „Nein“ → **Kill** (Recycle, falls behebbar)
- Ein Must-meet „Offen“ → **Hold**
- Score ≥ 70 % → **Go**, 50–69 % → **Recycle / Hold**, < 50 % → **Kill**

Die Schwellen sind eigene Setzungen, nicht aus dem Kurs. Die Entscheidung treffen die Gatekeeper.

## Prozesswahl (aus dem Kurs)

| Unsicherheit | Empfehlung |
|---|---|
| gering | klassisches Stage-Gate |
| Technik hoch | Stage-Gate mit TRL-Gates |
| Markt hoch | Design Thinking / Lean Startup |
| beides hoch | Hybrid mit Effectuation-Logik |

## Ausgabe

`gate-protokoll_<projekt>_<gate>_<datum>.md` mit Stammdaten, Entscheidung, Prozesswahl, Deliverables, Kriterientabellen, Score, Maßnahmen und nächstem Termin.
