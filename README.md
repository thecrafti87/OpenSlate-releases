# OpenSlate

**Ein Programm für Markdown, PDF und alles Textliche dazwischen — für Windows.**

Vollwertiger Editor, PDF-Werkzeugkasten und Betrachter in einem, mit Menüband,
Befehlspalette und Funktionen, die über einzelne Dokumente hinausreichen.

Aktuelle Version: **1.6.0** · [Installer herunterladen](https://github.com/thecrafti87/OpenSlate-releases/releases/latest)

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
| Navigation | Gliederungs-Seitenleiste aus den Überschriften; Editor und Vorschau scrollen gemeinsam oder getrennt |
| Suchen | Suchen und Ersetzen mit regulären Ausdrücken |
| Ausgeben | Export als eigenständige HTML-Datei, als PDF, oder direkt drucken |
| Bilder | Aus der Zwischenablage einfügen — wird als Datei neben dem Dokument abgelegt und verlinkt |

### Bearbeiten wie in einer Entwicklungsumgebung

Diese Werkzeuge gelten für **jedes** Textformat, nicht nur für Markdown:

| Bereich | Was drin ist |
| --- | --- |
| Cursor | Mehrfach-Cursor (Alt+Klick), Spaltenauswahl (Alt+Ziehen), nächstes Vorkommen auswählen (Strg+D) |
| Zeilen | verschieben (Alt+↑/↓), duplizieren, löschen, verbinden, sortieren, doppelte und leere entfernen |
| Text | Groß-/Kleinschreibung, Leerraum am Zeilenende aufräumen, Kommentar umschalten, ein- und ausrücken |
| Navigation | Gehe zu Zeile (Strg+G), Klammer-Sprung, Code-Faltung |
| Ansicht | Zeilennummern, aktive Zeile, Sonderzeichen, Zeilenumbruch — einzeln schaltbar; Einrückung frei einstellbar |
| Rückgängig | Strg+Z und Strg+Y, mit Knöpfen in der Leiste und im Menü |

**Schreibhilfen:** Enter setzt Listen, Aufgaben und Zitate fort und nummeriert dabei die
folgenden Punkte nach — ein leerer Punkt beendet die Liste. Dazu Wortvervollständigung aus
dem Dokument, paarweise Klammern und eine **Rechtschreibprüfung** mit Korrekturvorschlägen
per Rechtsklick und eigenem Wörterbuch.

### Über Dokumentgrenzen hinweg

- **Strg+Umschalt+F** sucht und ersetzt in **allen offenen Dokumenten oder einem ganzen Ordner**, mit Trefferliste zum Anspringen
- **Zwei Dokumente vergleichen** — Unterschiede nebeneinander, gemeinsam scrollend
- **Geteilte Ansicht** für zwei beliebige Dokumente nebeneinander
- Auswahl in ein anderes Dokument übertragen, mehrere Dateien zu einem zusammenführen

### Damit nichts verloren geht

- Wurde eine geöffnete Datei zwischenzeitlich von einem anderen Programm geändert, fragt OpenSlate nach, statt sie kommentarlos zu überschreiben — ein Warnzeichen am Tab weist darauf hin
- Die zuletzt offenen Dateien kommen beim Start zurück; ein versehentlich geschlossener Tab mit **Strg+Umschalt+T**
- Kodierung und Zeilenenden werden erkannt und lassen sich in der Statusleiste umstellen

### Schneller arbeiten

**Strg+P** (oder **F1**) öffnet die Befehlspalette: ein Suchfeld über der App, in dem sich
jeder Befehl durch Tippen finden lässt. Die Suche ist unscharf und verzeiht Umlaute — „sw"
findet „Schwärzen anwenden", „schwaerzen" ebenso. Angeboten wird nur, was im aktuellen
Dokument möglich ist; zuletzt benutzte Befehle stehen oben, die zuletzt geöffneten Dateien
ebenfalls.

**Editor und Vorschau hängen zusammen.** Markierst du Text in der Vorschau, wird die
zugehörige Stelle im Editor mitmarkiert — die Auswahl in der Vorschau bleibt dabei
bestehen, Kopieren funktioniert also weiterhin. Umgekehrt zeigt eine dezente Hinterlegung,
an welchem Absatz du gerade schreibst. Das gemeinsame Scrollen lässt sich über das
Schloss-Symbol trennen, wenn du beide Seiten unabhängig lesen willst.

### PDF lesen

- Fortlaufende Seitenansicht mit Zoom, „An Breite anpassen" und „Ganze Seite"
- Textebene: markieren und kopieren wie in jedem PDF-Betrachter
- Volltextsuche mit hervorgehobenen Treffern
- Seitenleiste mit Miniaturen und den Lesezeichen des Dokuments
- Lupe, die dem Zeiger folgt (1,5× bis 6×)
- Ansicht drehen, Drucken, passwortgeschützte Dateien nach Eingabe des Passworts

### Seiten-Werkbank

Die Antwort auf „ich muss mal eben Seiten aus drei PDFs zu einem zusammenstellen": Alle
offenen PDFs liegen als Spalten nebeneinander auf einer Arbeitsfläche, jede Seite als
Miniatur.

| Aktion | Bedienung |
| --- | --- |
| Seite verschieben | Karte greifen und ablegen — auch **in eine andere Spalte**; eine Markierung zeigt, wo sie landet |
| Mehrere auf einmal | Strg-Klick für einzelne, Umschalt-Klick für einen Bereich — die Auswahl wandert zusammen |
| Weiteres PDF dazu | Knopf „PDF hinzufügen…" oder eine Datei aus dem Explorer auf die Fläche ziehen |
| Drehen · Duplizieren · Löschen | Knöpfe unten, wirken auf die Auswahl |
| Fertig | „Alles übernehmen" — jede Spalte geht in ihren Tab zurück, hinzugefügte werden neue Tabs |

Spalten, an denen nichts geändert wurde, bleiben unangetastet.

### PDF bearbeiten

| Werkzeug | Was es tut |
| --- | --- |
| Seiten verwalten | Umsortieren per Ziehen, drehen, löschen (innerhalb eines Dokuments) |
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

### Lesen wie auf einem E-Book-Reader

Mit **F9** (oder dem Buch-Symbol) wird aus jedem Markdown-Dokument ein Buch mit echten
Seiten. EPUB-E-Books öffnen sich per Doppelklick direkt in diesem Lesemodus.

- Einzel- oder Doppelseite; beim Umblättern rollt sich die Seite wie Papier und folgt dem Finger, der Maus oder dem Touchpad — wie beim Kindle
- Auch PDFs lassen sich so lesen: mit an das Thema angepassten Seitenfarben und auf Wunsch abgeschnittenen weißen Rändern
- Lesestelle wird pro Buch gemerkt, auch über einen Neustart hinweg
- Lesezeichen mit Eselsohr und Übersicht, Restlesezeit für Kapitel und Buch mit lernendem Lesetempo
- Vier Lesehintergründe (Hell, Sepia, Dunkel, Nacht), vier Schriften, Größe, Zeilenabstand, Ränder, Blocksatz
- Bei EPUBs: Cover, Inhaltsverzeichnis, jedes Kapitel auf einer neuen Seite, aktuelles Kapitel in der Kopfzeile
- Die Formatierung des Verlags weicht den eigenen Leseeinstellungen — so bleibt Text in jedem Thema lesbar

Kopiergeschützte E-Books (DRM) lassen sich nur in der Lese-App des jeweiligen Shops
öffnen; OpenSlate lehnt sie mit einem Hinweis ab. Kindle-Formate (AZW, KFX, MOBI) werden
nicht unterstützt.

### Weitere Formate

Neben Markdown und PDF öffnet OpenSlate txt, json, js, ts, html, css, xml, svg, yaml,
toml, ini, csv, log und weitere Textformate — jeweils mit passender Syntax-Hervorhebung.
Die Vorschau blendet sich dabei automatisch aus.

---

## Installation

1. Unter [Releases](https://github.com/thecrafti87/OpenSlate-releases/releases/latest) die Datei `OpenSlate-Setup-1.6.0.exe` herunterladen
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

Für `.epub`-Dateien genauso — OpenSlate wird bei der Installation bereits als mögliches
Programm für E-Books eingetragen.

Für `.pdf`-Dateien führt der Weg über die Windows-Einstellungen → Apps → Standard-Apps →
Dateityp `.pdf` → OpenSlate. Edge, Acrobat und andere bleiben über „Öffnen mit" jederzeit
erreichbar.

---

## Updates

OpenSlate hält sich selbst aktuell: Kurz nach dem Start und danach alle vier Stunden
prüft es, ob hier ein neueres Release liegt. Ein neues Update wird ohne Rückfrage im
Hintergrund geladen und beim Beenden installiert — nie mitten in der Arbeit. Eine
Windows-Benachrichtigung meldet, wenn es bereitliegt; ein Klick darauf startet auf Wunsch
sofort neu. Ungespeicherte Dokumente werden dabei wie gewohnt abgefragt.

Wer selbst nachsehen möchte: Einstellungen → **Nach Updates suchen**.

Was dabei nach außen geht, sind Anfragen an diese Release-Seite auf GitHub und der Download des Installers.
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
- E-Books: nur EPUB ohne Kopierschutz; keine Kindle-Formate (AZW, KFX, MOBI), E-Books werden nur gelesen, nicht bearbeitet
- Nur Windows; macOS und Linux sind nicht vorgesehen

---

## Alle Versionen

Der vollständige Änderungsverlauf steht bei jedem Release unter
[Releases](https://github.com/thecrafti87/OpenSlate-releases/releases).

*Diese Seite gehört zu OpenSlate 1.6.0 und wird mit jeder Veröffentlichung aktualisiert.*
