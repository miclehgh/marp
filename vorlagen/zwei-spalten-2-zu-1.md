---
marp: true
paginate: true
title: Grid mit ungleichen Spalten
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
    color: #24527a;
  }

  .grid-2 {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 28px;
    width: 100%;
    align-items: center;
  }

  .text {
    text-align: left;
  }

  .merksatz {
    padding: 20px;
    background: #f4d35e;
    font-weight: bold;
  }

  .fusszeile {
    width: 100%;
    margin-top: auto;
    padding-top: 12px;
    border-top: 1px solid #17324d;
    text-align: center;
    font-size: 0.7rem;
  }
---

<div class="titel">

# Warum erneuerbare Energie?

</div>

<div class="grid-2">
  <div class="text">

  - Sonne und Wind stehen langfristig zur Verfügung.
  - Die Nutzung verursacht im Betrieb wenig CO2.
  - Speicher und Netze müssen weiterentwickelt werden.

  </div>
  <div class="merksatz">
  Merksatz: Die Energiewende braucht Technik und gute Planung.
  </div>
</div>

<div class="fusszeile">
  Warum erneuerbare Energie? · 2:1-Grid mit Merksatz und Begründung
</div>
