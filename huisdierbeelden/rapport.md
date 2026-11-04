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
