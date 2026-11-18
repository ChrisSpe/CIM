# Berufliche Entwicklung – Tools & Material

Sammlung eigener Tools und Unterlagen aus Weiterbildungen und Projekten.

## Struktur

```
.
├── cim/                      CIM-Fortbildung (RUB-Akademie)
│   ├── README.md             Übersicht aller CIM-Tools
│   ├── _vorlage-tool/        Vorlage für neue Tools (kopieren & umbenennen)
│   └── tools/
│       ├── stage-gate-assistent/
│       └── agile-stage-gate-planer/
└── README.md
```

Weitere Kurse oder Themen bekommen einen eigenen Ordner auf oberster Ebene (z. B. `ki-strategie/`).

## Konventionen

- Ein Tool = ein Ordner unter `<kurs>/tools/<tool-name>/` (Kleinbuchstaben, Bindestriche).
- Jedes Tool hat eine `README.md` (Zweck, Kursbezug, Bedienung) und möglichst eine eigenständige `index.html`, die ohne Build im Browser läuft.
- Neues Tool → Eintrag in der Tabelle der jeweiligen Kurs-README.
