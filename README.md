# Seriálové a filmové portfolio

Tento projekt je jednoduchý web, který zobrazuje přehled **nejlepších a nejhorších seriálů**, případně **nadcházejících seriálů a filmů**.  
Každý seriál nebo film je reprezentován **kartou s obrázkem, názvem a krátkým popisem**.

---

## Použité technologie

- **HTML5** – struktura stránek (`index.html`, `top10filmy.html`, `top10serialy.html`, `nove.html`)  
- **CSS3** – stylování, layout, karty a hover efekty (`style.css`)  
- **Flexbox** – pro zobrazení **2 karet vedle sebe** a jejich automatické zalamování do dalších řad  
- **Responsivní design** – media queries zajišťují, že na mobilu se karty zobrazí **jedna pod druhou**  

---

## Jak kód funguje

1. **Struktura souborů**

serialy-portfolio/
│
├── index.html <-- hlavní stránka s úvodem a odkazy
├── top10filmy.html <-- Top 10 nejlepších filmů
├── top10serialy.html <-- Top 10 nejlepších seriálů
├── nove.html <-- Nadcházející seriály/filmy
├── style.css <-- všechny styly, layout, karty, hover efekty
└── README.md


2. **Hlavní body CSS**
- `.series-grid` – kontejner karet, **flexbox**, `flex-wrap: wrap`, `justify-content: space-between`  
- `.series-card` – každá karta má šířku `calc(50% - 9px)`, border-radius, box-shadow a hover efekt  
- Obrázky (`img`) mají fixní výšku a `object-fit: cover`  
- `.card-body` – obsah karty (název, popis, meta informace)  
- Media query pro obrazovky menší než 700px → karty na **1 sloupec**  

3. **Proč kód funguje**
- Flexbox zajišťuje automatické zalamování řad a zarovnání karet  
- Šířka karty je přesně polovina kontejneru minus mezera (`gap`) → **2 karty vedle sebe**  
- Media query zaručuje, že na mobilu se karty nepřekrývají  
- Všechny styly jsou v samostatném `style.css`, HTML pouze odkazuje na tento soubor  

---

## Doporučené filmy/seriály

### Vykoupení z věznice Shawshank
![Shawshank](https://via.placeholder.com/400x225?text=Shawshank)  
Silný příběh o naději, přátelství a odvaze přežít. Sleduje muže uvězněného za čin, který nespáchal, a jeho cestu, jak se vyrovnává s životem za mřížemi a hledá cestu ke svobodě. Napínavý a inspirativní film, který stojí za zhlédnutí.  

### Kmotr (The Godfather)
![Kmotr](https://via.placeholder.com/400x225?text=Kmotr)  
Legendární příběh o moci, rodině a loajalitě v mafiánském světě. Napínavý a hluboce lidský film, který se stal klasikou.  

### Kmotr II (The Godfather Part II)
![Kmotr II](https://via.placeholder.com/400x225?text=Kmotr+II)  
Pokračování slavného příběhu, které odhaluje původ a životní cestu klíčových postav, plné intrik, rodinných vztahů a rozhodnutí, která formují osudy.  

### Temný rytíř (The Dark Knight)
![Temný rytíř](https://via.placeholder.com/400x225?text=Temny+Rytir)  
Napínavý superhrdinský film, který sleduje boj spravedlnosti s chaosem v Gotham City. Strhující akce, silné postavy a morální dilemata, která vás nenechají chladnými.  

---

## Jak web spustit

1. Otevři složku projektu ve **Visual Studio Code**  
2. Otevři HTML soubor (např. `top10.html`) → pravým klikem **Open with Live Server** nebo běžně v prohlížeči  
3. Obrázky můžeš měnit dle potřeby:  
   - URL z internetu  
   - Lokální soubory (např. `images/film1.jpg`)  

---

## Tipy pro úpravy

- Přidání dalších seriálů/filmů → zkopírovat `<article class="series-card">...</article>`  
- Změna velikosti karet → upravit `width` a `height` v CSS  
- Barevné ladění → upravit barvy pozadí, textu, linků a hover efektu v CSS  
