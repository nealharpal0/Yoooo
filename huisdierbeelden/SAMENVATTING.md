# Samenvatting – huisdierbeeldjes (nacht 4–5 november 2026)

## Wat er ligt

| Bestand | Inhoud |
|---|---|
| `rapport.md` | Rapport (±8 A4) met inhoudsopgave: foto → 3D-model, printen, schilderen, markt, kostprijs, regels, productpagina en advies; bronnen per deel in de bijlage |
| `startpakket.csv` | 12 producten voor je vriend met prijs, winkel, URL en status (basis ± € 145) |
| `concurrenten.csv` | 15 aanbieders (NL, BE, DE, internationaal, Etsy, full-colour) met prijs, levertijd en reviews |
| `kostprijs.csv` | Rekenmodel per formaat, 3 prijsniveaus, break-even en 2 verdeelmodellen |
| `productpagina.md` | Concepttekst voor Pootjespret met bestelflow, foto-tips en verplichte vinkjes |

**Kern:** AI (Meshy Pro, $20/mnd) is de goedkoopste route naar een model; FDM met filler primer volstaat om te beschilderen. Materiaal kost € 1–5 per beeldje, **arbeid is 75–80% van de kostprijs**. De directe concurrent (Atelier Robijns, BE) vraagt € 44,95 voor ±10 cm; op dat niveau verdienen jullie ±€ 7 per uur. Middenniveau (12 cm € 79) geeft ±€ 9–10 per uur en break-even na ±5 beeldjes. Btw is 21% (3D-geprinte beeldjes vallen niet onder 9%). Maatwerk heeft geen bedenktijd, mits je dat vooraf meldt.

## Aannames

1. **WebFetch werkte niet** (DNS-fout op elke site); alles komt uit zoekresultaten van WebSearch. Pagina's zijn niet volledig gelezen.
2. Printertype onbekend: beide behandeld, rekenmodel op **FDM/PLA**.
3. Modelvolume ±200 cm³ bij 12 cm; grammen, print- en schildertijden zijn **eigen schattingen**.
4. Rekentarief **€ 15/uur**, printervergoeding **€ 0,50/printuur** (plaatshouder), **5 beeldjes per maand**, 1 USD = € 0,87.
5. Uit je eigen notities en de Shopify-koppeling: eenmanszaak al bij KVK, **21% btw zonder KOR**, betalen via **Mollie op Shopify Basic** (Shopify rekent dan 2% extra).
6. Prijzen incl. verzending NL (PostNL € 6,35); België + € 6.
7. CSV's met puntkomma en decimale komma, zodat Nederlandse Excel ze direct goed opent.

## Open punten

- Officiële prijspagina's van Meshy, Tripo en Rodin niet gelezen; **Tripo-prijs en Rodin-licentie niet geverifieerd**.
- Geen Nederlandse prijs gevonden voor vernis, Mr. Surfacer, schuurpapier en handschoenen; de wet palette en de resin bij 123-3D waren uitverkocht.
- Weinig reviews en levertijden van kleine aanbieders gevonden.
- Controleer op je Shopify-factuur of de 2% extra echt wordt gerekend; Shopify Payments kan goedkoper zijn.
- Kies hoe klanten foto's uploaden (app of formulier) en stel de levertijd vast na de test.
- Laat de tekst over geen bedenktijd en het GPSR-etiket eventueel juridisch checken.
- **De repo Yoooo is openbaar.** Het rapport bevat zakelijke uitgangspunten (btw, betaalprovider). Een eerdere commit bevatte een paar details uit je notities (o.a. een uitbetalingsbedrag); die zijn eruit gehaald, maar staan nog in de git-geschiedenis. Overweeg de repo privé te maken.

## Wat je als eerste doet

1. **Werkgever:** vraag schriftelijk toestemming voor de printer, vraag welk type het is (FDM of resin) en spreek een vergoeding af (rapport §6.4).
2. **Vriend:** spreek een vast bedrag per beeldje af op één A4 (§5.4, §6.5) en bestel het uitgeklede schilderpakket (± € 78, §8.1).
3. **Proefbeeldje:** maak met het gratis Meshy-plan een model van een eigen of bekend dier, print 12 cm, laat het schilderen en meet de tijd. Zet daarna de productpagina live met een introductieprijs voor de eerste 5 bestellingen (§8.2).
