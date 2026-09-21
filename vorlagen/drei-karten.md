---
marp: true
paginate: true
title: Drei Karten mit CSS Grid
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

  .karten {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
    width: 100%;
  }

  .karte {
    min-height: 150px;
    padding: 16px;
    background: #eef5f9;
    border-top: 5px solid #24527a;
    text-align: left;
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

# Kompetenzen für die Zukunft

</div>

<div class="karten">
  <div class="karte">

  **Kritisches Denken**

  - Quellen vergleichen
  - Argumente prüfen

  </div>
  <div class="karte">

  **Teamarbeit**

  - Rollen verteilen
  - Ergebnisse teilen

  </div>
  <div class="karte">

  **Kreativität**

  - Ideen entwickeln
  - Lösungen testen

  </div>
</div>

<div class="fusszeile">
  Layout mit CSS Grid; drei Karten
</div>
