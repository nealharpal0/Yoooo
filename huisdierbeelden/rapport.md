# Handbeschilderde 3D-geprinte huisdierbeeldjes – verkenning

Opgesteld in de nacht van 4 op 5 november 2026. Bronnen geraadpleegd op 4–5 november 2026; de URL's staan per deel in de [bijlage](#bijlage-bronnen-per-deel).

> **Beperking.** WebFetch werkte in deze omgeving niet (elke site gaf een DNS-fout). Alle feiten komen uit zoekresultaten van WebSearch, die een korte samenvatting van de pagina's geven; de pagina's zelf zijn dus niet volledig gelezen. Waar bronnen elkaar tegenspreken of niets is gevonden, staat dat erbij ("niet geverifieerd"). Bedragen zonder bron zijn eigen schattingen en staan zo vermeld.

## Inhoud

1. [Van foto naar 3D-model](#1-van-foto-naar-3d-model)
2. [Printen om te beschilderen](#2-printen-om-te-beschilderen)
3. [Beschilderen](#3-beschilderen)
4. [Markt en concurrenten](#4-markt-en-concurrenten)
5. [Kostprijs, verkoopprijs en verdeling](#5-kostprijs-verkoopprijs-en-verdeling)
6. [Regels en praktische punten](#6-regels-en-praktische-punten)
7. [Productpagina](#7-productpagina)
8. [Advies: 5 testbeeldjes deze maand](#8-advies-5-testbeeldjes-deze-maand)

[Bijlage: bronnen per deel](#bijlage-bronnen-per-deel)

---

## 1. Van foto naar 3D-model

### 1.1 Drie routes

| Route | Werkt voor huisdieren? | Kosten per model | Commercieel gebruik |
|---|---|---|---|
| **AI image-to-3D** (Meshy, Tripo, Rodin): foto's uploaden, model in minuten | Ja, mits goede foto's; nabewerking bijna altijd nodig | Meshy Pro $20/mnd voor 1.000 credits; één model met textuur ±30–35 credits (±$0,60–0,70 per poging) | Meshy: betaald plan = eigen bezit; gratis plan = CC BY 4.0 met naamsvermelding |
| **Fotogrammetrie** (Polycam, KIRI Engine): tientallen foto's rondom een stilstaand onderwerp | Slecht: het dier moet stil blijven en vacht geeft weinig houvast | KIRI basis gratis; Polycam Pro $26,99/mnd (App Store, april 2026) | Niet geverifieerd |
| **Freelance modelleur** (Fiverr, Etsy) | Beste controle over houding en karakter | Fiverr-sculpts vanaf ±$30–57 (categorie printklare figuren $100–120); pet-STL op Etsy ±$10–47 | Per opdracht vastleggen |

### 1.2 AI image-to-3D in de praktijk

- **Kwaliteit.** In een praktijktest van 3DWithUs maakte Meshy van één hondenfoto een herkenbaar beeldje; bij Tripo hielp een "Refine"-stap bij vacht en staart. Onafhankelijke tests zijn schaars.
- **Typische fouten:** gaten in de mesh, te dunne poten, zeer zware mesh. Oplossen met de repairfunctie van 3D Builder, Meshmixer of de slicer, dunne delen 0,5–1 mm dikker maken en vereenvoudigen in Blender. Een **voetstuk** voorkomt de meeste breuk (eigen advies).
- **Meshy:** image-to-3D 20–25 credits plus 10 voor textuur (handig als kleurvoorbeeld). "Multi-View" (alleen betaald): hoofdfoto plus maximaal 3 hoeken, 45–90° uit elkaar, achtergrond verwijderd.
- **Tripo:** Professional 3.000 credits/mnd; prijs **niet geverifieerd** ($11,94–19,90). Gratis modellen volgens de meeste bronnen niet commercieel. **Rodin:** commerciële licentie expliciet alleen bij Business → **niet geverifieerd**. **Bambu MakerLab:** verkoop van de uitvoer **onduidelijk** → alleen oefenen.
- **Open-source:** de licentie van Hunyuan3D 2.0/2.1 geldt **niet in de EU**. TRELLIS is MIT (commercieel toegestaan) maar vraagt een NVIDIA-kaart met 24 GB.

### 1.3 Fotogrammetrie en freelancers

Fotogrammetrie vraagt een **stilstaand** onderwerp (een maker scande een cavia met ±60 losse foto's) en is voor klanten op afstand onbruikbaar. Een freelancer is de reserve voor dieren waar AI faalt; leg dan commercieel gebruik, revisies en levertijd vast.

### 1.4 Wat de klant aanlevert

Afgeleid van Meshy's Multi-View-richtlijnen plus wat de schilder nodig heeft (minimaal 3, liefst 5–8 foto's):

1. **Voorkant** op ooghoogte, hele dier in beeld.
2. **Zijkant links en rechts** (90°), in de gewenste houding.
3. **Achterkant** of schuin achter (rug en staart).
4. **Close-up van de kop** (ogen, neus, oren).
5. **Elke aftekening** apart (bles, sokjes, vlekken).
6. Daglicht, geen flits of filter, scherp, rustige achtergrond, origineel bestand.

**Advies:** Meshy Pro voor een maand ($20), vaste werkwijze: foto's → model → repareren en voetstuk → printen. Reken 2–4 generaties per dier en 30–60 minuten nabewerking (eigen schatting).

---

## 2. Printen om te beschilderen

### 2.1 FDM of resin?

| | FDM (filament, PLA) | Resin (MSLA, vloeibare hars) |
|---|---|---|
| Laagdikte | 0,08–0,2 mm; 0,08–0,12 mm is gangbaar voor figuren | 0,01–0,05 mm |
| Detail | Kenmerken < ±0,5 mm vervagen; laaglijnen zichtbaar | Vacht, ogen en neus blijven scherp |
| Nabewerking | Steunen weg, schuren, filler primer (meer werk) | Wassen in IPA, naharden onder UV, licht schuren |
| Gezondheid | Ventileren; hogere temperatuur geeft meer fijnstof | Hars kan huidallergie geven; ventilatie, nitrilhandschoenen, bril; IPA is brandbaar |
| Sterkte en tijd | Taai; tijd hangt af van volume | Broos; tijd hangt af van hoogte, dus meerdere beeldjes tegelijk |

**Advies:** FDM met 0,08–0,12 mm en een stevig voetstuk is goed genoeg om te beschilderen, mits er filler primer op gaat. Heeft je werk een resinprinter in een goed geventileerde ruimte, dan krijg je mooier detail en minder schuurwerk.

### 2.2 Gezondheid en ventilatie bij resin

- Het **RIVM** (2016) noemt de risico's van 3D-printen in huis moeilijk in te schatten en goede ventilatie belangrijk; **EU-OSHA** behandelt hars als gevaarlijke stof op de werkplek.
- Vloeibare hars en verse prints alleen met **nitrilhandschoenen** (geen latex), **oogbescherming** en goede **ventilatie**: ruik je hars, dan is het onvoldoende. "Waterwasbare" hars is niet minder giftig. Lees het veiligheidsinformatieblad, vang IPA en harsresten op en volg de arboregels van je werkgever.

### 2.3 Formaten, printtijd en materiaal

**Aannames (eigen schatting):** zittende hond of kat met voetstuk, ±200 cm³ massief bij 12 cm; volume schaalt met de derde macht van de hoogte (8 cm ≈ 0,3×, 15 cm ≈ 2×). Resin vanaf 12 cm hol (2 mm wand, minstens twee afvoergaten). Resin: lagen van 0,05 mm à 6–10 s (belichting ±2,7 s plus platformbeweging).

| Formaat | FDM filament / tijd | Resin hars / tijd | Materiaal FDM | Materiaal resin (incl. IPA e.d.) |
|---|---|---|---|---|
| 8 cm | 20–40 g / 1,5–3 u | 25–35 g / 2,5–4,5 u | € 0,50–1,10 | € 1,10–2,70 |
| 12 cm | 60–120 g / 4–8 u | 50–70 g / 4–7 u | € 1,30–3,20 | € 1,80–4,40 |
| 15 cm | 120–230 g / 7–14 u | 80–100 g / 5–8,5 u | € 2,70–6,10 | € 2,50–5,80 |

Ter vergelijking: MakerWorld-figuren van ±12 cm noemen 2,2 uur (16 g) tot ±5 uur (126 g). Vervang de schattingen door slicerwaarden.

**Prijzen (incl. btw):** grijs PLA 1 kg € 22,25 (2-pack 123-3D) tot € 26,50 → ± € 0,02–0,03 per gram. Elegoo Standard Resin grijs 1 kg € 47,50 (123-3D, uitverkocht bij raadplegen) of € 22,80 (Kubii, Frankrijk) → ± € 0,025–0,05 per gram. Grijs of wit is het handigst onder verf.

### 2.4 Nabewerking

**Steunen weg** (zijkniptang; resin eerst wassen, dan naharden) → **schuren** van hoge punten (korrel 120–220; primer verbergt ze niet) → **filler primer** (bijv. Mr. Surfacer 500/1000 of autofiller) en nat schuren (320–600), zo nodig herhalen; ruw PLA schuurt slecht, dus eerst filler → **eindprimer**. Reken ±20–40 minuten (FDM) of ±15–25 minuten (resin) per beeldje, exclusief droogtijd (eigen schatting).

---

## 3. Beschilderen

### 3.1 Methode en lagen

**Begin met het penseel**: goedkoop en ideaal voor ogen, neus en aftekeningen. Een **airbrush** geeft snelle, egale grondlagen en zachte overgangen, maar vraagt een investering en oefening (verdunnen, druk, nevel) en maakt je niet vanzelf sneller; overweeg die pas na 5–10 beeldjes. Veel schilders combineren: airbrush voor de basis, penseel voor detail.

Opbouw: filler primer (FDM) → primer (grijs; wit voor lichte, zwart voor donkere dieren) → basiskleuren in acrylverf → schaduw met speedpaint/wash en licht met **droogborstelen** (vacht) → details (ogen, neus, halsband; een glanspuntje in de ogen) → **matte vernis**, eventueel glans op ogen en neus. De vachttechnieken zijn gangbaar in de miniatuurhobby, maar niet specifiek door de bronnen bevestigd: laat je vriend ze op een proefprint testen.

### 3.2 Startpakket voor je vriend

Volledige lijst met winkels en URL's in [`startpakket.csv`](startpakket.csv) (puntkomma's, decimale komma). Prijzen incl. btw, gevonden op 4 november 2026:

| Pakket | Inhoud | Totaal |
|---|---|---|
| **Basis** | Warpaints Starter Set € 34,00 (De Dondersteen), Hobby Starter Brush Set € 15,99, Wet Palette € 21,95 (uitverkocht), Vallejo Surface Primer € 12,99 (123-3D), Motip primer-spuitbus € 4,99 (Hubo BE), Motip filler € 13,37 (Nonpaints), Vallejo matte vernis € 9,49 (Letse webshop; geen NL-prijs gevonden), Hobby Tool Kit € 31,93 | **± € 145** |
| **+ Speedpaint** | Speedpaint Starter Set 2.0 € 39,99 (officiële NL-webshop) | ± € 185 |
| **+ Airbrush** | Revell Airbrush Basic Set met compressor € 99,95 (Toemen) | ± € 285 |

Schuurpapier, handschoenen en stofmasker: prijs niet geverifieerd. Zelfgemaakte wet palette en losse zijkniptang en hobbymes: ± € 90–100 (eigen schatting).

### 3.3 Schildertijd

Geen bron voor huisdierbeeldjes. IJkpunten uit hobbyfora: een 28 mm-figuur 1,5–3 uur, een gangbare opdracht 4–6 uur, een 75 mm-figuur grofweg 5–10 uur. **Eigen schatting** voor iemand met wat ervaring, exclusief droogtijd: **8 cm 1,5–2,5 uur, 12 cm 2,5–4 uur, 15 cm 3,5–5 uur**. Reken voor de eerste 5 beeldjes het dubbele en laat je vriend de tijd bijhouden.

### 3.4 Kleuren en aftekeningen vastleggen

Bijna alle aanbieders van huisdierportretten sturen eerst een **foto ter goedkeuring**, vaak met één gratis correctie. Een vaste kleurprocedure vond ik niet; voorstel:

1. **Intakeformulier**: ras, vachtkleuren, kleur ogen en neus, kenmerken (bles, sokjes, vlekken), halsband ja/nee; plus de foto's uit 1.4.
2. **Aftekeningenkaart**: silhouet (voor, zij, achter, boven) waarop de klant vlekken intekent.
3. **Goedkeuring 1**: foto van het grijze model vóór het printen. **Goedkeuring 2**: foto van het geschilderde beeldje in daglicht vóór de vernis, met één kleine correctie inbegrepen.
4. **Vastleggen** welke verf en mengverhouding is gebruikt, voor nabestellingen.

---

## 4. Markt en concurrenten

Volledige lijst (15 aanbieders, met formaat, prijs, levertijd en reviews) in [`concurrenten.csv`](concurrenten.csv). Prijzen zijn momentopnames; levertijden en reviews ontbraken bij veel kleine webshops.

| Segment | Voorbeelden | Prijs (±10–12 cm) |
|---|---|---|
| **Onbeschilderd, één kleur** | Solid Memories, 3D Huisdier, Verrassingsdoos (NL) | € 25–60; Solid Memories 8 cm € 15,99 / 12 cm € 29,99 / 16 cm € 39 |
| **Handbeschilderde 3D-print** | Atelier Robijns (BE), Etsy-verkopers, Minipiece (NL) | € 45–55; Etsy ± $25–65 |
| **Handgeboetseerd** | Klischklick (DE) | € 126 (5–10 cm, incl. verzending) |
| **Meerkleurige FDM-print** | 3d-druck-scan.com, Figuroo (DE) | € 80–200; Figuroo € 25–120 |
| **Full-colour print (vergelijking)** | Youlittle, machmich3d (DE), DoubleMe3d (NL), My3DSelfie, Cuddle Clones (VS) | € 149–420; Cuddle Clones ± $99–129 (4 inch) |

**Observaties**
- De directe concurrent zit **laag**: Atelier Robijns (BE) vraagt € 44,95 voor ±10 cm handbeschilderd, met 15–20 werkdagen productietijd. Onbeschilderde prints beginnen bij € 16.
- **Full-colour printen** (vaak via scan, gips of zandsteen) kost € 149–420 voor 5–10 cm: handbeschildering is een goedkoper alternatief, maar klanten betalen bij concurrenten niet veel extra voor "met de hand".
- Gevonden **levertijden**: 15–20 werkdagen (Atelier Robijns), 3–5 weken (My3DSelfie). Twee à drie weken is concurrerend.

**Reviews** (weinig onafhankelijke reviews over deze kleine aanbieders):
- **Gewaardeerd:** gelijkenis met het eigen dier (Herdenkingsbeeldje.nl, My3DSelfie, Etsy), meedenken en een prototype kunnen aanpassen (My3DSelfie, PetPalsDIY), goedkeuring vóór verzending.
- **Gemist:** prijs/waarde bij dure full-colour beeldjes (My3DSelfie, Trustpilot UK), "generieke koppen met een beetje verf" in plaats van het eigen dier (PetPalsDIY), een geprinte foto in plaats van verwacht handwerk (Petsies), langere levertijd dan beloofd (verwante herdenkingswebshops).

**Les:** beloof alleen wat je waarmaakt, laat foto's van eigen werk zien en bouw twee goedkeuringsmomenten in.

---

## 5. Kostprijs, verkoopprijs en verdeling

Rekenmodel: [`kostprijs.csv`](kostprijs.csv). Pas de aannames aan zodra je echte slicer- en schildertijden hebt.

### 5.1 Uitgangspunten

- **Btw:** je eenmanszaak (met Pootjespret) staat al bij KVK en rekent **21% btw zonder KOR** (eigen notities); het model trekt 21% van de verkoopprijs af. Kosten staan incl. btw (voorzichtig; met facturen ±17% lager).
- **Productie:** FDM/PLA + 15% misdrukken; Meshy Pro $20/mnd (1 USD ≈ € 0,87, aanname) over **5 beeldjes per maand**; printer werkgever **€ 0,50 per printuur** (plaatshouder, zie 6.4).
- **Verzending:** PostNL pakket tot 3 kg NL € 6,35 (tarieven vanaf 12 juli 2026); België € 12,25, dus € 6 toeslag. Prijzen zijn incl. verzending NL.
- **Betalen:** Mollie op **Shopify Basic**; Shopify rekent volgens bronnen **2% extra** bij een externe betaalprovider; Mollie iDEAL € 0,29–0,32, kaart 1,8% + € 0,25. Model: **2% + € 0,39**.
- **Arbeid:** eigen tijd 1,25–1,75 u, schildertijd 2–4,25 u; rekentarief **€ 15/uur** (aanname, geen loon).

### 5.2 Kostprijs per beeldje

| | 8 cm | 12 cm | 15 cm |
|---|---|---|---|
| 3D-model (Meshy, 5/mnd) | € 3,48 | € 3,48 | € 3,48 |
| Filament incl. misdrukken | € 0,83 | € 2,48 | € 4,83 |
| Filler, primer, verf, vernis | € 1,00 | € 1,50 | € 2,00 |
| Printervergoeding (aanname) | € 1,12 | € 3,00 | € 5,25 |
| Verpakking | € 2,00 | € 2,25 | € 2,50 |
| Verzending NL | € 6,35 | € 6,35 | € 6,35 |
| **Directe kosten** | **€ 14,78** | **€ 19,06** | **€ 24,41** |
| Arbeid (uren × € 15) | € 48,75 | € 71,25 | € 90,00 |
| **Kostprijs incl. arbeid** (excl. btw en betaalkosten) | **€ 63,53** | **€ 90,31** | **€ 114,41** |

**Arbeid is 75–80% van de kostprijs**; materiaal is bijna verwaarloosbaar.

### 5.3 Drie prijsniveaus (incl. 21% btw en verzending NL)

| Niveau | 8 cm | 12 cm | 15 cm | Marge excl. arbeid (12 cm) | Per arbeidsuur | Break-even |
|---|---|---|---|---|---|---|
| **Laag** (gelijk aan Atelier Robijns/Etsy) | € 49 | € 65 | € 79 | € 32,97 | ± € 6,50–7,50 | 6 stuks |
| **Midden** | € 59 | € 79 | € 99 | € 44,26 | ± € 9–10 | 5 stuks |
| **Hoog** (naamplaatje, 2 correctierondes, cadeauverpakking) | € 75 | € 99 | € 125 | € 60,38 | ± € 12,50–14 | 4 stuks |

- **Marge excl. arbeid** = prijs − btw − directe kosten − betaalkosten; dit verdelen jullie. **Break-even** = vaste startkosten ± € 192 (startpakket € 145, proefprints € 25, PLA € 22) / marge, bij een mix 25/50/25% van 8/12/15 cm: dan zijn de uitgaven terug, de uren nog niet.
- **Op geen enkel niveau** zijn de uren betaald tegen € 15; daarvoor moet 12 cm naar ± € 120 of moet de tijd omlaag (speedpaint, vaste houdingen).
- **Etsy** kost € 6,67–10,87 per verkoop (6,5% + 4% + € 0,30 + $0,20) tegen € 1,57–2,37 via Pootjespret. Shopify Payments i.p.v. Mollie scheelt de extra 2% (niet gecontroleerd of dat voor jou kan).

**Advies:** na een introductieprijs op laag niveau voor de eerste 5 testbeeldjes (zie 8) ga je naar **middenniveau** (12 cm € 79); meet de echte uren en ga naar **hoog** zodra de kwaliteit vaststaat. Concurreer niet met onbeschilderde prints (€ 16–40).

### 5.4 Opbrengst verdelen met je vriend

Bij middenniveau (marge excl. arbeid: 8 cm € 32,41; 12 cm € 44,26; 15 cm € 55,04):

| | 8 cm | 12 cm | 15 cm |
|---|---|---|---|
| **Optie 1: vast bedrag** voor de schilder | € 20 (€ 10,00/u) | € 27 (€ 8,31/u) | € 33 (€ 7,76/u) |
| → rest voor jou | € 12,41 (€ 9,93/u) | € 17,26 (€ 11,50/u) | € 22,04 (€ 12,59/u) |
| **Optie 2: winstdeling 50/50** (ieder) | € 16,20 | € 22,13 | € 27,52 |
| **Optie 2b: winstdeling naar uren**: schilder / jij | € 19,94 / € 12,46 | € 30,28 / € 13,98 | € 38,99 / € 16,05 |

- **Vast bedrag** – voordelen: simpel, zekerheid voor je vriend, jij houdt zeggenschap, weinig administratie, het blijft jouw onderneming. Nadelen: jij draagt het risico; je vriend profiteert niet mee van hogere prijzen.
- **Winstdeling** – voordelen: gedeeld risico en motivatie, je vriend profiteert mee. Nadelen: open boekhouding nodig, uitkomst wisselt, bij 50/50 weinig per uur voor de schilder, en samen ondernemen kan een **vof** zijn met aansprakelijkheid met privévermogen (6.5).

**Advies:** begin met **vast bedrag per beeldje**; evalueer na 10–20 beeldjes en stap eventueel over op **winstdeling naar uren**. Leg vast wie mislukte of afgekeurde beeldjes betaalt.

---

## 6. Regels en praktische punten

> Geen juridisch of fiscaal advies; laat twijfelgevallen toetsen door Belastingdienst, KVK of een adviseur.

### 6.1 Inschrijving, btw en belasting

- **KVK:** inschrijving is nodig bij zelfstandig, tegen betaling en regelmatig leveren aan anderen dan familie en vrienden. Je eenmanszaak bestaat al; check of de activiteitenomschrijving beeldjes dekt.
- **21% btw.** Het 9%-tarief voor kunst geldt alleen voor werk dat helemaal door de kunstenaar zelf is gemaakt, niet voor serieproducten. Een kennisgroep van de Belastingdienst oordeelde dat **3D-geprinte (zwangerschaps)beeldjes** onder 21% vallen omdat de persoonlijke inbreng van de maker te klein is.
- **KOR** (omzet tot € 20.000/jaar): geen btw rekenen én niet aftrekken, minimaal 3 jaar, voor de **hele** eenmanszaak; nu niet in gebruik. **België:** onder € 10.000 afstandsverkopen per jaar reken je Nederlandse btw.
- **Je vriend:** zonder eigen bedrijf is de vergoeding "inkomsten uit overig werk", zelf op te geven in de aangifte (met Zvw-bijdrage; kosten mogen eraf). Met eigen bedrijf stuurt je vriend een factuur.
- **Uitbetaalde bedragen aan derden:** betalingen zonder btw-factuur moeten mogelijk worden doorgegeven (zonder personeel: op uitnodiging; bronnen tegenstrijdig). Noteer naam, adres, geboortedatum en bedrag.

### 6.2 Herroepingsrecht en betalen

- **Geen bedenktijd bij maatwerk.** Volgens de ACM geldt de bedenktijd van 14 dagen niet voor producten die volgens de specificaties van de klant zijn gemaakt of duidelijk persoonlijk zijn. Een beeldje van het eigen dier naar eigen foto's past daarin.
- De uitzondering is **smal**: kiezen uit standaardopties is niet genoeg en de verkoper moet aantonen dat het product aan niemand anders te verkopen is. **Meld** vóór de bestelling dat er geen bedenktijd is (vinkje), anders kan die tot een jaar worden verlengd.
- De **herroepingsknop** (verplicht sinds 25 juni 2026) blijft nodig voor de gewone producten. De **wettelijke garantie** blijft gelden (beschadigd of anders dan afgesproken).
- **Vooruitbetaling:** een consument kan niet verplicht worden meer dan **50%** vooruit te betalen. Laat klanten kiezen: alles vooraf of 50% aanbetaling en de rest na de goedkeuringsfoto.

### 6.3 Veiligheid en etikettering

- **GPSR** (sinds 13 december 2024, toezicht NVWA): wie onder eigen naam maakt en verkoopt, is **fabrikant**. Online moeten naam en postadres van de fabrikant, een productaanduiding en waarschuwingen zichtbaar zijn.
- **Geen speelgoed:** speelgoed is bedoeld voor spelen door kinderen onder 14. "Geen speelgoed" op het etiket is niet doorslaggevend; ontwerp en marketing tellen mee. Presenteer de beeldjes als **decoratie en herinnering voor volwassenen**.
- **Voorstel etiket** (onder het voetstuk en op de productpagina; formulering eigen advies): *Pootjespret – handgemaakt decoratief beeldje – geen speelgoed, niet geschikt voor kinderen onder 14 jaar; kleine delen kunnen afbreken – niet in contact met voedsel – afstoffen, niet nat reinigen – [postadres] – bestelnummer [xxx]*.
- Lever resinprints alleen volledig uitgehard en gewassen.

### 6.4 De printer van je werkgever

- **Nevenwerk** mag een werkgever sinds 1 augustus 2022 alleen verbieden met een objectieve reden (veiligheid, vertrouwelijke informatie, belangenverstrengeling). Meld het wel en check je contract; een concurrentiebeding blijft gelden.
- **De printer is van je werkgever:** vraag **schriftelijk** toestemming en leg vast wanneer (buiten werktijd, werkprints eerst), de vergoeding en wie materiaal betaalt (met factuur is de btw aftrekbaar), wie betaalt bij schade, veiligheid en afvoer bij resin, geen gebruik van bedrijfsinformatie, en een opzegtermijn. Plan B: eigen printer of printdienst (niet onderzocht).

### 6.5 Afspraken met je vriend op papier

- **Vast bedrag** = je vriend is opdrachtnemer; het blijft jouw onderneming. **Winstdeling en samen ondernemen** = al snel een **vof**: elke vennoot is met privévermogen aansprakelijk voor álle schulden. KVK raadt dan een samenwerkingscontract aan.
- **Op één A4:** taken, vergoeding per formaat en betaaltermijn, levertijd, kwaliteit en afkeur/herstel, wie het startpakket betaalt en bezit, omgang met klantfoto's en -gegevens, gebruik van foto's van het werk, naamsvermelding, stoppen.
- **Jonger dan 18?** Dan is toestemming van een ouder of voogd nodig; een contract zonder toestemming kan worden teruggedraaid (handlichting kan vanaf 16 jaar).

### 6.6 Foto's van klanten en privacy

- De maker van een foto heeft het **auteursrecht**: laat de klant bevestigen dat jij de foto's mag gebruiken voor het beeldje, en vraag **aparte toestemming** voor website of social media. Herkenbare mensen zijn persoonsgegevens; vraag foto's van alleen het dier.
- Meld in je privacyverklaring dat een externe 3D-tool de foto's verwerkt en gebruik een **betaald** Meshy-plan (gratis modellen vallen onder CC BY 4.0).

---

## 7. Productpagina

Concepttekst in [`productpagina.md`](productpagina.md), in de huisstijl van Pootjespret. Bevat: kop en intro, formaten en prijzen (middenniveau), bestelflow in 6 stappen (formaat → foto's uploaden → vachtformulier en aftekeningenkaart → goedkeuring model → schilderen en goedkeuring kleur → verzenden), foto-tips, levertijd als invulveld (voorstel ±3 weken), "goed om te weten" (handwerk, geen bedenktijd, betaalkeuze, geen speelgoed, onderhoud, fabrikantgegevens), veelgestelde vragen, verplichte vinkjes en notities voor de inrichting in Shopify. Er staan geen reviews, klantaantallen of verzonnen garanties in.

---

## 8. Advies: 5 testbeeldjes deze maand

**Doel:** in november 5 beeldjes maken én verkopen, zo goedkoop mogelijk, om echte tijd, kosten en reacties te meten.

### 8.1 Goedkoopste opzet

| Onderdeel | Keuze | Kosten (incl. btw) |
|---|---|---|
| 3D-model | 1–2 proeven op het gratis Meshy-plan met een eigen huisdierfoto (niet verkopen); daarna **Meshy Pro één maand** voor de 5 klantmodellen, en opzeggen | ± € 17 ($20) |
| Printen | **FDM op de printer van je werk** (na schriftelijke toestemming), grijs PLA, alleen **8 en 12 cm**, 0,12 mm, met voetstuk | rol PLA € 22,25 (±10 beeldjes van 12 cm) + vergoeding werkgever |
| Schilderen | **Uitgekleed pakket**: Warpaints Starter Set € 34, penselen € 15,99, Motip-primer € 4,99, Motip filler € 13,37, vernis € 9,49; wet palette zelf maken; zijkniptang en hobbymes los | ± € 78 (+ gereedschap, niet geverifieerd) |
| Verkopen | **Pootjespret** + eigen netwerk en de Pootjespret-socials; geen Etsy in de test | € 0 extra; betaalkosten ± € 1,60–2 per stuk |
| Verzenden | Lokaal zelf afgeven waar het kan; anders PostNL | € 0–6,35 per stuk |
| Verpakking | Doos, vulmateriaal, kaartje | ± € 2 per stuk |
| Je vriend | Ook in de test een vast bedrag, bijv. € 15–20 per beeldje | € 75–100 |
| **Totaal** | eenmalig ± € 117 + per stuk ± € 5–13 + je vriend | **± € 220–280** |

Met een **introductieprijs van € 49 (8 cm) / € 65 (12 cm)** levert 5 beeldjes ± € 200–270 excl. btw op: **ongeveer quitte tot ± € 80 tekort**, maar je houdt het schilderpakket en een halve rol PLA over en vanaf beeldje 6 vallen de eenmalige kosten weg. Noem het eerlijk een introductieprijs voor de eerste 5 bestellingen, in ruil voor feedback en (met toestemming) foto's, zonder nep-"van"-prijs (de ACM let op misleidende kortingen).

### 8.2 Planning november

| Week | Wat |
|---|---|
| **Wk 45 (5–8 nov)** | Schriftelijke toestemming werkgever en printertype vaststellen; afspraak met je vriend op papier; pakket en PLA bestellen; proefmodel maken en printen |
| **Wk 46 (9–15 nov)** | Productpagina live ("eerste 5 plekken"); 5 klanten werven; foto's en formulieren binnen; Meshy Pro afsluiten; modellen ter goedkeuring sturen |
| **Wk 47 (16–22 nov)** | Printen en nabewerken; je vriend schildert en houdt de tijd bij |
| **Wk 48 (23–29 nov)** | Goedkeuringsfoto's, correcties, vernissen, verzenden of afgeven |
| **30 nov** | Evaluatie: echte uren en kosten in `kostprijs.csv`, feedback ophalen, prijs en levertijd voor december vaststellen |

### 8.3 Beslisregels na de test

- **Doorgaan** als klanten hun dier herkennen, een 12 cm-beeldje samen minder dan ±5 uur kost en minstens de helft het voor de normale prijs zou kopen of aanraden; dan **prijs omhoog** naar midden of hoog.
- **Proces aanpassen** als AI-modellen vaak mislukken (vaste houdingen, meer foto's, freelancer). **Stoppen of anders inrichten** als de printer wegvalt of schilderen veel langer duurt.

---

## Bijlage: bronnen per deel

Alle bronnen geraadpleegd op 4–5 november 2026 via zoekresultaten van WebSearch (de pagina's zelf konden niet worden geopend, zie de opmerking bovenaan).

**Deel 1**
- Meshy prijzen: https://www.meshy.ai/pricing ; credits: https://docs.meshy.ai/en/webapp/pricing ; API-prijzen: https://www.meshy.ai/api
- Meshy licentie: https://help.meshy.ai/en/articles/9992001-can-i-use-my-generated-assets-for-commercial-projects ; https://help.meshy.ai/en/articles/10137554-what-is-the-ownership-of-the-generated-models
- Meshy Multi-View: https://intercom.help/meshy/en/articles/12634481-how-to-use-multi-view ; https://www.meshy.ai/tutorials/multi-view-image-to-3d
- Tripo: https://www.tripo3d.ai/help/billing/which-tripo-ai-plan-is-right-for-me ; https://www.tripo3d.ai/blog/commercial-use-ai-3d-models ; https://costbench.com/software/ai-3d-generation/tripo-ai/
- Rodin: https://hyper3d.ai/pricing ; https://blog.picassoia.com/rodin-gen-2-5-hyper3d-image-to-3d-pricing-and-quality
- Praktijktests: https://3dwithus.com/meshy-ai-hands-on-review-photo-to-3d-printing ; https://3dwithus.com/tripo-ai-review-3d-printing
- Mesh-reparatie: https://printpal.io/wiki/preparing-ai-models-for-3d-printing ; https://www.3daistudio.com/3d-generator-ai-comparison-alternatives-guide/can-i-3d-print-ai-generated-models
- MakerLab: https://cms.abduzeedo.com/node/89211 ; https://forum.bambulab.com/t/maker-lab-commercial-purposes/87539
- Hunyuan3D-licentie: https://huggingface.co/tencent/Hunyuan3D-2/blob/main/LICENSE ; TRELLIS: https://huggingface.co/JeffreyXiang/TRELLIS-image-large ; https://comfyui-wiki.com/en/models/trellis/trellis-2
- Fotogrammetrie: https://sites.google.com/view/vizproto/directory/mary-kate-mccormick/mkm-pet-portrait-using-3d-data-capture ; https://arxiv.org/html/2510.24117v1 ; https://www.kiriengine.app/FAQ ; Polycam: https://apppricinglab.com/iap/apple/1532482376
- Freelance: https://www.fiverr.com/gigs/3d-animal-sculpt ; https://www.fiverr.com/categories/graphics-design/buy/character-modeling/3d-printing ; https://www.etsy.com/market/custom_pet_sculpture

**Deel 2**
- FDM vs resin: https://jlc3dp.com/blog/resin-vs-fdm-for-miniatures ; https://blog.lootstudios.com/print/the-ultimate-fdm-versus-resin-guide/ ; https://www.3dsourced.com/guides/resin-vs-fdm-for-3d-printing-miniatures/
- RIVM: https://www.rivm.nl/publicaties/risicos-van-3d-printen-in-consumentenomgeving-technieken-materialen-en-producten ; EU-OSHA: https://osha.europa.eu/nl/publications/replacing-hazardous-resin-3d-printing-make-moulds ; BfR: https://www.bfr.bund.de/cm/349/3d-printing-a-dusty-business.pdf
- Resin-veiligheid: https://ameralabs.com/?p=30319 ; https://jlc3dp.com/blog/resin-hazards ; VOC-studie: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12848961/
- Printtijd resin: https://www.fabbaloo.com/news/prusa-reveals-how-they-sped-up-msla-3d-printing ; https://cults3d.com/:4019929 ; FDM-voorbeelden: https://makerworld.com/models/2911139 ; https://makerworld.com/models/1308641
- Hol printen: https://blog.lootstudios.com/print/hollow-vs-solid-3d-models/ ; https://3dprinterly.com/how-to-hollow-resin-3d-prints-properly/
- Prijzen: https://www.123-3d.nl/123-3D-Filament-PLA-Grijs-1-75-mm-2-pack-1-kg-i12218.html ; https://www.123inkt.nl/123-3D-Filament-PLA-Marmer-Grijs-1-75-mm-1-kg-i110111.html ; https://www.123-3d.nl/Elegoo-Standaard-resin-Grijs-1-kg-14-0007-61B-i8552.html ; https://www.kubii.com/en/consumable-materials/4594-standard-colored-resin-1-kg-for-3d-printer-3272496322394.html
- Filler primer: https://forums.kitmaker.net/t/filling-3d-ripples/33574 ; https://plastmodel.pl/en/products/7173-mr-surfacer-1000-sf-284 ; https://evezone.evetech.co.za/build-lab/how-to-finish-3d-printed-props-sand-fill-prime-and-paint

**Deel 3**
- Penseel vs airbrush: https://tistaminis.com/blogs/blog/airbrush-vs-brush-when-each-wins-for-miniatures-painting ; https://www.scalemodelshop.co.uk/paint-brushes-vs-airbrush-scale-models/ ; https://www.wargamer.com/the-best-airbrush-for-miniatures
- Schildertijd: https://cypaint.com/article/how-to-prices-a-commission-miniature-painting ; https://www.coolminiornot.com/forums/threads/how-long-do-you-spend-on-a-figure.10345/
- Goedkeuringsfoto's: https://www.riverry.com/products/mini-custom-watercolor-pet-portrait-cat-46341 ; https://madeit.com.au/products/handmade-custom-pet-plush-from-photo-pet-keepsake-ornament-memorial-gift-stellar-craft ; https://etsy.com/shop/SiennaPetPortraits
- Prijzen startpakket: zie URL's in `startpakket.csv` (o.a. https://de-dondersteen.nl/products/the-army-painter-warpaints-starter-paint-set ; https://www.123-3d.nl/Vallejo-Surface-Primer-Grey-200-ml-74601-i9597.html ; https://www.toemen.nl/en/product/revell-airbrush-basic-set-with-compressor-version-2023)

**Deel 4**
- NL/BE: https://solidmemories.nl/ ; https://3dhuisdier.nl/ ; https://www.minipiece.nl/producten/huisdieren-1 ; https://verrassingsdoos.com/shop/3d-beeldje-van-foto ; https://doubleme3d.nl/3d-dieren/ ; https://duplify.nl/3d-sculptuur-huisdier/ ; https://www.atelierrobijns.be/product/3d-print-van-je-huisdier/ ; https://dk.trustpilot.com/review/herdenkingsbeeldje.nl
- DE: https://figuroo.de/product/3d-avatar-hund-katze/ ; https://3d-druck-scan.com/produkt/3d-miniatur-figur-ihr-haustier-hund-katze-mehrfarbig/ ; https://youlittle.com/3d-figuren/preise/ ; https://machmich3d.de/produkt/3d-figur-haustiere/ ; https://www.klischklick.de/figuren/
- Internationaal: https://my3dselfie.com/nl-nl/products/urn-figurine-back ; https://uk.trustpilot.com/review/my3dselfie.com ; https://no.trustpilot.com/review/my3dselfie.com ; https://www.dogster.com/lifestyle/cuddle-clones-review/ ; https://www.etsy.com/market/custom_pet_figurine_from_photo ; https://www.etsy.com/market/hand_painted_dog_figurine
- Klachten: https://ca.trustpilot.com/review/petpalsdiy.com ; https://articles.hepper.com/petsies-custom-pet-plushies-review/ ; https://nl-be.trustpilot.com/review/herinnerdingendoos.nl

**Deel 5**
- Eigen gegevens: Shopify-koppeling (plan Basic, EUR), opgevraagd 4-11-2026; eigen notities over btw, KVK en betaalprovider (geraadpleegd 5-11-2026)
- Shopify 2% bij externe betaalprovider: https://www.trendtrack.io/nl/blog-post/hoeveel-rekent-shopify-per-verkoop-2026 ; https://sellfy.com/nl/blog/shopify-prijzen/ ; https://www.flatlineagency.com/nl/blog/shopify-payments-vs-externe-psps-verborgen-kosten-die-je-moet-kennen/
- Mollie-tarieven: https://www.zunapro.com/netherlands/nl/blog/ideal-betaalmethoden-nederland-online-verkopers ; https://comparepsp.pages.dev/providers/mollie/ ; https://www.emerce.nl/wire/mollie-introduceert-vast-tarief-bancontact
- Etsy-kosten: https://wisepim.com/tools/etsy-fee-calculator ; https://www.gelato.com/nl/blog/etsy-fees
- PostNL: https://www.postnl.nl/api/assets/blt43aa441bfc1e29f2/blt5e65605bca8690e0/tarievenboekje-12-juli-2026.pdf ; https://www.postnl.nl/api/assets/blt43aa441bfc1e29f2/blt4645e1ee01ff026a/tarievenfolder-2026b-EN.pdf
- Wisselkoers: https://tradingeconomics.com/euro-area/currency/news/498610 ; https://30rates.com/eur-usd-forecast-tomorrow-this-week
- Verpakking: https://hyperstack.viv.nl/kartonnen-dozen/verzendkokers

**Deel 6**
- KVK-criteria: https://www.kvk.nl/starten/moet-ik-mijn-bedrijf-inschrijven-bij-kvk/ ; ondernemer IB: https://www.belastingdienst.nl/wps/wcm/connect/bldcontentnl/belastingdienst/zakelijk/winst/inkomstenbelasting/wanneer_bent_u_ondernemer_voor_de_inkomstenbelasting/
- Btw-tarief kunst: https://www.belastingdienst.nl/wps/wcm/connect/bldcontentnl/belastingdienst/zakelijk/btw/tarieven_en_vrijstellingen/goederen_9_btw/kunst_verzamelvoorwerpen_antiek/kunstvoorwerpen/standbeelden_en_beeldhouwwerken ; 3D-geprinte beeldjes: https://kennisgroepen.belastingdienst.nl/publicaties/kg20920233-btw-tarief-levering-3d-geprinte-zwangerschapsbeeldjes/
- KOR: https://www.belastingdienst.nl/wps/wcm/connect/nl/btw/content/kor-voorwaarden ; afstandsverkopen: https://www.belastingdienst.nl/wps/wcm/connect/bldcontentnl/belastingdienst/zakelijk/btw/zakendoen_met_het_buitenland/afstandsverkopen-zoals-e-commerce-en-diensten-voor-particulieren-in-andere-eu-landen/afstandsverkopen-zoals-e-commerce-binnen-de-eu/
- Overig werk: https://www.belastingdienst.nl/wps/wcm/connect/nl/werk-en-inkomen/content/wat-zijn-inkomsten-uit-overig-werk ; uitbetaalde bedragen aan derden: https://www.belastingdienst.nl/wps/wcm/connect/bldcontentnl/belastingdienst/zakelijk/personeel_en_loon/uitbetaalde_bedragen_aan_derden/ ; https://gegevensportaal.belastingdienst.nl/ubd/faq/
- Bedenktijd: https://consument.acm.nl/aankoop-dienst-annuleren/bedenktijd ; https://www.acm.nl/nl/verkoop-aan-consumenten/klantenservice/bedenktijd ; https://www.acm.nl/nl/onderwerpen/verkoop-aan-consumenten/verkopen-aan-consumenten/checklist-verkoop-via-internet ; https://www.acm.nl/system/files/documents/definitief-besluit-openbare-waarschuwing-opslagplan.pdf ; https://consument.acm.nl/aankoop-dienst-annuleren/verplichte-informatie-bij-koop-product-dienst
- Vooruitbetaling: https://consument.acm.nl/rekeningen-en-incassoprocedures/wat-zijn-mijn-rechten-bij-een-aanbetaling ; https://www.acm.nl/nl/verkoop-aan-consumenten/de-koop-sluiten/betaalmogelijkheden-aanbieden
- GPSR: https://www.nvwa.nl/onderwerpen/gpsr-productveiligheidsverordening ; https://ondernemersplein.kvk.nl/gpsr-nieuwe-regels-voor-productveiligheid/ ; speelgoeddefinitie: https://zoek.officielebekendmakingen.nl/stcrt-2008-128-p28-SC86459.pdf ; https://resources.euconf.eu/casp/2022/NL/activity-reports/psa-1-toys-with-magnets-final-report/PSA1-Report-DS-03-23-169-NL-N.pdf
- Nevenwerk: https://www.kvk.nl/wetten-en-regels/verbod-op-nevenwerkzaamheden-alleen-met-goede-reden/ ; https://www.rijksoverheid.nl/documenten/2025/02/12/de-werking-van-het-verbod-op-het-nevenwerkzaamhedenbeding-in-de-praktijk
- Vof en samenwerkingscontract: https://www.kvk.nl/starten/de-vennootschap-onder-firma-vof/ ; https://www.kvk.nl/starten/samenwerkingscontract-voor-vof-maatschap-cv/
- Minderjarigen: https://ondernemersplein.kvk.nl/regels-voor-minderjarige-ondernemers/ ; https://www.kvk.nl/starten/handlichting-geen-18-toch-ondernemen/
- Auteursrecht en beeldmateriaal: https://ondernemersplein.kvk.nl/auteursrecht ; https://autoriteitpersoonsgegevens.nl/nl/onderwerpen/foto-en-film/beeldmateriaal ; Meshy-eigendom: https://help.meshy.ai/en/articles/10137554-what-is-the-ownership-of-the-generated-models

**Deel 8**
- Misleidende kortingen: https://consument.acm.nl/nieuws/acm-gaat-strenger-controleren-op-nepkortingen
- Overige bedragen: zie deel 2, 3 en 5 en `startpakket.csv` / `kostprijs.csv`

