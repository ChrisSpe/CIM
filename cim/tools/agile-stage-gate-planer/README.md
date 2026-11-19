# Agile-Stage-Gate-Planer

**Kursbezug:** CIM Modul 1, Tag 3 – Innovationsprozesse (Agile-Stage-Gate-Hybrid, Cooper 2016; Next-Generation Stage-Gate, Cooper 2014)
**Stand:** 2026-11-18

## Zweck

Ein Projekt im Agile-Stage-Gate-Hybrid aufsetzen und iterativ führen: Gates bleiben Investitionsentscheidungen, innerhalb der Stages wird in Sprints gearbeitet. Mit grafischer Auswertung und Export als Markdown-Projektdokument.

## Bedienung

`index.html` im Browser öffnen. Sieben Bereiche:

1. **Projekt** – Steckbrief, Rollen (Product Owner, Team, Gatekeeper), Sprintlänge, Unsicherheit → Prozessempfehlung
2. **Plan** – Stages mit Ziel, Anzahl Sprints und Budget; Termine werden berechnet. Must-/Should-meet-Kriterien für alle Gates
3. **Hypothesen** – Backlog mit Typ, Stage, Status und Testkriterium; kritische Hypothesen (★) müssen vor dem Gate bestätigt sein
4. **Sprints** – nach jedem Sprint-Review: Ziel, Ergebnis, Feedback, Learnings, Zielerreichung, Zuversicht 1–5, Budget, getestete Hypothesen
5. **Gates** – Must-/Should-meet, Vorschlag und Entscheidung (Go / Hold / Recycle / Pivot / Kill), freigegebene Sprints
6. **Auswertung** – Kennzahlen, Roadmap Plan vs. Ist, Budget je Stage, Hypothesen-Status, Zuversicht über die Sprints, Gate-Scores
7. **Export** – Projektdokument als **PDF** (inkl. aller Diagramme der Auswertung) oder als `.md` mit Mermaid-Roadmap (Gantt) und Hypothesen-Diagramm

„Beispiel laden“ füllt ein Demo-Projekt, um die Auswertung zu sehen.

## Speichern & Weiterarbeiten

- Der Stand bleibt im Browser gespeichert (localStorage).
- **Projekt speichern (.json)** sichert die Projektdatei.
- **Projekt laden** akzeptiert `.json` und auch ein exportiertes `.md` – die Daten stecken unsichtbar als Kommentar im Dokument.

## Entscheidungslogik (Vorschlag)

| Situation | Vorschlag |
|---|---|
| Must-meet „Nein“ | Kill |
| kritische Hypothese der Stage verworfen | Pivot |
| Must-meet offen | Hold |
| kritische Hypothese noch offen / in Test | Recycle (weitere Sprints) |
| Score ≥ 70 % | Go |
| Score 50–69 % | Recycle |
| Score < 50 % | Kill |

Schwellen und Regeln sind eigene Setzungen, nicht aus dem Kurs. Entscheiden tun die Gatekeeper.
