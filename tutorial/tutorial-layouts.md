---
marp: true
paginate: true
title: Layout-Tutorial mit Marp
description: Einfache Präsentationslayouts mit Überschriften, Listen und CSS Grid
style: |
  section {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    padding: 42px;
    font-family: Arial, Helvetica, sans-serif;
  }

  h1, h2 {
    text-align: center;
    color: #17324d;
  }

  code {
    color: #8a1538;
  }
---

# Einfache Layouts mit Marp und CSS

## Ein Tutorial für einfache Präsentationen

In diesem Tutorial lernst du, wie du Folien mit einer **zentrierten Überschrift**,
**Bullet-Points**, **zwei CSS-Grid-Spalten** und einer **Fußzeile** aufbaust.

Die Beispiele werden Schritt für Schritt etwas umfangreicher.

---

# 1. Grundgerüst einer Marp-Datei

Jede Datei beginnt mit einem Front-Matter-Block. Er steht ganz oben und wird von
`---` eingeschlossen.

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

Wichtig:

- `marp: true` schaltet die Markdown-Datei für Marp frei.
- `paginate: true` zeigt die Foliennummer an.
- Nach `style: |` muss jedes CSS-Zeile eingerückt sein.
- Auch HTML-Inhalte werden übersichtlich eingerückt.

---

# 2. Überschrift in der Mitte

Eine Überschrift wird mit `text-align: center` zentriert. Der Container erhält
mit `width: 100%` die gesamte Breite der Folie.

```html
<div class="titel">

# Meine Überschrift

</div>
```

```css
.titel {
  width: 100%;
  text-align: center;
}
```

Die Leerzeilen innerhalb des Containers helfen Marp, die Markdown-Überschrift
korrekt zu erkennen.

---

# 3. Bullet-Points unter dem Titel

Eine Liste folgt unterhalb des Titel-Containers. Sie wird in einen eigenen
Container gelegt, damit sie später leicht gestaltet werden kann.

```html
<div class="liste">

- Ein Punkt
- Noch ein Punkt
- Ein Punkt mit **hervorgehobenem Text**

</div>
```

```css
.liste {
  width: 80%;
  text-align: left;
}
```

Die Liste bleibt linksbündig, obwohl die Überschrift zentriert ist.

---

# 4. Flexbox oder CSS Grid?

Für die gesamte Folie ist `display: flex` sinnvoll. Die Elemente werden
hauptsächlich in **einer Richtung** angeordnet: Überschrift oben, Inhalt in
der Mitte und Fußzeile unten.

```css
section {
  display: flex;
  flex-direction: column;
}
```

Für den eigentlichen Inhalt ist `display: grid` besser. Grid eignet sich für
**zwei Dimensionen**, also für Zeilen und Spalten. Deshalb verwenden wir Grid
für zwei Spalten, Karten oder unterschiedliche Spaltenbreiten.

```css
.grid-2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
```

Merksatz:

- **Flexbox:** eine Richtung, zum Beispiel eine vertikale Folienstruktur
- **Grid:** mehrere Spalten und Zeilen, zum Beispiel Inhaltskarten
- **Kombination:** Flexbox für die Folie und Grid für den Inhaltsbereich

`display: grid` ist also nicht generell besser. Es ist besser, wenn ein
zweidimensionales Layout benötigt wird.

---

# 5. Zwei Spalten mit CSS Grid

CSS Grid teilt einen Container in Spalten. `1fr 1fr` bedeutet, dass beide
Spalten gleich breit sind.

```html
<div class="grid-2">
  <div class="spalte">

  - Linker Punkt
  - Noch ein linker Punkt

  </div>
  <div class="spalte">

  - Rechter Punkt
  - Noch ein rechter Punkt

  </div>
</div>
```

```css
.grid-2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 24px;
  width: 100%;
}
```

`gap` bestimmt den Abstand zwischen den Spalten.

---

# 6. Fußzeile ergänzen

Eine Fußzeile wird am Ende der Folie platziert. Mit `margin-top: auto` wandert
sie bei einem Flex-Layout nach unten.

```html
<div class="fusszeile">
  Klasse 10 · CSS Grid · Seite 1
</div>
```

```css
.fusszeile {
  width: 100%;
  margin-top: auto;
  padding-top: 12px;
  border-top: 2px solid #17324d;
  text-align: center;
  font-size: 0.7rem;
}
```

---

# 7. Aufgaben zum Ausprobieren

1. Ändere die Farbe der Überschrift.
2. Ersetze `1fr 1fr` durch `2fr 1fr`.
3. Ergänze eine dritte Liste.
4. Füge in der Fußzeile deinen Namen ein.
5. Erstelle eine Folie zum Thema „Mein Hobby“.

Die fertigen Beispiele findest du gesammelt im Ordner `vorlagen`.
