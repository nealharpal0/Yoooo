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
