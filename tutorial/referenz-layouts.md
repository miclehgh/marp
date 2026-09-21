---
marp: true
title: Referenz zu den Layout-Vorlagen
description: Einfache Erklärung der CSS-Klassen und Eigenschaften
style: |
  section {
    padding: 42px;
    font-family: Arial, Helvetica, sans-serif;
  }

  h1, h2 {
    color: #17324d;
  }

  table {
    font-size: 0.72rem;
  }
---

# Referenz: Layout-Vorlagen

Diese Datei erklärt die wichtigsten Bausteine aus den Vorlagen. Alle Dateien
verwenden Marp und können mit der Marp-Erweiterung in VS Code als Präsentation
dargestellt werden.

---

# Front-Matter

Das Front-Matter steht immer am Anfang der Datei:

```markdown
---
marp: true
paginate: true
style: |
  section {
    padding: 40px;
  }
---
```

| Eintrag | Bedeutung |
| --- | --- |
| `marp: true` | Aktiviert die Marp-Verarbeitung. |
| `paginate: true` | Zeigt die Seitenzahl an. |
| `style: |` | Beginnt den CSS-Block. |
| Einrückung | Alles unter `style` gehört zum CSS. |

---

# Die wichtigsten CSS-Klassen

| Klasse | Aufgabe |
| --- | --- |
| `.titel` | Zentriert die Überschrift über die gesamte Breite. |
| `.liste` | Richtet Bullet-Points linksbündig aus. |
| `.grid-2` | Erzeugt zwei Spalten mit CSS Grid. |
| `.spalte` | Formatiert den Inhalt einer Grid-Spalte. |
| `.karten` | Erzeugt mehrere gleich breite Karten. |
| `.fusszeile` | Setzt eine Linie und Text an das untere Ende. |

---

# Warum ist die Einrückung wichtig?

Nach `style: |` müssen die CSS-Zeilen eingerückt werden:

```yaml
style: |
  section {
    padding: 40px;
  }
```

Auch verschachtelte HTML-Elemente sollten eingerückt sein:

```html
<div class="grid-2">
  <div class="spalte">
    Inhalt der linken Spalte
  </div>
  <div class="spalte">
    Inhalt der rechten Spalte
  </div>
</div>
```

Die Einrückung verbessert die Lesbarkeit und verhindert, dass die Struktur
vertauscht oder versehentlich außerhalb des Containers fortgesetzt wird.

---

# CSS Grid: Spalten festlegen

```css
.grid-2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 24px;
}
```

| Wert | Erklärung |
| --- | --- |
| `display: grid` | Aktiviert CSS Grid. |
| `1fr 1fr` | Zwei gleich große Spalten. |
| `2fr 1fr` | Linke Spalte doppelt so breit. |
| `gap: 24px` | Abstand zwischen den Spalten. |

---

# Flexbox für die Fußzeile

Damit die Fußzeile unten bleibt, wird die Folie als Flex-Container aufgebaut:

```css
section {
  display: flex;
  flex-direction: column;
  min-height: 100%;
}

.fusszeile {
  margin-top: auto;
}
```

`margin-top: auto` nimmt den verfügbaren freien Platz ein und schiebt die
Fußzeile nach unten.

---

# Zuordnung der Beispiele

Alle Vorlagen liegen unabhängig von der Klassenstufe gemeinsam im Ordner
`vorlagen`. Die Dateinamen zeigen den jeweiligen Schwerpunkt:

| Datei | Schwerpunkt |
| --- | --- |
| `titel-und-bullet-points.md` | Überschrift und Bullet-Points |
| `zwei-spalten-gleich.md` | Zwei gleich große Grid-Spalten |
| `zwei-spalten-2-zu-1.md` | Spalten im Verhältnis 2 zu 1 |
| `zwei-spalten-mit-fusszeile.md` | Grid mit Fußzeile |
| `drei-karten.md` | Drei Karten mit CSS Grid |
| `zwei-spalten-grid.md` | Überschrift, zwei Spalten und Fußzeile |
| `arch-linux-kurz-erklaert.md` | Text und Bild am Beispiel Arch Linux |
