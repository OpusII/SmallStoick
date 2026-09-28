# Stoický kompas

Soukromý deník a jemný průvodce pro týdenní cíle. Stačí statický web, bez účtu, serveru a externích knihoven.

## Vyzkoušení

V adresáři spusť `python3 -m http.server 8000` a otevři `http://localhost:8000`. Samotný `index.html` lze otevřít i přímo, ale režim offline a instalace na plochu fungují jen přes HTTPS nebo localhost.

## GitHub Pages

Nahraj **obsah této složky** do kořenového adresáře repozitáře. V nastavení repozitáře otevři **Settings → Pages**, vyber publikování z větve `main` a složku `/ (root)`. Pak otevři adresu, kterou GitHub Pages zobrazí. Relativní cesty fungují i při publikování pod názvem repozitáře.

Na mobilu otevři publikovanou adresu a použij nabídku prohlížeče **Přidat na plochu**. Dostupnost instalačního tlačítka závisí na telefonu a prohlížeči. Po první návštěvě přes HTTPS aplikace funguje i bez sítě.

## Data a soukromí

Zápisy, cíle a preference jsou v `localStorage` daného prohlížeče. Není tu přihlášení ani synchronizace mezi telefonem a počítačem. GitHub Pages hostuje veřejně zdrojový kód aplikace, **nikoli tvé záznamy**. Pravidelně použij **Stáhnout zálohu**. Import stávající data nahradí po potvrzení. Smazání dat prohlížeče odstraní místní záznamy. Neexistují push notifikace; páteční impuls se ukáže při otevření aplikace.

Návrhy kompasu jsou lokální pravidla nad tvými zájmy, energií a zápisy, bez vzdáleného AI modelu. V dalších verzích lze přidat skutečný konverzační mentor, ale ten by vyžadoval backend a řešení přenosu soukromých záznamů.

## Licence

MIT – můžeš používat, upravovat a sdílet. Viz `LICENSE`.
