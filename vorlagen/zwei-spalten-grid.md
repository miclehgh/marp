---
marp: true
paginate: true
title: Zwei Spalten mit CSS Grid
style: |
  section {
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100%;
    padding: 40px;
    font-family: Arial, Helvetica, sans-serif;
  }

  .titel {
    width: 100%;
    margin-bottom: 40px;
    text-align: center;
  }

  .titel h1 {
    color: rgb(36, 13, 172);
    /* border: 2px solid rgb(36, 13, 172); */
  }

  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    width: 100%;
  }

  .spalte {
    padding: 20px;
    background: #f0f4f8;
    border-top: 5px solid rgb(100, 20, 40);
    text-align: left;
  }

  .fusszeile {
    width: 100%;
    margin-top: auto;
    padding-top: 12px;
    border-top: 1px solid rgb(100, 20, 40);
    text-align: center;
    font-size: 0.7rem;
  }
---

<div class="titel">

# CSS Grid: Zwei Spalten

</div>

<div class="grid-2">
  <div class="spalte">

  **Linke Spalte**

  - CSS Grid wird mit `display: grid` aktiviert.
  - `1fr` bedeutet: ein gleicher Teil.
  - Der Inhalt bleibt linksbündig.

  </div>
  <div class="spalte">

  **Rechte Spalte**

  - `grid-template-columns` legt Spalten fest.
  - `gap` bestimmt den Abstand.
  - Beide Spalten sind gleich breit.

  </div>
</div>

<div class="fusszeile">
  CSS Grid: Zwei Spalten · Gleich breite Spalten mit Bereichs-Layout
</div>
