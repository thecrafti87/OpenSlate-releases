# OpenSlate

**Ein Programm für Markdown, PDF und alles Textliche dazwischen — für Windows.**

Aktuelle Version: **1.1.0** · [Installer herunterladen](https://github.com/thecrafti87/OpenSlate-releases/releases/latest)

Dieses Repository ist die Bezugsquelle für die fertigen Installer. Hier liegen die
Releases, aus denen sich auch das eingebaute Auto-Update bedient. Der Quellcode wird
getrennt davon verwaltet.

---

## Wofür ist OpenSlate gedacht?

Der Alltag mit Dokumenten verteilt sich üblicherweise auf mehrere Programme: ein Editor
für Markdown, ein Betrachter für PDFs, ein weiteres Werkzeug, sobald aus dem PDF etwas
herausgelöst, geschwärzt oder zusammengefügt werden soll — und für schnelle Blicke in eine
Konfigurationsdatei wieder etwas anderes.

OpenSlate ist als das eine Programm gedacht, das diese Wege zusammenführt. Es startet
schnell genug, um als Windows-Standardprogramm für `.md`- und `.pdf`-Dateien zu taugen,
und bringt gleichzeitig genug Werkzeug mit, dass man für die üblichen Aufgaben nichts
anderes mehr öffnen muss. Alles läuft dabei lokal auf dem eigenen Rechner: kein Konto,
keine Anmeldung, keine Cloud.

Typische Situationen, für die es gebaut wurde:

- Notizen, Dokumentation und Konzepte in Markdown schreiben — mit einer Vorschau, die auch Formeln, Diagramme und Code richtig darstellt
- Ein PDF lesen und dabei rechts daneben mitschreiben, ohne das Fenster zu wechseln
- Aus einem Vertrag die entscheidenden Stellen markieren und als zitierfähiges Markdown herausziehen
- Seiten aus mehreren PDFs zu einem Dokument zusammenstellen, drehen, aufteilen
- Personenbezogene Angaben vor der Weitergabe **wirklich** schwärzen, nicht nur schwarz übermalen
- Kurz in eine JSON-, YAML- oder CSS-Datei schauen, ohne dafür eine Entwicklungsumgebung zu starten

---

## Funktionsumfang

### Markdown

| Bereich | Was drin ist |
| --- | --- |
| Schreiben | Editor auf Basis von CodeMirror 6, Tabs für mehrere Dokumente, Formatierleiste, Zeilenumbruch, automatisches Speichern auf Wunsch |
| Vorschau | GitHub-Markdown mit Tabellen, Aufgabenlisten und Fußnoten; live, wahlweise geteilt oder allein |
| Formeln | KaTeX, inline `$…$` und als Block `$$…$$` |
| Diagramme | Mermaid — Flussdiagramme, Sequenzen, Gantt und mehr, direkt aus dem Codeblock |
| Code | Syntax-Hervorhebung für über 190 Sprachen |
| Navigation | Gliederungs-Seitenleiste aus den Überschriften, synchrones Scrollen von Editor und Vorschau |
| Suchen | Suchen und Ersetzen mit regulären Ausdrücken |
| Ausgeben | Export als eigenständige HTML-Datei, als PDF, oder direkt drucken |
| Bilder | Aus der Zwischenablage einfügen — wird als Datei neben dem Dokument abgelegt und verlinkt |

### PDF lesen

- Fortlaufende Seitenansicht mit Zoom, „An Breite anpassen" und „Ganze Seite"
- Textebene: markieren und kopieren wie in jedem PDF-Betrachter
- Volltextsuche mit hervorgehobenen Treffern
- Seitenleiste mit Miniaturen und den Lesezeichen des Dokuments
- Lupe, die dem Zeiger folgt (1,5× bis 6×)
- Ansicht drehen, Drucken, passwortgeschützte Dateien nach Eingabe des Passworts

### PDF bearbeiten

| Werkzeug | Was es tut |
| --- | --- |
| Seiten verwalten | Umsortieren per Ziehen, drehen, löschen |
| Zusammenfügen | Weitere PDFs an das offene anhängen |
| Aufteilen | Jede Seite einzeln, alle N Seiten oder nach Bereichen |
| Seiten herauslösen | Auswahl wie `1-3, 7, 12-` als neues Dokument |
| Als Bilder exportieren | PNG oder JPEG mit 96, 150 oder 300 dpi |
| Bilder zu PDF | PNG- und JPEG-Dateien zu einem Dokument zusammenfassen |
| Text als Markdown | Die Textebene als neues Markdown-Dokument öffnen |
| Seitenzahlen | Format, Position, Größe, Startnummer und Seitenbereich frei wählbar |
| Wasserzeichen | Diagonaler Text über ausgewählte Seiten |
| Eigenschaften | Titel, Autor, Thema, Schlagwörter ändern |
| Formulare | Felder ausfüllen und anschließend flach machen |

### Anmerkungen

Markieren in fünf Farben, Notizen und Freihand — auch zum Unterschreiben. Anmerkungen
landen zunächst **nicht** im PDF, sondern in einer Datei daneben; das Original bleibt
unangetastet, bis sie bewusst eingebrannt werden. Die Seitenleiste listet alles nach Seite
auf, ein Klick springt hin.

Aus den Anmerkungen lässt sich ein Markdown-Dokument erzeugen: Markiertes wird zum Zitat,
Notizen werden zum Text, und jede Seite bekommt einen Verweis, der zurück ins PDF an genau
diese Stelle führt.

### Schwärzen, das hält

Ein schwarzes Rechteck über einen Text zu legen, entfernt ihn nicht — er bleibt im PDF
enthalten und lässt sich weiterhin markieren, kopieren und auslesen. OpenSlate baut die
betroffenen Seiten stattdessen als Bild neu auf, mit den schwarzen Flächen bereits darin.
Der ursprüngliche Inhalt landet in der Ausgabe gar nicht erst.

Der Preis dafür: Diese Seiten sind danach Bilder, ihr Text ist nicht mehr durchsuchbar.
Alle übrigen Seiten bleiben unverändert.

### Ausschnitte und Notizen

Mit dem Bereichswerkzeug lässt sich ein Rechteck über eine Seite aufziehen und als Bild
ins Markdown einfügen, in die Zwischenablage legen oder als Datei speichern. Der Ausschnitt
wird dabei mit 200 dpi frisch gerendert und bleibt scharf, unabhängig vom Zoom.

Der Knopf **Notizen** blendet rechts neben dem PDF ein Markdown-Feld ein und schreibt in
`<name>-notizen.md` im Ordner des PDFs. Speichern und Suchen richten sich danach, wo
zuletzt gearbeitet wurde.

### Weitere Formate

Neben Markdown und PDF öffnet OpenSlate txt, json, js, ts, html, css, xml, svg, yaml,
toml, ini, csv, log und weitere Textformate — jeweils mit passender Syntax-Hervorhebung.
Die Vorschau blendet sich dabei automatisch aus.

---

## Installation

1. Unter [Releases](https://github.com/thecrafti87/OpenSlate-releases/releases/latest) die Datei `OpenSlate-Setup-1.1.0.exe` herunterladen
2. Ausführen — die Installation läuft ohne Rückfragen und benötigt **keine** Administratorrechte
3. OpenSlate wird für den angemeldeten Benutzer installiert, samt Verknüpfung im Startmenü und auf dem Schreibtisch

Windows SmartScreen meldet sich beim ersten Start möglicherweise mit „Der Computer wurde
durch Windows geschützt". Das liegt daran, dass der Installer nicht mit einem kostenpflichtigen
Zertifikat signiert ist, nicht an einem Fund. Über „Weitere Informationen" → „Trotzdem
ausführen" geht es weiter.

**Systemvoraussetzungen:** Windows 10 oder 11 (64 Bit). Rund 300 MB Platz auf der Festplatte.

### Als Standardprogramm festlegen

Für `.md`-Dateien:

1. Rechtsklick auf eine `.md`-Datei → „Öffnen mit" → „Andere App auswählen"
2. OpenSlate auswählen, Haken bei „Immer diese App verwenden" setzen

Für `.pdf`-Dateien führt der Weg über die Windows-Einstellungen → Apps → Standard-Apps →
Dateityp `.pdf` → OpenSlate. Edge, Acrobat und andere bleiben über „Öffnen mit" jederzeit
erreichbar.

---

## Updates

OpenSlate prüft kurz nach dem Start, ob hier ein neueres Release liegt. Wird eines
gefunden, fragt das Programm nach — heruntergeladen wird nur nach Bestätigung. Installiert
wird das Update beim Beenden oder auf Wunsch sofort; ungespeicherte Dokumente werden dabei
wie gewohnt abgefragt.

Wer selbst nachsehen möchte: Einstellungen → **Nach Updates suchen**.

Was dabei nach außen geht, ist eine einzelne Anfrage an diese Release-Seite auf GitHub.
Es werden keine Nutzungsdaten, Dateiinhalte oder Kennungen übertragen, und OpenSlate
verbindet sich zu keinem anderen Zweck mit dem Internet.

---

## Rechte und Lizenz

OpenSlate steht unter der **MIT-Lizenz**.

Copyright © 2026 Benjamin Ziemann (BeZi-Film)

Das bedeutet in Kurzform: Das Programm darf kostenlos genutzt, weitergegeben, verändert
und auch kommerziell eingesetzt werden. Einzige Bedingung ist, dass der Urheberrechts- und
Lizenzhinweis bei einer Weitergabe erhalten bleibt.

**Gewährleistungsausschluss:** Die Software wird ohne jede Gewährleistung bereitgestellt.
Eine Haftung für Schäden, die aus ihrer Nutzung entstehen, ist ausgeschlossen, soweit
gesetzlich zulässig. Das betrifft insbesondere die Werkzeuge, die Dateien verändern —
Schwärzen, Seiten löschen, Formulare flach machen und Anmerkungen einbrennen lassen sich
nicht rückgängig machen. Vor solchen Schritten empfiehlt sich eine Sicherungskopie.

**Deine Dokumente bleiben deine.** OpenSlate beansprucht keinerlei Rechte an den Dateien,
die damit geöffnet oder erstellt werden, und überträgt sie nirgendwohin.

### Verwendete Open-Source-Komponenten

Der Installer enthält Komponenten Dritter, deren Urheberrechte bei ihren jeweiligen Autoren
liegen. Alle sind unter Lizenzen veröffentlicht, die Weitergabe und kommerzielle Nutzung
erlauben.

| Komponente | Lizenz | Wofür |
| --- | --- | --- |
| [Electron](https://github.com/electron/electron) | MIT | Programmrahmen (Chromium + Node.js) |
| [electron-updater](https://github.com/electron-userland/electron-builder) | MIT | Auto-Update |
| [CodeMirror 6](https://github.com/codemirror) | MIT | Editor-Kern, Suche, Syntax-Hervorhebung |
| [markdown-it](https://github.com/markdown-it/markdown-it) samt Erweiterungen | MIT, ISC, Unlicense | Markdown-Vorschau, Fußnoten, Aufgabenlisten, Anker |
| [KaTeX](https://github.com/KaTeX/KaTeX) | MIT | Formelsatz |
| [highlight.js](https://github.com/highlightjs/highlight.js) | BSD-3-Clause | Code-Hervorhebung |
| [Mermaid](https://github.com/mermaid-js/mermaid) | MIT | Diagramme aus Text |
| [DOMPurify](https://github.com/cure53/DOMPurify) | MPL-2.0 oder Apache-2.0 | Absicherung der Vorschau |
| [pdf.js](https://github.com/mozilla/pdf.js) | Apache-2.0 | PDF anzeigen und auslesen |
| [pdf-lib](https://github.com/Hopding/pdf-lib) | MIT | PDF bearbeiten |

pdf.js und DOMPurify werden unverändert eingebunden. Eine ausführliche Aufstellung mit
Versionsangaben liegt im Quell-Repository unter `THIRD-PARTY-LICENSES.md`.

---

## Was noch fehlt

Ehrlichkeit vor Werbung — diese Grenzen sind bekannt:

- Kein OCR: Gescannte Seiten ohne Textebene liefern keinen Text
- Keine Komprimierung und keine Passwortvergabe für PDFs
- Verschlüsselte PDFs lassen sich lesen, aber nicht bearbeiten
- Lesezeichen und Formularfelder gehen verloren, sobald Seiten umsortiert oder gelöscht werden
- Keine Umwandlung nach Word, Excel oder PowerPoint
- Nur Windows; macOS und Linux sind nicht vorgesehen

---

## Alle Versionen

Der vollständige Änderungsverlauf steht bei jedem Release unter
[Releases](https://github.com/thecrafti87/OpenSlate-releases/releases).

*Diese Seite gehört zu OpenSlate 1.1.0 und wird mit jeder Veröffentlichung aktualisiert.*
