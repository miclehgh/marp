---
marp: true
paginate: true
title: Layout mit CSS-Variablen
style: |
  :root {
    --dunkel: #182b49;
    --akzent: #e07a5f;
    --hell: #f4f1de;
  }

  section {
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100%;
    padding: 40px;
    background: var(--hell);
    font-family: Arial, Helvetica, sans-serif;
  }

  .titel {
    width: 100%;
    text-align: center;
    color: var(--dunkel);
  }

  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    width: 100%;
  }

  .spalte {
    padding: 18px;
    background: white;
    border-top: 6px solid var(--akzent);
    text-align: left;
  }

  .fusszeile {
    width: 100%;
    margin-top: auto;
    color: var(--dunkel);
    text-align: center;
    font-size: 0.7rem;
  }
---

<div class="titel">

# Nachhaltige Stadt

</div>

<div class="grid-2">
  <div class="spalte">

  **Verkehr**

  - Sichere Radwege
  - Gute Busverbindungen
  - Weniger Autoverkehr

  </div>
  <div class="spalte">

  **Energie**

  - Solaranlagen
  - Energiesparende Gebäude
  - Intelligente Beleuchtung

  </div>
</div>

<div class="fusszeile">
  Nachhaltige Stadt · Zwei Spalten mit CSS-Variablen
</div>

