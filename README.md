# Einfache Präsentationslayouts mit Marp

Diese Sammlung enthält einfache Markdown-Vorlagen für Präsentationen mit
[Marp](https://marp.app/). Die Beispiele sind für den Unterricht und für
erste eigene Präsentationen gedacht.

## Ordner

- `tutorial` enthält die Erklärungen und die CSS-Referenz.
- `vorlagen` enthält die fertigen Layout-Vorlagen.
- `bilder` enthält verwendete Bilder, darunter das Arch-Linux-Logo.

## Start in VS Code

1. Installiere die Erweiterung **Marp for VS Code**.
2. Öffne eine Datei aus `vorlagen`.
3. Öffne die Vorschau mit `Strg+Umschalt+V`.
4. Ändere Überschrift, Listen und Farben.

## Eine passende Vorlage finden

| Aufgabe | Vorlage |
| --- | --- |
| Überschrift und Liste | `titel-und-bullet-points.md` |
| Zwei gleich große Spalten | `zwei-spalten-gleich.md` |
| Eine breite und eine schmale Spalte | `zwei-spalten-2-zu-1.md` |
| Arch Linux mit Bild | `arch-linux-kurz-erklaert.md` |
| Drei Themen nebeneinander | `drei-karten.md` |
| Vollständige Inhaltsfolie | `komplettes-layout.md` |

## PDF exportieren

Öffne die Marp-Vorschau in VS Code und wähle dort **Export slide deck**.
Danach kannst du zum Beispiel **PDF** auswählen.

## Aufbau einer Vorlage

Jede Vorlage besteht aus drei Teilen:

1. Front-Matter am Anfang der Datei
2. CSS im Bereich `style: |`
3. Inhalt mit Markdown und eingerücktem HTML

Das Tutorial in `tutorial/tutorial-layouts.md` erklärt diese Teile Schritt
für Schritt.

## Bildnachweis

Das Arch-Linux-Logo in `bilder/arch-linux-logo.svg` stammt von der
offiziellen Arch-Linux-Webseite. Die Verwendung des Logos sollte die
Arch-Linux-Richtlinien zur Markennutzung beachten.
