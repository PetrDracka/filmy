Seriálové portfolio / Filmové doporučení

Tento projekt je jednoduchý web, který zobrazuje přehled nejlepších a nejhorších seriálů, případně nadcházejících seriálů/filmů. Každý seriál nebo film je reprezentován kartou s obrázkem, názvem a krátkým popisem.

Použité technologie

HTML5 – struktura stránek (index.html, top10.html, flop10.html, nove.html)

CSS3 – stylování, zajištění kompaktního layoutu a responzivity (style.css)

Flexbox – pro zobrazení 2 karet vedle sebe a jejich automatické zalamování do dalších řad
Responsivní design – díky media queries se karty zobrazují na mobilu jedna pod druhou

Jak je kód nastavený

Struktura souborů:

serialy-portfolio/
│
├── index.html       <-- hlavní stránka s úvodem a odkazy
├── top10.html       <-- Top 10 nejlepších seriálů/filmů
├── flop10.html      <-- Top 10 nejhorších seriálů/filmů
├── nove.html        <-- Nadcházející seriály/filmy
├── style.css        <-- všechny styly, layout, karty, hover efekty
└── README.md


Hlavní body CSS:

.series-grid – kontejner karet, flexbox, flex-wrap: wrap, justify-content: space-between

.series-card – každá karta má šířku calc(50% - 9px), border-radius, box-shadow a hover efekt

Obrázky (img) mají fixní výšku a object-fit: cover

.card-body – obsah karty (název, popis, meta informace)

Media query pro obrazovky menší než 700px → karty na 1 sloupec

Proč kód funguje:

Flexbox zajišťuje automatické zalamování řad a zarovnání karet

Šířka karty je přesně polovina kontejneru minus mezera (gap) → 2 karty vedle sebe

Media query zaručuje, že na mobilu se karty nepřekrývají

Všechny styly jsou v samostatném style.css, HTML pouze odkazuje na tento soubor

Doporučení k použití

Otevři složku v Visual Studio Code

Ujisti se, že všechny soubory jsou ve stejné složce

Otevři HTML soubor (např. top10.html) → pravým klikem Open with Live Server nebo běžně v prohlížeči

Obrázky můžeš měnit dle potřeby – můžeš použít:

URL z internetu

Lokální soubory (např. images/film1.jpg)

Tipy pro úpravy

Přidání dalších seriálů/filmů → zkopírovat <article class="series-card">...</article>

Změna velikosti karet → upravit width a height v CSS

Barevné ladění → upravit barvy pozadí, textu, linků a hover efektu v CSS# filmy