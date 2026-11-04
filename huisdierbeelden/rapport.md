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

- **Kwaliteit.** In een praktijktest van 3DWithUs maakte Meshy van één hondenfoto een herkenbaar beeldje; houding en details bleven na het printen zichtbaar. Bij Tripo hielp een extra "Refine"-stap vooral bij vacht en staart. Onafhankelijke tests zijn schaars.
- **Typische fouten:** gaten in de mesh, omgekeerde vlakken, te dunne poten en een zeer zware mesh. Oplossing: automatisch repareren (3D Builder, Meshmixer of de slicer), dunne delen 0,5–1 mm dikker maken, mesh vereenvoudigen in Blender. Een **voetstuk** onder de poten voorkomt de meeste breuk (eigen advies).
- **Meerdere foto's.** Meshy "Multi-View" (alleen betaald): één hoofdfoto plus maximaal 3 extra hoeken, minstens 45–90° uit elkaar, liefst voor, zij en achter met de achtergrond verwijderd.
- **Credits Meshy.** Image-to-3D 20–25 credits plus 10 voor textuur (documentatie; de API-pagina noemt 20/30). Textuur is niet nodig voor de print, maar handig als kleurvoorbeeld.
- **Tripo:** Professional 3.000 credits/mnd (tot 200 modellen); prijs **niet geverifieerd** ($11,94–19,90 in bronnen). Gratis modellen volgens de meeste Tripo-pagina's niet commercieel; één blog zegt CC BY. **Rodin:** commerciële licentie expliciet alleen bij Business; andere sites zeggen anders → **niet geverifieerd**.
- **Bambu Lab MakerLab** (Meshy binnen MakerWorld): export kost 2 verdiende credits; of verkoop mag, is **onduidelijk** → alleen om te oefenen.
- **Open-source:** de licentie van Tencent Hunyuan3D 2.0/2.1 geldt **niet in de EU** → niet gebruiken. Microsoft TRELLIS is MIT (commercieel toegestaan), maar de nieuwste versie vraagt een NVIDIA-kaart met 24 GB.

### 1.3 Fotogrammetrie en freelancers

Fotogrammetrie vraagt een **stilstaand** onderwerp; zelfs ademhalen verstoort de reconstructie. Een maker scande een cavia met ±60 losse foto's, een ander een liggende hond. Voor klanten op afstand is dit onbruikbaar. Een freelancer is de reserve voor dieren waar AI faalt; leg dan vast dat je het bestand commercieel mag printen, hoeveel revisies inbegrepen zijn en wanneer het klaar is.

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
| Sterkte | Taai | Standaardhars is broos; dunne delen breken sneller |
| Printtijd | Hangt af van volume | Hangt af van hoogte; meerdere beeldjes tegelijk kost nauwelijks extra tijd |

**Advies:** FDM met 0,08–0,12 mm en een stevig voetstuk is goed genoeg om te beschilderen, mits er filler primer op gaat. Heeft je werk een resinprinter in een goed geventileerde ruimte, dan krijg je mooier detail en minder schuurwerk.

### 2.2 Gezondheid en ventilatie bij resin

- Het **RIVM** (2016) concludeert dat 3D-printen in huis risico's geeft waarvan de ernst niet goed vast te stellen is, en dat goede ventilatie belangrijk is (niet specifiek over hars). **EU-OSHA** behandelt hars als gevaarlijke stof op de werkplek.
- Gidsen en leveranciers zijn eensgezind: vloeibare hars en verse prints alleen met **nitrilhandschoenen** (geen latex; AmeraLabs: minimaal 0,15 mm), **oogbescherming** en vooral **ventilatie**. Ruik je hars, dan is de ventilatie onvoldoende. "Waterwasbare" hars is niet minder giftig.
- Lees het **veiligheidsinformatieblad** van de hars, vang IPA en harsresten op en volg de arboregels van je werkgever (zie 6.4).

### 2.3 Formaten, printtijd en materiaal

**Aannames (eigen schatting):** zittende hond of kat met voetstuk, ±200 cm³ massief bij 12 cm; volume schaalt met de derde macht van de hoogte (8 cm ≈ 0,3×, 15 cm ≈ 2×). Resin vanaf 12 cm hol (2 mm wand, minstens twee afvoergaten). Resin: lagen van 0,05 mm à 6–10 s (belichting ±2,7 s plus platformbeweging).

