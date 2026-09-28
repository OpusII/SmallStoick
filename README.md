# Stoický kompas

Soukromý deník a jemný průvodce pro týdenní cíle. Stačí statický web, bez účtu, serveru a externích knihoven.

## Co aplikace umí

- Denní česká myšlenka, otázka a drobný pokus: **všech 51 oddílů** Epiktétova *Enchiridionu* a poznámek v dodaném PDF je zastoupeno vlastní stručnou parafrází, plus 8 nenáboženských cvičení všímavosti. V denním cyklu se 17 kapitol vybraných uživatelem objevuje častěji; poměr 68 stoických ku 8 všímavým dnům je přibližně 90 % ku 10 %. Celou sbírku lze procházet na úvodní stránce. Myšlenky jsou **autorské parafráze**, nikoli doslovné citáty či úplný překlad knihy.
- Čtyři stoické ctnosti jsou na úvodní stránce převedeny do běžných otázek: moudrost, spravedlnost, odvaha, uměřenost. Nejsou hodnocené body.
- Verze 3 přidává **Mentora**: čtyři krátké kroky nad vlastní situací (událost a výklad; co ovlivním; ctnost; malý další krok), plus zcela dobrovolné ranní a večerní úvahy. Ranní příprava je volně inspirována Markem Aureliem (*Hovory k sobě* II.1), večerní ohlédnutí Senekou (*O hněvu* III.36). Nejsou zde série, penalizace za vynechání ani upozornění mimo aplikaci. Mentor skládá odpověď z tvých slov a připravených pravidel; není to model, který by tvé situaci rozuměl jako člověk.
- V deníku lze označit, zda ses věnoval přírodě, čtení, lidem, pohybu, tvoření nebo odpočinku. Kompas počítá třicetidenní přehled z těchto štítků, jednoduchých zmínek v textu a zapsaných cílů.
- Pokud je dost zápisů a oblast se v nich dlouho neobjevila, kompas ji může jemně navrhnout. Absence zmínky není důkaz, že se aktivita nestala. Návrhy jsou jednoduchá pravidla, nikoli konverzační umělá inteligence.
- Starší záznamy ze stejného prohlížeče zůstávají zachované; rozšířený formát zálohy zachovává i nové štítky.
- Verze 4 přidává XP a úrovně. Deník přidá 8 XP za den, zapsaný cíl 7 XP (nejvýše dvě různá splnění za den), mentorský rozhovor 8 XP za den, ranní úvaha 2 XP, večerní 3 XP a týdenní ohlédnutí 12 XP. Návrat po aspoň sedmidenní pauze přidá 10 XP. Každou odměnu lze získat jen jednou za příslušný den nebo týden; úpravy zápisu ji nerozmnoží. Úroveň roste podle hranice `60 × (úroveň − 1) + 6 × (úroveň − 1)²`, bez konečného stropu. Dřívější XP se při aktualizaci dopočítají ze stávajících záznamů a nikdy se kvůli pauze neodečítají. Počet zaznamenaných aktivních dní za posledních 28 dní dává jen kontext, bez série a sankcí. XP i úrovně jsou uložené pouze v místním prohlížeči a v záloze.

Na úvodní stránce pod dnešní myšlenkou rozbal **Procházet všech 51 oddílů Enchiridionu a cvičení všímavosti**. Označení **TVÁ CESTA · VERZE 4** slouží i ke kontrole načtené verze.

## Vyzkoušení

V adresáři spusť `python3 -m http.server 8000` a otevři `http://localhost:8000`. Samotný `index.html` lze otevřít i přímo, ale režim offline a instalace na plochu fungují jen přes HTTPS nebo localhost.

## GitHub Pages

Nahraj **obsah této složky** do kořenového adresáře repozitáře. V nastavení repozitáře otevři **Settings → Pages**, vyber publikování z větve `main` a složku `/ (root)`. Pak otevři adresu, kterou GitHub Pages zobrazí. Relativní cesty fungují i při publikování pod názvem repozitáře.

Na mobilu otevři publikovanou adresu a použij nabídku prohlížeče **Přidat na plochu**. Dostupnost instalačního tlačítka závisí na telefonu a prohlížeči. Po první návštěvě přes HTTPS aplikace funguje i bez sítě.

Pokud aktualizuješ už publikovanou verzi, nahraj všechny soubory znovu včetně nového `thoughts.js` a `sw.js`. Po publikování aplikaci zavři a dvakrát obnov, aby se aktivovala nová offline verze. Data prohlížeče nemaž.

## Data a soukromí

Zápisy, cíle, mentorovy rozhovory a preference jsou v `localStorage` daného prohlížeče. Není tu přihlášení ani synchronizace mezi telefonem a počítačem. GitHub Pages hostuje veřejně zdrojový kód aplikace, **nikoli tvé záznamy**. Pravidelně použij **Stáhnout zálohu**. Import stávající data nahradí po potvrzení. Smazání dat prohlížeče odstraní místní záznamy. Neexistují push notifikace; páteční impuls se ukáže při otevření aplikace.

Návrhy kompasu jsou lokální pravidla nad tvými zájmy, energií a zápisy, bez vzdáleného AI modelu. V dalších verzích lze přidat skutečný konverzační mentor, ale ten by vyžadoval backend a řešení přenosu soukromých záznamů.

## Licence

MIT – můžeš používat, upravovat a sdílet. Viz `LICENSE`.
