# Focus & Center

**Der Präsentations-Werkzeugkasten für Windows.**

Zoomen, Zeichnen, Verwischen, Einfrieren, Text erkennen – live in jeder Präsentation. Eine Datei, keine Installation, gratis.

> Präsentieren ohne den Vortrag zu unterbrechen. Jedes Werkzeug liegt auf einem globalen Hotkey und wirkt auf dem Monitor, auf dem deine Maus gerade steht – auch bei mehreren Bildschirmen und unterschiedlicher Skalierung.

---

## Warum

Die Präsentation läuft, dreißig Augenpaare folgen deinem Mauszeiger – und genau jetzt ist die Schrift zu klein, die Kundennummer sichtbar, die Zahl aus der anderen Tabelle nicht zur Hand. Focus & Center ist für genau diese Sekunden gebaut.

Passend, wenn du:

- Schulungen, Webinare oder Vorlesungen hältst
- Software live vorführst – beim Kunden oder im Team
- Zahlen aus Excel & Dashboards präsentierst
- Bildschirminhalte mit vertraulichen Daten zeigst
- Architekturpläne vorstellst

---

## Werkzeuge

Neun Werkzeuge, null Unterbrechung.

| Hotkey                  | Werkzeug                          | Was es tut                                                                                                                                             |
| ----------------------- | --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `Strg+1`              | **Zoom**                    | Friert den Bildschirm ein und vergrößert bis 16-fach. Ansicht folgt der Maus; Mausrad oder ↑/↓ zoomen, zeichnen geht direkt hinein.                |
| `Strg+2`              | **Zeichnen**                | Stift, gerade Linie, Rechteck, Ellipse, Pfeil. Zehn Stiftfarben auf Einzeltasten, Textmarker-Modus, Strichbreite per`Strg+Mausrad`.                  |
| `X`                   | **Verwisch-Stift**          | Verwischt Bildschirminhalt unter dem Strich – Namen, Beträge, E-Mails in einer Handbewegung unkenntlich. Auch als Rechteck oder Ellipse.             |
| `T` / `Strg+V`      | **Text & Einfügen**        | Text direkt auf den Bildschirm tippen.`Strg+V` fügt Text, Bilder und Excel-Tabellen ein – Tabellen werden automatisch als sauberes Bild gerendert. |
| `W` / `K`           | **Whiteboard & Blackboard** | Weißer oder schwarzer Hintergrund auf Tastendruck.`Strg+C` kopiert die Ansicht, `Strg+S` speichert als PNG.                                       |
| `Strg+7`              | **Focus & Center**          | Bereiche aufziehen – sie springen vergrößert in die Bildschirmmitte, der Rest wird abgedunkelt und weichgezeichnet.                                 |
| `Strg+Umsch+C`        | **Bereiche einfrieren**     | Ausschnitte werden zu schwebenden Fenstern – als eigene Prozesse überleben sie sogar das Beenden der App.                                            |
| `Strg+Umsch+T`        | **Texterkennung (OCR)**     | Bereich aufziehen, fertig: Text und Zahlen per Tesseract erkannt (Deutsch + Englisch gebündelt), in die Zwischenablage kopiert, editierbar.           |
| `Strg+3` / `Strg+6` | **Timer & Snip**            | Pausen-Timer im Vollbild. Snip legt Ausschnitte in die Zwischenablage (`Strg+6`) oder als PNG (`Strg+Umsch+6`).                                    |

### Werkzeuge stapeln sich wie Folien

Modi lassen sich verschachteln: zeichnen (`Strg+2`), Bereich hervorheben (`Strg+7`), darüber weiterzeichnen – jede Ebene setzt auf der vorherigen auf. `Esc` schließt immer nur die oberste Ebene. Beliebig tief.

---

## Systeme

- **macOS** – Apple Silicon & Intel
- **Ubuntu Linux** – X11 (`maim`, `xclip`) oder Wayland (`grim`, `wl-clipboard`), dazu `libnotify` und `tesseract-ocr`
- **Windows 10/11** – klassische Windows-Version inkl. LiveZoom (`Strg+4`)

Eigenständige Einzeldatei. Keine Installation, keine Adminrechte. Löschen der Datei entfernt alles.