| Formaat | FDM filament / tijd | Resin hars / tijd | Materiaal FDM | Materiaal resin (incl. IPA e.d.) |
|---|---|---|---|---|
| 8 cm | 20–40 g / 1,5–3 u | 25–35 g / 2,5–4,5 u | € 0,50–1,10 | € 1,10–2,70 |
| 12 cm | 60–120 g / 4–8 u | 50–70 g / 4–7 u | € 1,30–3,20 | € 1,80–4,40 |
| 15 cm | 120–230 g / 7–14 u | 80–100 g / 5–8,5 u | € 2,70–6,10 | € 2,50–5,80 |

Ter vergelijking: op MakerWorld staan figuren van ±12 cm met 2,2 uur (16 g, slank) tot ±5 uur (126 g). Vervang de schattingen door slicerwaarden zodra je een echt model hebt.

**Prijzen (incl. btw):** grijs PLA 1 kg € 22,25 (2-pack 123-3D) tot € 26,50 → ± € 0,02–0,03 per gram. Elegoo Standard Resin grijs 1 kg € 47,50 (123-3D, uitverkocht bij raadplegen) of € 22,80 (Kubii, Frankrijk) → ± € 0,025–0,05 per gram. Grijs of wit is het handigst onder verf.

### 2.4 Nabewerking

1. **Steunen weg**: FDM met een zijkniptang ("tree supports" laten minder sporen na); resin eerst wassen, steunen weg, dan naharden.
2. **Schuren**: hoge punten en steunresten weg (korrel 120–220 bij FDM). Primer verbergt hoge punten niet, hij maakt ze juist zichtbaar.
3. **Filler primer** (bijv. Mr. Surfacer 500/1000 of een filler uit de autospuitbus) vult laaglijnen; daarna nat schuren (320–600) en zo nodig herhalen. Ruw PLA schuurt slecht, dus eerst filler, dan schuren.
4. **Eindprimer** in grijs, wit of zwart.

Reken ±20–40 minuten per beeldje bij FDM en ±15–25 minuten bij resin, exclusief droogtijd (eigen schatting).

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

Schuurpapier, handschoenen en stofmasker: prijs niet geverifieerd. Besparen kan door de wet palette zelf te maken (bakje, keukenpapier, bakpapier) en alleen een zijkniptang en hobbymes te kopen: dan ± € 90–100 (eigen schatting).

### 3.3 Schildertijd

Geen bron voor huisdierbeeldjes. IJkpunten uit hobbyfora: een 28 mm-figuur 1,5–3 uur, een gangbare opdracht 4–6 uur, een 75 mm-figuur grofweg 5–10 uur. **Eigen schatting** voor iemand met wat ervaring, exclusief droogtijd: **8 cm 1,5–2,5 uur, 12 cm 2,5–4 uur, 15 cm 3,5–5 uur**. Reken voor de eerste 5 beeldjes het dubbele en laat je vriend de tijd bijhouden.

### 3.4 Kleuren en aftekeningen vastleggen

Bijna alle aanbieders van huisdierportretten sturen eerst een **foto ter goedkeuring**, vaak met één gratis correctie. Een vaste kleurprocedure vond ik niet; voorstel:

1. **Intakeformulier**: naam en ras, vachtkleur(en), kleur ogen en neus, kenmerken (bles, sokjes, vlekken, scheurtje in een oor), halsband ja/nee.
2. **Foto's** volgens 1.4, met close-ups van elke aftekening.
3. **Aftekeningenkaart**: silhouet (voor, zij, achter, boven) waarop de klant vlekken intekent.
4. **Goedkeuring 1**: foto van het grijze model (houding, verhoudingen) vóór het printen.
5. **Goedkeuring 2**: foto van het geschilderde beeldje in daglicht vóór de vernis; één kleine correctie inbegrepen.
6. **Vastleggen** welke verf en mengverhouding per bestelling is gebruikt, voor nabestellingen.

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

