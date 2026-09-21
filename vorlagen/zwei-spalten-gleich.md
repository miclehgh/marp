---
marp: true
paginate: true
title: Gleich große Grid-Spalten
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
    margin-bottom: 40px;
  }

  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    width: 100%;
  }

  .spalte {
    padding: 18px;
    background: #e8f1f8;
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

# Zwei Seiten des Internets

</div>

<div class="grid-2">
  <div class="spalte">

  **Chancen**

  - Schnelle Informationen
  - Austausch mit anderen
  - Digitale Lernangebote

  </div>
  <div class="spalte">

  **Risiken**

  - Falsche Informationen
  - Datenschutzprobleme
  - Zu viel Bildschirmzeit

  </div>
</div>

<div class="fusszeile">
  Layout mit CSS Grid; Überschrift, zwei Spalten, Fußzeile
</div>