> **Hinweis Wayland:** Globale Hotkeys sind dort systembedingt eingeschränkt. Unter Ubuntu-Standard-GNOME funktionieren sie in der Regel; ansonsten sind alle Werkzeuge über das Tray-Menü oder eigene System-Shortcuts erreichbar.

---

## Design-Prinzipien

- **Eine einzige Datei** – herunterladen, starten, fertig. Symbol in der Menüleiste bzw. neben der Uhr.
- **System-Technik als Motor** – Screenshots per macOS-Screencapture bzw. `grim`/`maim`, OCR per Tesseract. Bewährte Technik statt Blackbox.
- **Keine Telemetrie, kein Konto** – arbeitet vollständig lokal, baut keine Internetverbindung auf.
- **Verträgt sich mit belegten Hotkeys** – ist ein Kürzel vergeben (z. B. durch ZoomIt), meldet sich das Tool per Hinweis; alle Funktionen bleiben über das Tray-Menü erreichbar.

---

## Hotkey-Spickzettel

### Modi

| Taste            | Funktion                       |
| ---------------- | ------------------------------ |
| `Strg+1`       | Zoom (eingefroren, zeichenbar) |
| `Strg+2`       | Zeichnen ohne Zoom             |
| `Strg+3`       | Pausen-Timer                   |
| `Strg+4`       | Hinweis auf die System-Lupe    |
| `Strg+6`       | Snip → Zwischenablage         |
| `Strg+Umsch+6` | Snip → PNG-Datei              |
| `Strg+7`       | Focus & Center                 |
| `Strg+Umsch+C` | Bereich(e) einfrieren          |
| `Strg+Umsch+T` | Texterkennung (OCR)            |

### Im Zeichenmodus

| Taste                   | Funktion                      |
| ----------------------- | ----------------------------- |
| `Umschalt+Ziehen`     | Gerade Linie                  |
| `Strg+Ziehen`         | Rechteck                      |
| `Tab+Ziehen`          | Ellipse                       |
| `Umsch+Strg+Ziehen`   | Pfeil                         |
| `R G B O Y P Q V E S` | Stiftfarben                   |
| `Umschalt+Farbe`      | Textmarker                    |
| `X`                   | Verwisch-Stift an/aus         |
| `T`                   | Text tippen                   |
| `Strg+V`              | Text/Bild/Tabelle einfügen   |
| `W` / `K`           | Whiteboard / Blackboard       |
| `Strg+Z` / `Entf`   | Rückgängig / alles löschen |
| `Strg+C` / `Strg+S` | Kopieren / als PNG speichern  |

### In Focus & Center (`Strg+7`)

| Taste                     | Funktion                         |
| ------------------------- | -------------------------------- |
| `Ziehen`                | Bereich hervorheben              |
| `Umschalt+Ziehen`       | Weiteren Bereich hinzufügen     |
| `Entf` / `Rücktaste` | Letzten Bereich zurücknehmen    |
| `Mausrad`               | Abdunkeln/Weichzeichnen stärker |
| `Esc`                   | Alle Bereiche schließen         |

---

## FAQ

**Brauche ich Adminrechte oder eine Installation?**
Nein. Eine einzelne, eigenständige Datei. macOS fragt beim ersten Start einmalig nach Freigabe für Bildschirmaufnahme (Systemeinstellungen → Datenschutz & Sicherheit).

**Was ist mit LiveZoom (`Strg+4`)?**
Basiert auf der Windows Magnification-API, daher nur in der Windows-Version. Auf macOS/Linux zeigt `Strg+4` einen Hinweis auf die System-Lupe. Der eingefrorene Zoom (`Strg+1`) deckt die typischen Präsentationsfälle ab.

**Sammelt das Tool Daten?**
Nein. Komplett lokal, keine Internetverbindung, keine Telemetrie.

**Ist eine Bildschirmaufnahme enthalten?**
Nein, bewusst nicht – dein System bringt sie mit: `Cmd+Umsch+5` (macOS), `Strg+Umsch+Alt+R` (GNOME), `Win+Alt+R` (Windows).

**Geld-zurück-Garantie?**
14 Tage, ohne Angabe von Gründen.

---

## Lizenz

MIT License · Copyright (c) 2026 JJJ-Engineering
