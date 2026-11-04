# Handbeschilderde 3D-geprinte huisdierbeeldjes – verkenning

Opgesteld: nacht van 4 op 5 november 2026. Alle bronnen geraadpleegd op 4–5 november 2026.

> **Werkwijze en beperking.** WebFetch werkte in deze omgeving niet (elke site gaf een DNS-fout). Alle feiten komen daarom uit zoekresultaten van WebSearch, die steeds een korte samenvatting van de gevonden pagina's geven. De pagina's zijn dus niet volledig gelezen. Waar bronnen elkaar tegenspreken of geen bron is gevonden, staat dat erbij ("niet geverifieerd"). Bedragen zonder bron zijn eigen schattingen en staan ook zo vermeld.

## Inhoud

1. [Van foto naar 3D-model](#1-van-foto-naar-3d-model)
2. [Printen om te beschilderen](#2-printen-om-te-beschilderen)
3. [Beschilderen](#3-beschilderen)
4. [Markt en concurrenten](#4-markt-en-concurrenten)
5. [Kostprijs, verkoopprijs en verdeling](#5-kostprijs-verkoopprijs-en-verdeling)
6. [Regels en praktische punten](#6-regels-en-praktische-punten)
7. [Productpagina](#7-productpagina)
8. [Advies: 5 testbeeldjes deze maand](#8-advies-5-testbeeldjes-deze-maand)

---

## 1. Van foto naar 3D-model

### 1.1 Drie routes

| Route | Hoe het werkt | Geschikt voor huisdieren? | Kosten per model | Commercieel gebruik |
|---|---|---|---|---|
| **AI image-to-3D** (Meshy, Tripo, Rodin) | Klantfoto('s) uploaden, model in enkele minuten | Ja, mits goede foto's; nabewerking bijna altijd nodig | Meshy Pro: $20/mnd voor 1.000 credits; één model met textuur ±30–35 credits → ±$0,60–0,70 per poging | Meshy: betaald = eigen bezit; gratis = CC BY 4.0 met naamsvermelding. Tripo/Rodin: zie hieronder |
| **Fotogrammetrie** (Polycam, KIRI Engine) | 30–100+ foto's rondom een stilstaand onderwerp, software rekent model uit | Slecht: dier moet stil blijven; vacht geeft weinig houvast | KIRI basis gratis; Polycam Pro $26,99/mnd (App Store, april 2026) | Niet geverifieerd |
| **Freelance 3D-modelleur** (Fiverr, Etsy) | Kunstenaar boetseert digitaal op basis van foto's | Beste controle over pose en karakter | Fiverr-sculpts vanaf ±$30–57; kant-en-klare pet-STL op Etsy ±$10–47 | Per opdracht afspreken (rechten op het bestand) |

### 1.2 AI image-to-3D: wat werkt en wat niet

- **Kwaliteit.** Een praktijktest van 3DWithUs liet zien dat Meshy van één hondenfoto een herkenbaar beeldje kon maken; de houding en details bleven goed zichtbaar na het printen. Bij Tripo werd een extra "Refine"-stap gebruikt die vooral vacht en staart aanpaste. Onafhankelijke tests zijn schaars; Meshy's eigen claims over printbaarheid zijn niet onafhankelijk gecontroleerd.
- **Typische problemen.** Gaten en niet-gesloten mesh, omgekeerde normalen, te dunne poten en een zeer zware mesh. Oplossingen: automatisch repareren (Microsoft 3D Builder, Meshmixer of de repairfunctie van de slicer), dunne delen 0,5–1 mm dikker maken en de mesh vereenvoudigen in Blender (Decimate). Een vast **voetstuk** onder de poten lost het probleem van dunne poten grotendeels op (eigen advies).
- **Meerdere foto's.** Meshy ondersteunt "Multi-View": één hoofdfoto plus maximaal 3 extra hoeken, alleen voor betaalde abonnementen. Volgens Meshy's helpcentrum moeten de hoeken echt verschillen (minstens 45–90° uit elkaar), het liefst voor, zijkant (90°) en achter, met de achtergrond verwijderd. Bronnen spreken elkaar tegen over welk Meshy-model Multi-View ondersteunt.
- **Kosten Meshy.** Pro kost $20 per maand voor 1.000 credits (verlopen maandelijks). Image-to-3D kost volgens de documentatie 20–25 credits plus 10 voor textuur; de API-pagina noemt 20 zonder en 30 met textuur. Voor ongekleurde prints is textuur niet nodig, maar wel handig als kleurvoorbeeld voor de schilder.
- **Tripo.** Professional geeft 3.000 credits per maand (tot 200 modellen) volgens Tripo's helppagina. De maandprijs is **niet geverifieerd**: bronnen noemen $11,94 tot $19,90. Gratis modellen zijn volgens de meeste Tripo-pagina's niet voor commercieel gebruik; één Tripo-blog noemt CC BY 4.0. Tegenstrijdig, dus voor verkoop een betaald plan nemen.
- **Rodin (Hyper3D).** De prijspagina noemt een commerciële licentie expliciet alleen bij het Business-plan; andere sites zeggen dat alle uitvoer commercieel vrij is. **Niet geverifieerd** → niet gebruiken zonder de licentietekst te lezen.
- **Bambu Lab MakerLab** (Meshy-motor binnen MakerWorld): export kost 2 MakerLab-credits, die je verdient en niet koopt. Of je de uitvoer mag verkopen, is **niet duidelijk**; alleen een gebruikersmening op het forum. Geschikt om te testen, niet voor verkoop.
- **Open-source.** Tencent Hunyuan3D 2.0/2.1: de licentie geldt uitdrukkelijk **niet in de EU**, het VK en Zuid-Korea → niet gebruiken. Microsoft TRELLIS staat onder MIT-licentie (commercieel toegestaan), maar de nieuwste versie vraagt een NVIDIA-kaart met 24 GB geheugen; alleen interessant als je die hardware hebt.

### 1.3 Fotogrammetrie

Fotogrammetrie heeft tientallen scherpe foto's van een **stilstaand** onderwerp nodig; zelfs ademhalen kan de reconstructie verstoren. Een maker die een cavia scande, gebruikte ±60 losse foto's in plaats van een live-scan; een ander scande een liggende hond. Onderzoek naar hondenbeweging noemt vacht lastig omdat delen weinig textuur tonen. **Conclusie:** onbruikbaar voor klanten die op afstand foto's sturen; hooguit voor een slapend dier bij jou thuis.

### 1.4 Freelance modelleurs

Op Fiverr bieden veel verkopers "huisdier naar STL" aan. Zoekresultaten tonen vanafprijzen van ±$30 tot $57 voor figuur-sculpts en een categorieprijs van $100–120 voor printklare personages; specifieke huisdier-gigs toonden geen prijs. Op Etsy kosten digitale pet-STL's ±$10–47. Specialistische studio's rekenen veel meer (een portretfiguur "vanaf $429", inclusief print). Let op: leg vast dat je het bestand commercieel mag printen en verkopen, hoeveel revisies inbegrepen zijn en de levertijd.

### 1.5 Wat moet de klant aanleveren?

Afgeleid van Meshy's richtlijnen voor Multi-View plus wat de schilder nodig heeft:

1. **Voorkant** op ooghoogte van het dier, hele dier in beeld.
2. **Zijkant links en rechts** (90°), staand of in de gewenste houding.
3. **Achterkant** of schuin achter (rug en staart).
4. **Close-up van de kop** (ogen, neus, oren).
5. **Aftekeningen**: vlekken, bles, sokjes, afwijkende kleuren (voor de schilder).
6. Eisen: daglicht, geen flits, scherp, rustige achtergrond, geen filters, origineel bestand (geen schermafdruk). Minimaal 3, liefst 5–8 foto's.

### 1.6 Advies deel 1

Start met **Meshy Pro (1 maand, $20)** en een vaste werkwijze: foto's → model → repareren en voetstuk toevoegen → printen. Reken 2–4 generaties per dier en 30–60 minuten eigen nabewerking (eigen schatting). Houd een freelancer achter de hand voor dieren waar AI faalt (lastige houding, langharige rassen).

**Bronnen deel 1**
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

---

## 2. Printen om te beschilderen

### 2.1 FDM of resin?

Je weet nog niet welk type printer je werkgever heeft. Beide zijn bruikbaar; resin geeft meer detail, FDM is eenvoudiger en veiliger.

| | FDM (filament, bijv. PLA) | Resin (MSLA, vloeibare hars) |
|---|---|---|
| Laagdikte | 0,08–0,2 mm; 0,08–0,12 mm is een gangbaar compromis voor figuren | 0,01–0,05 mm |
| Detail | Kenmerken kleiner dan ±0,5 mm (spuitmond 0,4 mm) vervagen; laaglijnen zichtbaar | Fijne vacht, ogen en neus blijven scherp |
| Nabewerking | Steunen weghalen, schuren, filler primer om laaglijnen te vullen (meer werk) | Afspoelen in IPA, naharden onder UV, steunen weghalen, licht schuren |
| Gezondheid | Ventileren; hogere temperatuur geeft meer fijnstof (BfR) | Vloeibare hars kan huidallergie geven; ventileren, nitrilhandschoenen, bril; IPA is brandbaar |
| Sterkte | Taai, breekt niet snel | Standaardhars is broos; dunne delen breken sneller bij verzending |
| Printtijd | Hangt af van volume | Hangt alleen af van hoogte; meerdere beeldjes tegelijk kost bijna geen extra tijd |

**Advies:** voor de eerste testbeeldjes werkt FDM met 0,08–0,12 mm laagdikte en een stevig voetstuk prima, mits je vriend een filler primer gebruikt. Heeft je werk een resinprinter met een goed geventileerde ruimte, dan levert dat mooiere details en minder schuurwerk op.

### 2.2 Gezondheid en ventilatie bij resin

- Het **RIVM** (2016, in opdracht van de NVWA) concludeert dat 3D-printen in een consumentenomgeving risico's geeft, dat de ernst niet goed vast te stellen is en dat goede ventilatie belangrijk is. Het rapport is niet specifiek over hars.
- **EU-OSHA** heeft een praktijkvoorbeeld gepubliceerd over het vervangen van gevaarlijke hars bij 3D-printen; resin wordt daarin als gevaarlijke stof op de werkplek behandeld.
- Leveranciers en veiligheidsgidsen zijn het eens over de basis: niet-uitgeharde hars en kleverige verse prints alleen aanraken met **nitrilhandschoenen** (geen latex; AmeraLabs noemt minimaal 0,15 mm), **oogbescherming**, en **ventilatie** als belangrijkste maatregel. Vuistregel: ruik je de hars, dan is de ventilatie onvoldoende. "Waterwasbare" hars is niet minder giftig.
- Lees altijd het **veiligheidsinformatieblad (SDS)** van de gebruikte hars. Vang IPA-afval en harsresten op; laat restanten uitharden in de zon voor je ze weggooit (eigen advies; check de gemeentelijke regels voor chemisch afval).
- Op het werk: de arboregels van je werkgever gelden. Overleg wie verantwoordelijk is voor PBM en afvoer (zie deel 6).

### 2.3 Formaten, printtijd en materiaal

**Aannames (eigen schatting):** een zittende hond of kat met voetstuk; het volume schaalt met de derde macht van de hoogte (8 cm ≈ 0,3×, 15 cm ≈ 2× het volume van 12 cm). De ruwe rekensom voor 12 cm (kop ±4 cm, lijf ±5×7×8 cm, voetstuk) geeft ±200 cm³ massief volume. Resin: hol met 2 mm wand vanaf 12 cm. Printtijd resin: 2.400 lagen van 0,05 mm × 6–10 s per laag (belichting ±2,7 s plus het op- en neerbewegen van het platform).

| Formaat | FDM: filament | FDM: printtijd | Resin: hars (incl. steunen) | Resin: printtijd |
|---|---|---|---|---|
| 8 cm | 20–40 g | 1,5–3 uur | 25–35 g (massief) | 2,5–4,5 uur |
| 12 cm | 60–120 g | 4–8 uur | 50–70 g (hol) | 4–7 uur |
| 15 cm | 120–230 g | 7–14 uur (0,12 mm) | 80–100 g (hol) | 5–8,5 uur |

Ter vergelijking: op MakerWorld staan figuren van ±12 cm met een opgegeven printtijd van 2,2 uur (16 g, slank model) tot ±5 uur (126 g inclusief steunen). Het werkelijke verbruik lees je af in de slicer zodra je een echt model hebt; vervang dan deze schattingen in `kostprijs.csv`.

**Materiaalprijzen (incl. btw):**
- PLA grijs 1,75 mm, 1 kg: € 22,25 per kg (2-pack 123-3D, € 44,50) tot € 26,50 (123-3D marmergrijs). → **± € 0,02–0,03 per gram**.
- Elegoo Standard Resin grijs, 1 kg: € 47,50 bij 123-3D.nl (tijdelijk uitverkocht bij raadplegen) en € 22,80 bij Kubii (Frankrijk). → **± € 0,025–0,05 per gram**, plus IPA, handschoenen en papier (eigen schatting ± € 0,50–1,00 per print; prijzen niet geverifieerd).

**Materiaalkosten per beeldje (eigen berekening):**

| Formaat | FDM (PLA) | Resin (hars + verbruik) |
|---|---|---|
| 8 cm | € 0,50–1,10 | € 1,10–2,70 |
| 12 cm | € 1,30–3,20 | € 1,80–4,40 |
| 15 cm | € 2,70–6,10 | € 2,50–5,80 |

Een grijze of witte kleur is het handigst onder verf. Hol printen loont bij kleine beeldjes nauwelijks; vanaf ±12 cm wel. Zorg dan voor minstens twee afvoergaten in het voetstuk, anders blijft er hars achter en kan de print later scheuren.

### 2.4 Nabewerking stap voor stap

1. **Steunen verwijderen.** FDM: met een zijkniptang; "tree supports" laten minder sporen na. Resin: eerst wassen, steunen verwijderen terwijl de print nog iets zacht is, daarna naharden onder UV.
2. **Schuren.** Hoge punten en steunresten wegschuren (korrel 120–220 bij FDM, fijner bij resin). Primer verbergt geen hoge punten; die worden juist beter zichtbaar.
3. **Filler primer.** Een vullende primer zoals Mr. Surfacer 500 (grof) of 1000 (fijn) vult laaglijnen; daarna licht nat schuren (320–600 of fijner) en zo nodig herhalen. Ruw PLA schuurt slecht; eerst een laag filler primer en dan schuren werkt beter.
4. **Eindprimer** in grijs, wit of zwart als ondergrond voor de verf (zie deel 3).

Reken voor nabewerking ±20–40 minuten per beeldje bij FDM en ±15–25 minuten bij resin (eigen schatting, exclusief droogtijd).

**Bronnen deel 2**
- FDM vs resin: https://jlc3dp.com/blog/resin-vs-fdm-for-miniatures ; https://blog.lootstudios.com/print/the-ultimate-fdm-versus-resin-guide/ ; https://www.3dsourced.com/guides/resin-vs-fdm-for-3d-printing-miniatures/
- RIVM: https://www.rivm.nl/publicaties/risicos-van-3d-printen-in-consumentenomgeving-technieken-materialen-en-producten ; EU-OSHA: https://osha.europa.eu/nl/publications/replacing-hazardous-resin-3d-printing-make-moulds ; BfR: https://www.bfr.bund.de/cm/349/3d-printing-a-dusty-business.pdf
- Resin-veiligheid: https://ameralabs.com/?p=30319 ; https://jlc3dp.com/blog/resin-hazards ; VOC-studie: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12848961/
- Printtijd resin: https://www.fabbaloo.com/news/prusa-reveals-how-they-sped-up-msla-3d-printing ; https://cults3d.com/:4019929 ; FDM-voorbeelden: https://makerworld.com/models/2911139 ; https://makerworld.com/models/1308641
- Hol printen: https://blog.lootstudios.com/print/hollow-vs-solid-3d-models/ ; https://3dprinterly.com/how-to-hollow-resin-3d-prints-properly/
- Prijzen: https://www.123-3d.nl/123-3D-Filament-PLA-Grijs-1-75-mm-2-pack-1-kg-i12218.html ; https://www.123inkt.nl/123-3D-Filament-PLA-Marmer-Grijs-1-75-mm-1-kg-i110111.html ; https://www.123-3d.nl/Elegoo-Standaard-resin-Grijs-1-kg-14-0007-61B-i8552.html ; https://www.kubii.com/en/consumable-materials/4594-standard-colored-resin-1-kg-for-3d-printer-3272496322394.html
- Filler primer: https://forums.kitmaker.net/t/filling-3d-ripples/33574 ; https://plastmodel.pl/en/products/7173-mr-surfacer-1000-sf-284 ; https://evezone.evetech.co.za/build-lab/how-to-finish-3d-printed-props-sand-fill-prime-and-paint

---

## 3. Beschilderen

### 3.1 Methodes

| Methode | Voordelen | Nadelen | Advies |
|---|---|---|---|
| **Penseel** | Goedkoop, weinig voorbereiding, ideaal voor ogen, neus en aftekeningen | Grote vlakken en zachte overgangen kosten meer tijd | Hiermee beginnen |
| **Airbrush** | Snelle, egale grondlagen en zachte overgangen (bijv. vachtverloop) | Compressor en schoonmaakspullen zijn een investering; oefenen met verdunnen, druk en nevel; maakt je niet vanzelf sneller | Pas na 5–10 beeldjes, als het volume groeit |
| **Combinatie** | Airbrush voor basis, penseel voor detail; veel schilders werken zo | — | Doelvorm op termijn |

Praktische technieken voor vacht (eigen advies, gangbaar in de miniatuurhobby): een **"speedpaint"/contrastverf** die zelf in de diepere delen van de vacht loopt, daarna **droogborstelen** (drybrushing) met een lichtere tint om de vachtstructuur op te laten lichten, en tot slot detail met een fijn penseel. De zoekresultaten bevestigden deze vacht-technieken niet specifiek; laat je vriend ze testen op een proefprint.

### 3.2 Opbouw van de lagen

1. **Filler primer** (alleen FDM, zie 2.4) → schuren.
2. **Primer** in grijs (neutraal), wit (lichte dieren) of zwart (donkere dieren).
3. **Basiskleuren** in acrylverf (watergedragen, makkelijk schoon te maken).
4. **Schaduw en licht**: speedpaint/wash en droogborstelen.
5. **Details**: ogen, neus, nagels, halsband; een glanzend puntje op de ogen maakt het beeldje levendig.
6. **Matte vernis** ter bescherming; eventueel glansvernis alleen op ogen en neus.

### 3.3 Startpakket voor je vriend

Volledige lijst met winkels, URL's en status in [`startpakket.csv`](startpakket.csv) (puntkomma-gescheiden, decimale komma). Samengevat, prijzen incl. btw zoals gevonden op 4 november 2026:

| Pakket | Inhoud | Totaal |
|---|---|---|
| **Basis** | Warpaints Starter Set (€ 34,00), penselen (€ 15,99), wet palette (€ 21,95), Vallejo primer (€ 12,99), Motip primer-spuitbus (€ 4,99), Motip filler (€ 13,37), matte vernis (€ 9,49), Hobby Tool Kit (€ 31,93) | **± € 145** |
| **+ Speedpaint** | Speedpaint Starter Set 2.0 (€ 39,99) | ± € 185 |
| **+ Airbrush** | Revell Airbrush Basic Set met compressor (€ 99,95) | ± € 285 |

Kanttekeningen: schuurpapier, handschoenen en stofmasker hebben geen geverifieerde prijs. De vernisprijs komt van een Letse webshop omdat er geen Nederlandse prijs werd gevonden. De wet palette was uitverkocht; een zelfgemaakte versie (bakje, keukenpapier, bakpapier) werkt ook. Besparen: sla de wet palette en de tool kit over (alleen een zijkniptang en hobbymes), dan kom je op ± € 90–100 (eigen schatting).

### 3.4 Schildertijd per beeldje

Er is geen bron voor huisdierbeeldjes specifiek. Ijkpunten uit hobbyfora: een figuur op 28 mm-schaal kost 1,5–3 uur, een gangbare opdracht 4–6 uur, en een 75 mm-figuur grofweg 5–10 uur (schatting op basis van die fora). Een huisdier is één onderwerp zonder kleding of wapens, maar de vacht en aftekeningen vragen precisie.

**Eigen schatting (exclusief droogtijd, voor iemand met wat ervaring):**

| Formaat | Schildertijd | Eerste 5 beeldjes |
|---|---|---|
| 8 cm | 1,5–2,5 uur | reken ±2× zo lang |
| 12 cm | 2,5–4 uur | reken ±2× zo lang |
| 15 cm | 3,5–5 uur | reken ±2× zo lang |

Laat je vriend bij de testbeeldjes de tijd bijhouden en pas `kostprijs.csv` daarop aan.

### 3.5 Kleuren en aftekeningen vastleggen met de klant

Bijna alle aanbieders van huisdierportretten en -beeldjes sturen de klant een **foto ter goedkeuring** vóór verzending, vaak met één gratis correctieronde. Een vaste kleurprocedure vond ik in de bronnen niet; dit is een voorstel:

1. **Intakeformulier** bij de bestelling: naam en ras van het dier, vachtkleur(en), kleur van ogen en neus, bijzondere kenmerken (bles, sokjes, vlekken, scheur in oor), wel/geen halsband (kleur, eventueel naamplaatje).
2. **Foto's** volgens 1.5, waarvan minstens één in daglicht zonder filter, plus close-ups van elke aftekening.
3. **Aftekeningenkaart**: een eenvoudig silhouet (voor, zij, achter, boven) waarop de klant de vlekken intekent of omcirkelt. Kan als PDF of als foto van een print.
4. **Goedkeuring 1 – model**: stuur een render of foto van het grijze 3D-model (houding en verhoudingen). Pas na akkoord printen.
5. **Goedkeuring 2 – verf**: foto van het beschilderde beeldje in daglicht vóór de vernislaag. Eén kleine correctieronde inbegrepen; grotere wijzigingen tegen meerprijs.
6. **Vastleggen**: noteer per bestelling de gebruikte verfkleuren en mengverhoudingen, zodat een nabestelling er hetzelfde uitziet.
7. **Verwachting managen** op de productpagina: handwerk, dus kleine verschillen met de foto zijn mogelijk.

**Bronnen deel 3**
- Penseel vs airbrush: https://tistaminis.com/blogs/blog/airbrush-vs-brush-when-each-wins-for-miniatures-painting ; https://www.scalemodelshop.co.uk/paint-brushes-vs-airbrush-scale-models/ ; https://www.wargamer.com/the-best-airbrush-for-miniatures
- Schildertijd: https://cypaint.com/article/how-to-prices-a-commission-miniature-painting ; https://www.coolminiornot.com/forums/threads/how-long-do-you-spend-on-a-figure.10345/
- Goedkeuringsfoto's: https://www.riverry.com/products/mini-custom-watercolor-pet-portrait-cat-46341 ; https://madeit.com.au/products/handmade-custom-pet-plush-from-photo-pet-keepsake-ornament-memorial-gift-stellar-craft ; https://etsy.com/shop/SiennaPetPortraits
- Prijzen startpakket: zie URL's in `startpakket.csv` (o.a. https://de-dondersteen.nl/products/the-army-painter-warpaints-starter-paint-set ; https://www.123-3d.nl/Vallejo-Surface-Primer-Grey-200-ml-74601-i9597.html ; https://www.toemen.nl/en/product/revell-airbrush-basic-set-with-compressor-version-2023)

---

## 4. Markt en concurrenten

Volledige lijst (15 aanbieders) in [`concurrenten.csv`](concurrenten.csv). Prijzen zijn momentopnames uit zoekresultaten van 4 november 2026; levertijden en reviews ontbraken bij veel kleine webshops.

### 4.1 Prijsladder

| Segment | Voorbeelden | Prijs (±10–12 cm) |
|---|---|---|
| **Onbeschilderd, één kleur** | Solid Memories (NL), 3D Huisdier (NL), Verrassingsdoos (NL) | € 25–60 (Solid Memories: 8 cm € 15,99 / 12 cm € 29,99 / 16 cm € 39,00) |
| **Handbeschilderde 3D-print** | Atelier Robijns (BE), Etsy-verkopers, Minipiece (NL) | € 45–55; Etsy ± $25–65 |
| **Handgeboetseerd** | Klischklick (DE) | € 126 (5–10 cm, incl. verzending) |
| **Meerkleurige FDM-print** | 3d-druck-scan.com (DE), Figuroo (DE) | € 80–200; Figuroo € 25–120 |
| **Full-colour print (vergelijking)** | Youlittle (DE), machmich3d (DE), DoubleMe3d (NL), My3DSelfie, Cuddle Clones (VS) | € 149–420; Cuddle Clones ± $99–129 (4 inch) |

### 4.2 Observaties

- **De directe concurrent zit laag in prijs.** Atelier Robijns (BE) verkoopt een handbeschilderd 3D-geprint beeldje van ±10 cm voor € 44,95 met 15–20 werkdagen productietijd. Etsy-verkopers zitten in dezelfde orde. Onbeschilderde prints beginnen al bij € 16.
- **Full-colour printen is geen goedkope route.** Full-colour diensten (vaak op basis van een scan, gips/zandsteen) kosten € 149–420 voor 5–10 cm. Handbeschildering is dus een realistisch alternatief, maar de klant betaalt bij concurrenten niet veel extra voor "met de hand".
- **Levertijden** die wel gevonden zijn: 15–20 werkdagen (Atelier Robijns), 3–5 weken (My3DSelfie). Een levertijd van 2–3 weken is dus concurrerend.
- **Formaten 8, 12 en 15/16 cm** komen terug bij Solid Memories; ±10 cm is het meest voorkomende enkele formaat.

### 4.3 Wat klanten waarderen en missen (reviews)

Er zijn weinig onafhankelijke reviews over deze kleine aanbieders. Wat terugkomt in de gevonden reviews:

**Gewaardeerd**
- **Gelijkenis**: "het is echt mijn hond/kat" is het belangrijkste compliment (Herdenkingsbeeldje.nl, My3DSelfie, Etsy).
- **Meedenken en aanpassen**: klanten waarderen dat ze een prototype of foto kregen en wijzigingen konden doorgeven (My3DSelfie, PetPalsDIY).
- **Goedkeuring vóór verzending**: veel verkopers sturen eerst een foto; klanten zien dat als zekerheid.

**Gemist of klachten**
- **Prijs/waarde**: full-colour beeldjes worden als duur en soms tegenvallend ervaren (My3DSelfie, Trustpilot UK).
- **Standaardmodel in plaats van het eigen dier**: een Trustpilot-review van PetPalsDIY klaagt over "generieke koppen met een beetje verf".
- **Verwachting niet waargemaakt**: bij Petsies kreeg een koper een geprinte foto in plaats van het verwachte handwerk.
- **Levertijd langer dan beloofd**: komt voor bij verwante herdenkingswebshops (bijv. Herinnerdingendoos.nl).

**Les voor jou:** beloof alleen wat je waarmaakt (echt handwerk, echte levertijd), laat foto's van eigen werk zien en bouw twee goedkeuringsmomenten in (zie 3.5).

**Bronnen deel 4**
- NL/BE: https://solidmemories.nl/ ; https://3dhuisdier.nl/ ; https://www.minipiece.nl/producten/huisdieren-1 ; https://verrassingsdoos.com/shop/3d-beeldje-van-foto ; https://doubleme3d.nl/3d-dieren/ ; https://duplify.nl/3d-sculptuur-huisdier/ ; https://www.atelierrobijns.be/product/3d-print-van-je-huisdier/ ; https://dk.trustpilot.com/review/herdenkingsbeeldje.nl
- DE: https://figuroo.de/product/3d-avatar-hund-katze/ ; https://3d-druck-scan.com/produkt/3d-miniatur-figur-ihr-haustier-hund-katze-mehrfarbig/ ; https://youlittle.com/3d-figuren/preise/ ; https://machmich3d.de/produkt/3d-figur-haustiere/ ; https://www.klischklick.de/figuren/
- Internationaal: https://my3dselfie.com/nl-nl/products/urn-figurine-back ; https://uk.trustpilot.com/review/my3dselfie.com ; https://no.trustpilot.com/review/my3dselfie.com ; https://www.dogster.com/lifestyle/cuddle-clones-review/ ; https://www.etsy.com/market/custom_pet_figurine_from_photo ; https://www.etsy.com/market/hand_painted_dog_figurine
- Klachten: https://ca.trustpilot.com/review/petpalsdiy.com ; https://articles.hepper.com/petsies-custom-pet-plushies-review/ ; https://nl-be.trustpilot.com/review/herinnerdingendoos.nl

---


## 5. Kostprijs, verkoopprijs en verdeling

Het volledige rekenmodel staat in [`kostprijs.csv`](kostprijs.csv) (puntkomma-gescheiden, decimale komma). Pas de aannames aan zodra je echte slicer- en schildertijden hebt.

### 5.1 Uitgangspunten

- **Je bestaande eenmanszaak.** Volgens je eigen notities valt Pootjespret onder een eenmanszaak die al bij KVK staat ingeschreven, en reken je **21% btw zonder kleineondernemersregeling (KOR)**. Het model trekt daarom 21% btw van de verkoopprijs af. Kosten staan inclusief btw (voorzichtig gerekend); met facturen op naam van de zaak kun je die btw terugvragen, waardoor de kosten ±17% lager uitvallen.
- **Printen:** FDM met PLA, 15% opslag voor mislukte prints (resin is per beeldje vergelijkbaar of iets duurder, zie 2.3).
- **3D-model:** Meshy Pro $20/mnd (aanname 1 USD ≈ € 0,87; de koers lag in oktober–november 2026 rond 1,12–1,15 dollar per euro), verdeeld over **5 beeldjes per maand**. Bij 20 per maand daalt dit van € 3,48 naar € 0,87.
- **Printer van je werkgever:** in het model staat een **aangenomen vergoeding van € 0,50 per printuur**. Dat is geen bedrag uit een bron, maar een plaatshouder voor de afspraak met je werkgever (zie 6.4).
- **Verzending:** PostNL klein pakket tot 3 kg naar een huisadres in NL € 6,35 (online frankering, tarieven vanaf 12 juli 2026). België: pakket 0–2 kg naar huisadres € 12,25; reken daar € 6 toeslag. Pootjespret geeft al gratis verzending vanaf € 29,95, dus de prijzen zijn inclusief verzending NL.
- **Betaalkosten:** Pootjespret rekent af via **Mollie**, niet via Shopify Payments, op een **Shopify Basic**-abonnement (opgevraagd via de Shopify-koppeling). Shopify rekent dan volgens meerdere bronnen **2% extra** per bestelling bij een externe betaalprovider. Mollie iDEAL: bronnen noemen € 0,29–0,32; het model rekent voorzichtig met € 0,39 (inclusief btw). Creditcard bij Mollie: 1,8% + € 0,25. Het model rekent met **2% + € 0,39**.
- **Arbeid:** eigen tijd 1,25–1,75 uur en schildertijd 2–4,25 uur per beeldje (eigen schattingen). Voor de kostprijs is een rekentarief van **€ 15 per uur** gebruikt; dat is een aanname, geen loon.

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

De **arbeid is 75–80% van de kostprijs**. Materiaal is bijna verwaarloosbaar; tijd is de echte kostenpost.

### 5.3 Drie prijsniveaus (incl. 21% btw en verzending NL)

| Niveau | 8 cm | 12 cm | 15 cm | Marge excl. arbeid (12 cm) | Opbrengst per arbeidsuur | Break-even (mix) |
|---|---|---|---|---|---|---|
| **Laag** (gelijk aan Atelier Robijns/Etsy) | € 49 | € 65 | € 79 | € 32,97 | ± € 6,50–7,50 | 6 stuks |
| **Midden** | € 59 | € 79 | € 99 | € 44,26 | ± € 9–10 | 5 stuks |
| **Hoog** (premium: naamplaatje, 2 correctierondes, cadeauverpakking) | € 75 | € 99 | € 125 | € 60,38 | ± € 12,50–14 | 4 stuks |

- **Marge excl. arbeid** = prijs − 21% btw − directe kosten − betaalkosten. Dit bedrag verdelen jullie samen voor jullie uren.
- **Break-even** = vaste startkosten (± € 192: startpakket € 145, proefprints € 25, rol PLA € 22; KVK-inschrijving is niet nodig) gedeeld door de marge, bij een mix van 25% 8 cm, 50% 12 cm en 25% 15 cm. Dan zijn je **uitgaven** terug; de uren zijn dan nog niet betaald.
- **Op geen enkel niveau** wordt de arbeid volledig gedekt tegen € 15 per uur. Wil je dat, dan moet de prijs omhoog (12 cm ± € 120) of de tijd omlaag (sneller schilderen met speedpaint, kleiner formaat, vaste houdingen).
- **Via Etsy** gaan er op middenniveau € 6,67–10,87 per verkoop naar platform- en betaalkosten (6,5% transactie + 4% + € 0,30 betaling + $0,20 listing), tegenover € 1,57–2,37 via Pootjespret. Etsy is wel een extra vindplaats.
- **Tip:** met Shopify Payments in plaats van Mollie vervalt de extra 2% van Shopify (± € 1,60 per beeldje van € 79). Of dat voor jou kan, heb ik niet gecontroleerd.

**Advies:** start op **middenniveau** (12 cm voor € 79) voor de testbeeldjes, meet de echte uren en schuif op naar **hoog** zodra de kwaliteit vaststaat. Concurreer niet op prijs met onbeschilderde prints (€ 16–40).

### 5.4 Opbrengst verdelen met je vriend

Rekenvoorbeeld bij middenniveau (marge excl. arbeid: 8 cm € 32,41; 12 cm € 44,26; 15 cm € 55,04):

| | 8 cm | 12 cm | 15 cm |
|---|---|---|---|
| **Optie 1: vast bedrag** voor de schilder | € 20 | € 27 | € 33 |
| → schilder per uur | € 10,00 | € 8,31 | € 7,76 |
| → rest voor jou (per uur) | € 12,41 (€ 9,93) | € 17,26 (€ 11,50) | € 22,04 (€ 12,59) |
| **Optie 2: winstdeling 50/50** (ieder) | € 16,20 | € 22,13 | € 27,52 |
| → schilder per uur | € 8,10 | € 6,81 | € 6,48 |
| **Optie 2b: winstdeling naar uren** – schilder | € 19,94 | € 30,28 | € 38,99 |
| → jij | € 12,46 | € 13,98 | € 16,05 |

| | Vast bedrag per beeldje | Winstdeling |
|---|---|---|
| **Voordelen** | Simpel; je vriend weet vooraf precies wat een beeldje oplevert; jij houdt zeggenschap over prijs en kanaal; weinig administratie; geen gezamenlijke onderneming | Gedeeld risico en gedeelde motivatie; de schilder profiteert mee van hogere prijzen; eerlijk als je vriend ook meedenkt over verkoop |
| **Nadelen** | Jij draagt het risico (retouren, mislukte beeldjes, weinig verkoop); de schilder profiteert niet mee bij een prijsverhoging; bij lage prijzen eet het vaste bedrag je marge op | Vraagt open boekhouding en afspraken over welke kosten meetellen; uitkomst per beeldje wisselt; bij 50/50 krijgt de schilder weinig per uur omdat schilderen de meeste tijd kost; samen ondernemen met winstdeling kan als vof gezien worden, met hoofdelijke aansprakelijkheid (zie 6.5) |

**Advies:** begin met **optie 1 (vast bedrag per beeldje)** in de testfase: helder, makkelijk vast te leggen en het blijft jouw onderneming. Evalueer na 10–20 beeldjes en stap eventueel over op **winstdeling naar uren (2b)**, wat eerlijker is dan 50/50. Leg vast wie mislukte of afgekeurde beeldjes betaalt.

**Bronnen deel 5**
- Eigen gegevens: Shopify-koppeling (plan Basic, EUR), opgevraagd 4-11-2026; eigen notities over btw, KVK en betaalprovider (geraadpleegd 5-11-2026)
- Shopify 2% bij externe betaalprovider: https://www.trendtrack.io/nl/blog-post/hoeveel-rekent-shopify-per-verkoop-2026 ; https://sellfy.com/nl/blog/shopify-prijzen/ ; https://www.flatlineagency.com/nl/blog/shopify-payments-vs-externe-psps-verborgen-kosten-die-je-moet-kennen/
- Mollie-tarieven: https://www.zunapro.com/netherlands/nl/blog/ideal-betaalmethoden-nederland-online-verkopers ; https://comparepsp.pages.dev/providers/mollie/ ; https://www.emerce.nl/wire/mollie-introduceert-vast-tarief-bancontact
- Etsy-kosten: https://wisepim.com/tools/etsy-fee-calculator ; https://www.gelato.com/nl/blog/etsy-fees
- PostNL: https://www.postnl.nl/api/assets/blt43aa441bfc1e29f2/blt5e65605bca8690e0/tarievenboekje-12-juli-2026.pdf ; https://www.postnl.nl/api/assets/blt43aa441bfc1e29f2/blt4645e1ee01ff026a/tarievenfolder-2026b-EN.pdf
- Wisselkoers: https://tradingeconomics.com/euro-area/currency/news/498610 ; https://30rates.com/eur-usd-forecast-tomorrow-this-week
- Verpakking: https://hyperstack.viv.nl/kartonnen-dozen/verzendkokers

---

## 6. Regels en praktische punten

> Dit is geen juridisch of fiscaal advies. De punten hieronder komen uit de genoemde bronnen; laat twijfelgevallen toetsen door de Belastingdienst, KVK of een adviseur.

### 6.1 Inschrijving, btw en inkomstenbelasting

- **KVK.** Je moet ingeschreven zijn als je zelfstandig producten levert, er een prijs voor vraagt en regelmatig levert aan anderen dan familie en vrienden. Volgens je eigen notities heb je al een eenmanszaak met de handelsnaam Pootjespret. Een nieuwe inschrijving is dan niet nodig; controleer wel of de omschrijving van je activiteiten bij KVK ook "vervaardigen en verkopen van beeldjes" dekt (kosten van een wijziging: niet geverifieerd).
- **Btw-tarief: 21%.** Het verlaagde tarief (9%) voor kunstvoorwerpen geldt alleen voor werk dat helemaal door de kunstenaar zelf is gemaakt, en niet voor serieproducten of reproducties met een commercieel karakter. Een kennisgroep van de Belastingdienst oordeelde specifiek over **3D-geprinte (zwangerschaps)beeldjes** dat de persoonlijke inbreng van de maker te klein was voor 9%. Reken dus met **21%**.
- **KOR.** De kleineondernemersregeling kan bij een omzet tot € 20.000 per kalenderjaar: je rekent dan geen btw, maar trekt ook geen btw af en doet geen aangifte. Aanmelden minstens 4 weken voor het btw-tijdvak; je zit er minimaal 3 jaar aan vast. De KOR geldt voor je **hele** eenmanszaak (dus ook voor je andere activiteiten). Je gebruikt hem nu niet; het model gaat daarom uit van 21% btw.
- **Klanten in België.** Zolang je totale afstandsverkopen aan particulieren in andere EU-landen onder **€ 10.000 per jaar** blijven, reken je Nederlandse btw. Daarboven geldt Belgische btw (via het éénloketsysteem).
- **Inkomstenbelasting.** De winst telt mee als winst uit onderneming van je eenmanszaak.
- **Je vriend.** Is je vriend geen ondernemer, dan is de vergoeding voor het schilderen "inkomsten uit overig werk": die moet je vriend zelf opgeven in de aangifte, met een inkomensafhankelijke bijdrage Zvw; kosten mogen eraf. Heeft je vriend een eigen bedrijf, dan stuurt die een factuur.
- **Uitbetaalde bedragen aan derden.** Wie werk laat doen door iemand die geen factuur met btw stuurt, kan de betalingen moeten doorgeven aan de Belastingdienst. Voor ondernemers zonder personeel gebeurt dat volgens de Belastingdienst op uitnodiging; bronnen spreken elkaar hierover tegen. Leg daarom per betaling naam, adres, geboortedatum en bedrag vast.

### 6.2 Herroepingsrecht en betalen

- **Geen bedenktijd bij maatwerk.** Normaal hebben consumenten bij online aankopen 14 dagen bedenktijd. Volgens de ACM geldt die niet voor producten die volgens de specificaties van de klant zijn gemaakt of die duidelijk persoonlijk zijn. Een beeldje van iemands eigen huisdier op basis van eigen foto's valt daar naar verwachting onder.
- **Maar: smalle uitzondering.** De ACM legt dit strikt uit: kiezen uit standaardopties (zoals alleen een formaat) maakt een product niet gepersonaliseerd, en de verkoper moet kunnen aantonen dat het product aan niemand anders te verkopen is. Bij jullie is dat sterk, omdat elk beeldje naar het eigen dier wordt gemaakt.
- **Wel melden.** Vertel de klant vóór de bestelling duidelijk dat er géén bedenktijd geldt. Ontbreekt die informatie, dan kan de bedenktijd tot een jaar verlengd worden. Laat de klant in de bestelflow een vinkje zetten.
- **Herroepingsknop.** Volgens de ACM moeten webwinkels sinds 25 juni 2026 een knop aanbieden om een koop ongedaan te maken. Dat geldt voor de gewone producten van Pootjespret; zet bij de beeldjes duidelijk dat de uitzondering geldt.
- **Wettelijke garantie blijft.** Komt een beeldje beschadigd aan of wijkt het af van wat is afgesproken, dan heeft de klant gewoon recht op herstel of vervanging.
- **Vooruitbetaling.** Een consument kan niet verplicht worden meer dan **50%** van de prijs van een product vooruit te betalen; een Nederlandse webwinkel moet een betaalmogelijkheid bieden om minstens de helft achteraf te betalen. Praktisch: laat klanten kiezen tussen volledig vooraf betalen of 50% aanbetaling en de rest via een betaallink na de goedkeuringsfoto (zie 3.5).

### 6.3 Veiligheid en etikettering

- **GPSR.** Sinds 13 december 2024 geldt de Europese productveiligheidsverordening (in Nederland via de Warenwet; toezicht NVWA). Wie een product onder eigen naam maakt en verkoopt, geldt als **fabrikant**. Online moet bij het product zichtbaar zijn: de naam en het postadres van de fabrikant, een productaanduiding en eventuele waarschuwingen.
- **Geen speelgoed.** Speelgoed is alles wat bedoeld of kennelijk bestemd is om door kinderen onder de 14 bij het spelen te worden gebruikt. Alleen "geen speelgoed" op het etiket is niet doorslaggevend: ook ontwerp en marketing tellen mee. Presenteer de beeldjes dus als **decoratie en herinnering voor volwassenen**, niet als speelgoed of knuffelvervanger.
- **Voorstel etiket** (sticker onder het voetstuk en op de productpagina): *Pootjespret – handgemaakt decoratief beeldje – geen speelgoed, niet geschikt voor kinderen jonger dan 14 jaar; kleine delen kunnen afbreken – niet in contact brengen met voedsel – afstoffen met een zachte kwast, niet nat reinigen – [postadres] – bestelnummer [xxx]*. De precieze formulering is eigen advies; de verplichte elementen (naam, adres, identificatie, waarschuwingen) volgen uit de GPSR.
- **Resin.** Lever alleen volledig uitgeharde en gewassen prints; vloeibare hars is huidgevoelig (zie 2.2).

### 6.4 De printer van je werkgever

- **Nevenwerk mag meestal.** Sinds 1 augustus 2022 mag een werkgever nevenwerk alleen verbieden met een objectieve reden (zoals veiligheid, vertrouwelijke informatie of belangenverstrengeling). Meld je activiteiten wel vooraf en controleer je contract; een concurrentiebeding blijft gewoon gelden.
- **Gebruik van spullen van de zaak is iets anders.** De printer is eigendom van je werkgever. Vraag daarom **schriftelijk** toestemming voor commercieel gebruik en leg vast:
  1. wanneer je mag printen (buiten werktijd, zonder voorrang op werkprints);
  2. de vergoeding (per printuur, per beeldje of vast per maand) en wie het filament of de hars betaalt; laat je werkgever een factuur sturen, dan is de btw aftrekbaar;
  3. wie betaalt bij slijtage, schade of een mislukte print, en of je werkgever aansprakelijk is;
  4. veiligheid: bij resin ventilatie, handschoenen en de afvoer van hars en IPA (arboregels van je werkgever);
  5. dat je geen bedrijfsinformatie of -bestanden gebruikt;
  6. hoe de afspraak eindigt (bijvoorbeeld een maand opzegtermijn), zodat je niet ineens zonder printer zit.
- **Plan B.** Houd rekening met een eigen printer of een printdienst als je werkgever nee zegt of de printer zelf nodig heeft (prijzen niet onderzocht).

### 6.5 Afspraken met je vriend op papier

- **Kies een vorm.** Bij een **vast bedrag per beeldje** is je vriend opdrachtnemer en blijft het jouw onderneming. Bij **winstdeling** en samen ondernemen ontstaat al snel een **vof**: dan is elke vennoot met privévermogen aansprakelijk voor álle schulden van de vof, ook die van de ander. KVK raadt bij een vof een samenwerkingscontract aan (inbreng, winstverdeling, bevoegdheden, beëindiging).
- **Zet in een korte overeenkomst:** taken (wie doet wat), vergoeding per formaat en betaaltermijn, levertijd per beeldje, kwaliteitseisen en wat er gebeurt bij afkeur of herstel, wie het startpakket betaalt en van wie het is, omgang met klantgegevens en -foto's (alleen gebruiken voor de opdracht), of jullie foto's van het werk mogen gebruiken voor portfolio en social media, naamsvermelding van de schilder, en hoe jullie stoppen.
- **Minderjarig?** Wie jonger is dan 18 heeft voor overeenkomsten toestemming van een ouder of voogd nodig; een contract zonder toestemming kan worden teruggedraaid. Vanaf 16 jaar kan handlichting bij de kantonrechter.

### 6.6 Foto's van klanten en privacy

- De maker van een foto heeft automatisch het **auteursrecht**. Laat de klant bij de bestelling bevestigen dat de foto's van henzelf zijn (of dat ze ze mogen gebruiken) en dat jij ze mag gebruiken om het beeldje te maken.
- Wil je foto's van het eindresultaat of de klantfoto's op je website of social media zetten, vraag dan **aparte toestemming**. Staan er herkenbare mensen op een foto, dan zijn dat persoonsgegevens; vraag liever foto's van alleen het dier.
- Zet in je privacyverklaring dat foto's worden verwerkt met een externe 3D-tool. Gebruik een **betaald** Meshy-plan: modellen van het gratis plan vallen onder CC BY 4.0, terwijl betaalde gebruikers eigenaar worden zolang ze de modellen niet in de Meshy-community publiceren.

**Bronnen deel 6**
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

---

## 7. Productpagina

De concepttekst staat in [`productpagina.md`](productpagina.md), geschreven in de huisstijl van Pootjespret (warm, persoonlijk, "je/jouw"). Opbouw:

1. **Kop en intro** met de belofte: beeldje van het eigen dier, met de hand beschilderd, met twee goedkeuringsmomenten.
2. **Formaten en prijzen**: 8 cm € 59, 12 cm € 79, 15 cm € 99 (incl. btw en verzending NL; België + € 6).
3. **Bestelflow in 6 stappen**: formaat kiezen → foto's uploaden → vachtformulier en aftekeningenkaart → goedkeuring 3D-model → schilderen en goedkeuring kleur → verzenden. Levertijd als invulveld (voorstel: ±3 weken, vast te stellen na de testbeeldjes).
4. **Foto-tips** (zie 1.5).
5. **Goed om te weten**: handwerk, geen bedenktijd (maatwerk), keuze voor betalen (vooraf of 50% aanbetaling), geen speelgoed, onderhoud, materiaal en de verplichte fabrikantgegevens.
6. **Veelgestelde vragen** en **verplichte vinkjes** bij afrekenen (geen bedenktijd, toestemming foto's, optioneel toestemming voor social media).
7. **Notities voor Shopify** (niet voor de klant): varianten, btw aanzetten, uploadoplossing, aanbetaling.

Er staan geen reviews, klantaantallen of verzonnen garanties in. Vul ze pas in als ze echt zijn.

---

## 8. Advies: 5 testbeeldjes deze maand

**Doel:** in november 5 beeldjes maken én verkopen, zo goedkoop mogelijk, om de echte tijd, kosten en reacties te meten.

### 8.1 Goedkoopste opzet

| Onderdeel | Keuze | Kosten (incl. btw) |
|---|---|---|
| 3D-model | Eerst gratis Meshy-plan voor 1–2 proeven met een eigen huisdierfoto (niet verkopen); daarna **Meshy Pro voor één maand** voor de 5 klantmodellen, en weer opzeggen | ± € 17 ($20) |
| Printen | **FDM op de printer van je werk** (na schriftelijke toestemming), grijs PLA, alleen **8 en 12 cm**, 0,12 mm laagdikte, met voetstuk | rol PLA € 22,25 (genoeg voor ±10 beeldjes van 12 cm) + vergoeding werkgever (af te spreken) |
| Schilderen | **Uitgekleed startpakket**: Warpaints Starter Set € 34, penselen € 15,99, Motip-primer € 4,99, Motip filler € 13,37, matte vernis € 9,49; wet palette zelf maken; zijkniptang en hobbymes los of uit eigen gereedschap | ± € 78 (+ gereedschap, prijs niet geverifieerd) |
| Verkopen | **Pootjespret** (bestaand Shopify-abonnement) + je eigen netwerk en de Pootjespret-socials; geen Etsy in de testfase | € 0 extra; betaalkosten ± € 1,60–2 per beeldje |
| Verzenden | Lokaal zelf afgeven waar het kan; anders PostNL | € 0–6,35 per beeldje |
| Verpakking | Doos, vulmateriaal, kaartje | ± € 2 per beeldje |
| **Totaal uitgaven** | | **± € 160–200** voor 5 beeldjes |

Bij een **testprijs van € 49 (8 cm) / € 65 (12 cm)** en 5 verkochte beeldjes is de omzet ± € 245–325 incl. btw (± € 200–270 excl. btw). Je verdient je uitgaven dan ongeveer terug, en je houdt het startpakket en de rest van de rol PLA over. De uren zijn in de testfase nog niet betaald; dat is de prijs van het leren. Spreek met je vriend ook voor de test een vast bedrag af (bijvoorbeeld € 15–20 per beeldje), zodat de afspraak meteen echt is.

Noem de lagere prijs eerlijk een **introductieprijs voor de eerste 5 bestellingen** in ruil voor feedback en (met toestemming) foto's. Toon geen nep-"van"-prijs; de ACM let op misleidende kortingen.

### 8.2 Planning november

| Week | Wat |
|---|---|
| **Wk 45 (5–8 nov)** | Toestemming werkgever (schriftelijk) en printertype vaststellen; afspraak met je vriend op papier (vast bedrag, 1 A4); startpakket en PLA bestellen; proefmodel van een eigen of bekend huisdier maken en printen |
| **Wk 46 (9–15 nov)** | Productpagina live als "eerste 5 plekken"; 5 klanten werven in je netwerk en via Pootjespret; foto's en vachtformulier binnen; Meshy Pro afsluiten; modellen maken en ter goedkeuring sturen |
| **Wk 47 (16–22 nov)** | Printen en nabewerken (filler, schuren, primer); je vriend schildert, tijd bijhouden per beeldje |
| **Wk 48 (23–29 nov)** | Goedkeuringsfoto's, kleine correcties, vernissen, verzenden of afgeven |
| **30 nov** | Evaluatie: echte uren en kosten invullen in `kostprijs.csv`, feedback ophalen, prijs en levertijd vaststellen voor december |

### 8.3 Beslisregels na de test

- **Doorgaan** als klanten het dier herkennen, de echte tijd per 12 cm-beeldje onder ± 5 uur samen ligt en minstens de helft van de klanten zegt het beeldje voor de normale prijs te kopen of aan te raden.
- **Prijs omhoog** naar midden of hoog als de kwaliteit goed is; de marge op het lage niveau dekt jullie uren niet (zie 5.3).
- **Proces aanpassen** als AI-modellen vaak mislukken: vaste houdingen (zittend/liggend), meer foto's vragen, of een freelancer voor lastige dieren.
- **Stoppen of anders inrichten** als de printer niet beschikbaar blijft of de schildertijd veel hoger uitvalt dan geschat.

---
