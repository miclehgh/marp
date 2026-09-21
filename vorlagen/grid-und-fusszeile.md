---
marp: true
paginate: true
title: Grid, Überschrift und Fußzeile
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
    grid-template-columns: 2fr 1fr;
    gap: 30px;
    width: 100%;
    align-items: start;
  }

  .haupttext {
    text-align: left;
  }

  .seiteninfo {
    padding: 16px;
    background: #f4d35e;
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

# Künstliche Intelligenz im Alltag

</div>

<div class="grid-2">
  <div class="haupttext">

  - Sprachassistenten erkennen gesprochene Befehle.
  - Empfehlungssysteme schlagen Inhalte vor.
  - Übersetzungsprogramme verarbeiten Sprache.
  - Ergebnisse müssen kritisch geprüft werden.

  </div>
  <div class="seiteninfo">
  
  **Leitfrage**

  Wo hilft KI und wo brauchen wir menschliche Kontrolle?
  </div>
</div>

<div class="fusszeile">
  Klasse 11 · Technik und Gesellschaft · 2026
</div>