- **Btw:** volgens je eigen notities valt Pootjespret onder een eenmanszaak die al bij KVK staat en reken je **21% btw zonder KOR**. Het model trekt 21% btw van de verkoopprijs af. Kosten staan inclusief btw (voorzichtig); met facturen op naam van de zaak zijn ze ±17% lager.
- **Productie:** FDM/PLA met 15% opslag voor misdrukken; Meshy Pro $20/mnd (aanname 1 USD ≈ € 0,87, koers okt–nov 2026 ±1,12–1,15) over **5 beeldjes per maand** (bij 20 per maand: € 0,87 per beeldje).
- **Printer werkgever:** **aangenomen vergoeding € 0,50 per printuur** – een plaatshouder, geen bron (zie 6.4).
- **Verzending:** PostNL pakket tot 3 kg naar huisadres NL € 6,35 (online, tarieven vanaf 12 juli 2026); België 0–2 kg € 12,25, dus € 6 toeslag. Prijzen zijn incl. verzending NL (Pootjespret heeft al gratis verzending vanaf € 29,95).
- **Betaalkosten:** Pootjespret rekent af via **Mollie** op **Shopify Basic** (plan opgevraagd via de Shopify-koppeling). Shopify rekent dan volgens meerdere bronnen **2% extra** bij een externe betaalprovider. Mollie iDEAL € 0,29–0,32 volgens bronnen, creditcard 1,8% + € 0,25. Model: **2% + € 0,39**.
- **Arbeid:** eigen tijd 1,25–1,75 u en schildertijd 2–4,25 u per beeldje; rekentarief **€ 15 per uur** (aanname, geen loon).

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

- **Marge excl. arbeid** = prijs − btw − directe kosten − betaalkosten: dit verdelen jullie voor jullie uren.
- **Break-even** = vaste startkosten ± € 192 (startpakket € 145, proefprints € 25, rol PLA € 22; KVK is al geregeld) gedeeld door de marge bij een mix van 25% 8 cm, 50% 12 cm, 25% 15 cm. Dan zijn de **uitgaven** terug, de uren nog niet.
- **Op geen enkel niveau** zijn de uren betaald tegen € 15. Daarvoor moet de prijs omhoog (12 cm ± € 120) of de tijd omlaag (speedpaint, vaste houdingen, kleiner formaat).
- **Etsy** kost op middenniveau € 6,67–10,87 per verkoop (6,5% + 4% + € 0,30 + $0,20), tegenover € 1,57–2,37 via Pootjespret. Met Shopify Payments in plaats van Mollie vervalt de extra 2% (± € 1,60 per beeldje van € 79); of dat voor jou kan, is niet gecontroleerd.

**Advies:** start op **middenniveau** (12 cm € 79), meet de echte uren en ga naar **hoog** zodra de kwaliteit vaststaat. Concurreer niet met onbeschilderde prints (€ 16–40).

### 5.4 Opbrengst verdelen met je vriend

Bij middenniveau (marge excl. arbeid: 8 cm € 32,41; 12 cm € 44,26; 15 cm € 55,04):

| | 8 cm | 12 cm | 15 cm |
|---|---|---|---|
| **Optie 1: vast bedrag** voor de schilder | € 20 (€ 10,00/u) | € 27 (€ 8,31/u) | € 33 (€ 7,76/u) |
| → rest voor jou | € 12,41 (€ 9,93/u) | € 17,26 (€ 11,50/u) | € 22,04 (€ 12,59/u) |
| **Optie 2: winstdeling 50/50** (ieder) | € 16,20 | € 22,13 | € 27,52 |
| **Optie 2b: winstdeling naar uren**: schilder / jij | € 19,94 / € 12,46 | € 30,28 / € 13,98 | € 38,99 / € 16,05 |

| | Vast bedrag per beeldje | Winstdeling |
|---|---|---|
| **Voordelen** | Simpel; je vriend weet vooraf wat een beeldje oplevert; jij houdt zeggenschap over prijs en kanaal; weinig administratie; het blijft jouw onderneming | Gedeeld risico en gedeelde motivatie; de schilder profiteert mee van hogere prijzen |
| **Nadelen** | Jij draagt het risico (mislukte beeldjes, weinig verkoop); de schilder profiteert niet mee van prijsverhogingen | Open boekhouding en afspraken over welke kosten meetellen; uitkomst wisselt; bij 50/50 krijgt de schilder weinig per uur; samen ondernemen met winstdeling kan een **vof** zijn, met aansprakelijkheid met privévermogen (zie 6.5) |

**Advies:** begin met **vast bedrag per beeldje**; evalueer na 10–20 beeldjes en stap eventueel over op **winstdeling naar uren**. Leg vast wie mislukte of afgekeurde beeldjes betaalt.

