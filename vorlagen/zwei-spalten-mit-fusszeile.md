---
marp: true
paginate: true
title: Grid mit Fußzeile
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
    text-align: center;
    color: #17324d;
  }

  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    width: 100%;
  }

  .spalte {
    padding: 18px;
    border: 2px solid #7aa7c7;
    text-align: left;
  }

  .fusszeile {
    width: 100%;
    margin-top: auto;
    padding-top: 12px;
    border-top: 2px solid #17324d;
    text-align: center;
    font-size: 0.7rem;
  }
---

<div class="titel">

# Eine gute Präsentation

</div>

<div class="grid-2">
  <div class="spalte">

  **Inhalt**

  - Eine klare Aussage pro Folie
  - Kurze Stichpunkte
  - Passende Beispiele

  </div>
  <div class="spalte">

  **Gestaltung**

  - Gute Kontraste
  - Genügend Abstand
  - Einheitliche Farben

  </div>
</div>

<div class="fusszeile">
  Eine gute Präsentation · Zwei Spalten mit Inhalt und Gestaltung
</div>

