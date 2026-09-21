---
marp: true
paginate: true
title: Titel und Bullet-Points
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

  .layout {
    display: grid;
    grid-template-columns: 1.4fr 0.8fr;
    gap: 24px;
    width: 100%;
    align-items: start;
  }

  .liste {
    padding: 18px 20px;
    background: #f7f9fc;
    border-left: 6px solid #17324d;
    text-align: left;
    font-size: 1.05rem;
  }

  .notiz {
    padding: 18px;
    background: #fff3cd;
    border: 1px solid #d9b32d;
    text-align: left;
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

# Mein Hobby

</div>

<div class="layout">
  <div class="liste">

  - Ich spiele gerne Fußball.
  - Ich trainiere zweimal pro Woche.
  - Am Wochenende spiele ich mit meinem Team.

  </div>
  <div class="notiz">

  Freizeit macht Spaß, wenn sie regelmäßig und mit Motivation passiert.

  </div>
</div>

<div class="fusszeile">
  Mein Hobby · Bullet-Points mit Zusatznotiz statt nur einer Liste
</div>