---

## 6. Regels en praktische punten

> Geen juridisch of fiscaal advies; laat twijfelgevallen toetsen door Belastingdienst, KVK of een adviseur.

### 6.1 Inschrijving, btw en belasting

- **KVK:** inschrijving is nodig als je zelfstandig levert, een prijs vraagt en regelmatig verkoopt aan anderen dan familie en vrienden. Je eenmanszaak met handelsnaam Pootjespret bestaat al (eigen notities); controleer of de activiteitenomschrijving ook het maken en verkopen van beeldjes dekt (kosten van een wijziging niet geverifieerd).
- **21% btw.** Het 9%-tarief voor kunst geldt alleen voor werk dat helemaal door de kunstenaar zelf is gemaakt, niet voor serieproducten. Een kennisgroep van de Belastingdienst oordeelde dat **3D-geprinte (zwangerschaps)beeldjes** onder 21% vallen omdat de persoonlijke inbreng van de maker te klein is.
- **KOR** (omzet tot € 20.000 per jaar): geen btw rekenen, maar ook niet aftrekken; minstens 4 weken vooraf aanmelden, minimaal 3 jaar, en hij geldt voor de **hele** eenmanszaak. Je gebruikt hem nu niet.
- **België:** blijven je afstandsverkopen aan particulieren in andere EU-landen onder **€ 10.000 per jaar**, dan reken je Nederlandse btw.
- **Je vriend:** zonder eigen bedrijf is de vergoeding "inkomsten uit overig werk", zelf op te geven in de aangifte (met Zvw-bijdrage; kosten mogen eraf). Met eigen bedrijf stuurt je vriend een factuur.
- **Uitbetaalde bedragen aan derden:** betalingen aan iemand zonder btw-factuur kunnen doorgegeven moeten worden; voor ondernemers zonder personeel volgens de Belastingdienst op uitnodiging (bronnen tegenstrijdig). Noteer per betaling naam, adres, geboortedatum en bedrag.

### 6.2 Herroepingsrecht en betalen

- **Geen bedenktijd bij maatwerk.** Volgens de ACM geldt de bedenktijd van 14 dagen niet voor producten die volgens de specificaties van de klant zijn gemaakt of duidelijk persoonlijk zijn. Een beeldje van het eigen dier naar eigen foto's past daarin.
- **Smalle uitzondering:** kiezen uit standaardopties (alleen formaat) is niet genoeg, en de verkoper moet kunnen aantonen dat het product aan niemand anders te verkopen is.
- **Wel melden** vóór de bestelling (vinkje in de bestelflow); anders kan de bedenktijd tot een jaar worden verlengd.
- **Herroepingsknop:** sinds 25 juni 2026 verplicht voor webwinkels (ACM). Die blijft nodig voor de gewone Pootjespret-producten; vermeld bij de beeldjes dat de uitzondering geldt.
- **Wettelijke garantie** blijft: beschadigd of anders dan afgesproken = herstel of vervanging.
- **Vooruitbetaling:** een consument kan niet verplicht worden meer dan **50%** vooruit te betalen. Laat klanten kiezen: alles vooraf of 50% aanbetaling en de rest na de goedkeuringsfoto.

### 6.3 Veiligheid en etikettering

- **GPSR** (sinds 13 december 2024, toezicht NVWA): wie onder eigen naam maakt en verkoopt, is **fabrikant**. Online moeten naam en postadres van de fabrikant, een productaanduiding en waarschuwingen zichtbaar zijn.
- **Geen speelgoed:** speelgoed is bedoeld voor spelen door kinderen onder 14. "Geen speelgoed" op het etiket is niet doorslaggevend; ontwerp en marketing tellen mee. Presenteer de beeldjes als **decoratie en herinnering voor volwassenen**.
- **Voorstel etiket** (onder het voetstuk en op de productpagina; formulering eigen advies): *Pootjespret – handgemaakt decoratief beeldje – geen speelgoed, niet geschikt voor kinderen onder 14 jaar; kleine delen kunnen afbreken – niet in contact met voedsel – afstoffen, niet nat reinigen – [postadres] – bestelnummer [xxx]*.
- Lever resinprints alleen volledig uitgehard en gewassen.

### 6.4 De printer van je werkgever

- **Nevenwerk** mag een werkgever sinds 1 augustus 2022 alleen verbieden met een objectieve reden (veiligheid, vertrouwelijke informatie, belangenverstrengeling). Meld het wel en check je contract; een concurrentiebeding blijft gelden.
- **De printer is van je werkgever.** Vraag **schriftelijk** toestemming en leg vast: wanneer (buiten werktijd, werkprints gaan voor); vergoeding en wie filament of hars betaalt (met factuur is de btw aftrekbaar); wie betaalt bij slijtage of schade; veiligheid en afvoer bij resin; geen gebruik van bedrijfsinformatie; opzegtermijn.
- **Plan B:** eigen printer of printdienst (prijzen niet onderzocht).

### 6.5 Afspraken met je vriend op papier

- **Vast bedrag** = je vriend is opdrachtnemer; het blijft jouw onderneming. **Winstdeling en samen ondernemen** = al snel een **vof**: elke vennoot is met privévermogen aansprakelijk voor álle schulden. KVK raadt dan een samenwerkingscontract aan.
- **Op één A4:** taken, vergoeding per formaat en betaaltermijn, levertijd, kwaliteit en afkeur/herstel, wie het startpakket betaalt en bezit, omgang met klantfoto's en -gegevens, gebruik van foto's van het werk, naamsvermelding, stoppen.
- **Jonger dan 18?** Dan is toestemming van een ouder of voogd nodig; een contract zonder toestemming kan worden teruggedraaid (handlichting kan vanaf 16 jaar).

### 6.6 Foto's van klanten en privacy

- De maker van een foto heeft het **auteursrecht**: laat de klant bevestigen dat de foto's van henzelf zijn (of dat ze ze mogen gebruiken) en dat jij ze mag gebruiken voor het beeldje.
- Voor foto's op website of social media: **aparte toestemming**. Herkenbare mensen op foto's zijn persoonsgegevens; vraag foto's van alleen het dier.
- Meld in je privacyverklaring dat een externe 3D-tool de foto's verwerkt, en gebruik een **betaald** Meshy-plan (gratis modellen vallen onder CC BY 4.0).

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

Met een **introductieprijs van € 49 (8 cm) / € 65 (12 cm)** is de omzet van 5 beeldjes ± € 245–325 incl. btw, ofwel ± € 200–270 excl. btw. Reken op **ongeveer quitte tot ± € 80 tekort**; je houdt het schilderpakket (± € 78) en ruim een halve rol PLA over, en je eigen uren zijn nog onbetaald. Vanaf beeldje 6 vallen de eenmalige kosten weg. Noem de prijs eerlijk een **introductieprijs voor de eerste 5 bestellingen** in ruil voor feedback en (met toestemming) foto's, zonder nep-"van"-prijs: de ACM let op misleidende kortingen.

### 8.2 Planning november

| Week | Wat |
|---|---|
| **Wk 45 (5–8 nov)** | Schriftelijke toestemming werkgever en printertype vaststellen; afspraak met je vriend op papier; pakket en PLA bestellen; proefmodel maken en printen |
| **Wk 46 (9–15 nov)** | Productpagina live ("eerste 5 plekken"); 5 klanten werven; foto's en formulieren binnen; Meshy Pro afsluiten; modellen ter goedkeuring sturen |
| **Wk 47 (16–22 nov)** | Printen en nabewerken; je vriend schildert en houdt de tijd bij |
| **Wk 48 (23–29 nov)** | Goedkeuringsfoto's, correcties, vernissen, verzenden of afgeven |
| **30 nov** | Evaluatie: echte uren en kosten in `kostprijs.csv`, feedback ophalen, prijs en levertijd voor december vaststellen |

### 8.3 Beslisregels na de test

- **Doorgaan** als klanten hun dier herkennen, een 12 cm-beeldje samen minder dan ±5 uur kost en minstens de helft van de klanten het voor de normale prijs zou kopen of aanraden.
- **Prijs omhoog** naar midden of hoog zodra de kwaliteit goed is; het lage niveau dekt jullie uren niet.
- **Proces aanpassen** als AI-modellen vaak mislukken: vaste houdingen, meer foto's vragen of een freelancer voor lastige dieren.
- **Stoppen of anders inrichten** als de printer niet beschikbaar blijft of het schilderen veel langer duurt dan geschat.

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

