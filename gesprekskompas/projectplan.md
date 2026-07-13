# Projectplan Gesprekskompas

**AI-ondersteunde gespreksanalyse voor ouderschapsbemiddeling — compact projectplan**

*Generiek startdocument, bruikbaar als basis voor een subsidieaanvraag, een samenwerking met een hogeschool of universiteit, of een interne pilot binnen de jeugdhulp. Het volledige onderzoeksvoorstel staat in [`onderzoeksvoorstel.md`](onderzoeksvoorstel.md); een visuele schets van het beoogde dashboard in [`dashboard-schets.html`](dashboard-schets.html).*

---

## 1. Samenvatting

Ouderschapsbemiddeling bij complexe scheidingen draait grotendeels om het herkennen en beïnvloeden van gespreksprocessen: spanning, onderbrekingen, verwijten, terugtrekgedrag en herstelbewegingen. Bemiddelaars nemen deze signalen nu vooral intuïtief waar; een systematische manier om ze achteraf zichtbaar en bespreekbaar te maken ontbreekt.

Het project Gesprekskompas ontwikkelt en toetst een prototype van een AI-ondersteunde gespreksanalysetool. Een opgenomen bemiddelingsgesprek wordt getranscribeerd en op meerdere lagen geanalyseerd: inhoud en thema's, stemkenmerken, interactiepatronen en het handelen van de bemiddelaar. De uitkomsten verschijnen in een analyseomgeving met een spanningstijdlijn, themakaart, interactiekaart, kantelpuntkaarten en een gestructureerde gesprekssamenvatting.

De AI is nadrukkelijk een **digitale observator en reflectieassistent**, geen beslisser, diagnosticus of vervanger van de bemiddelaar. Alle uitkomsten zijn toetsbare hypotheses, herleidbaar tot concrete gespreksfragmenten, met betrouwbaarheidsindicatie en alternatieve verklaringen.

Beoogd resultaat: beter onderbouwde reflectie en supervisie, snellere ontwikkeling van gespreksvaardigheden, betere herkenning van escalatie- en herstelpatronen, en uiteindelijk effectievere en veiligere ouderschapsbemiddeling.

## 2. Aanleiding en probleemstelling

Een bemiddelaar moet tijdens een gesprek tegelijk letten op inhoud, emotie, interactie, veiligheid, samenwerking en het perspectief van het kind. Dat gebeurt grotendeels in het moment, waardoor belangrijke patronen onopgemerkt kunnen blijven: terugkerende escalatie bij specifieke onderwerpen, eenzijdig onderbreken, subtiele terugtrekking, gemiste toenaderingspogingen, of momenten waarop het kindperspectief uit het gesprek verdwijnt.

Onderzoek in aangrenzende domeinen (automatische codering van therapeutische gesprekken, motiverende gespreksvoering, multimodale interactieanalyse) laat zien dat de technische bouwstenen bestaan. Voor ouderschapsbemiddeling is echter nog geen geïntegreerd, inhoudelijk gevalideerd systeem beschikbaar dat taal, stem, interactie, spanning en professionele interventies gezamenlijk analyseert.

De kernvraag van het project:

> **Hoe kan AI waarneembare gesprekskenmerken systematisch analyseren en vertalen naar bruikbare, toetsbare hypotheses waarmee bemiddelaars hun gesprekken beter kunnen begrijpen, evalueren en sturen?**

## 3. Doel en onderzoeksvragen

**Doel:** het ontwerpen, ontwikkelen en evalueren van een prototype van een AI-ondersteunde gespreksanalysetool die bemiddelaars helpt spanningsveranderingen te herkennen, interactiepatronen te identificeren, effecten van interventies te onderzoeken en over meerdere gesprekken heen ontwikkeling zichtbaar te maken.

**Centrale onderzoeksvraag:** op welke wijze kan een multimodale AI-gespreksanalysetool bijdragen aan het herkennen, begrijpen en beïnvloeden van spanning, interactiepatronen en herstelbewegingen tijdens ouderschapsbemiddeling?

De negentien deelvragen uit het onderzoeksvoorstel clusteren in drie lijnen:

1. **Technisch** — wat kan betrouwbaar uit audio (en later video) worden gehaald; welke stem- en interactiekenmerken hangen samen met door deskundigen waargenomen spanning; hoeveel voegt multimodale analyse toe boven transcriptanalyse alleen?
2. **Inhoudelijk** — welke gesprekskenmerken zien ervaren bemiddelaars als signalen van escalatie of herstel; welke interactiepatronen en interventies zijn relevant; welke informatie moet de tool presenteren om werkelijk bruikbaar te zijn?
3. **Professioneel** — leidt AI-feedback tot betere zelfreflectie, snellere vaardigheidsontwikkeling, betere supervisie/intervisie en uiteindelijk tot constructievere gesprekken en duurzamere afspraken?

## 4. Aanpak: conceptueel model en werkpakketten

### Conceptueel model — vijf analyselagen

| Laag | Functie |
|---|---|
| 1. Gespreksregistratie | Opname met (bij voorkeur) gescheiden audiokanalen per deelnemer en tijdcodering |
| 2. Transcriptie & sprekerherkenning | Automatische tekst, spreekbeurten, overlap, pauzes; corrigeerbaar door de bemiddelaar |
| 3. Multimodale analyse | Inhoud/thema's en taalpatronen; stemkenmerken t.o.v. persoonlijke uitgangswaarde; interactie (spreektijd, onderbrekingen, beurtwisseling); later eventueel video |
| 4. Patronen & kantelpunten | Signalen samengevoegd op één tijdlijn; sequenties van escalatie en herstel gemarkeerd |
| 5. Professionele ondersteuning | Reflectievragen, interventieanalyse en alternatieve hypotheses — nooit één definitieve interpretatie |

### Werkpakketten

- **WP1 – Verkenning van kennis en technologie.** Systematische verkenning van transcriptie, sprekerherkenning, speech emotion recognition, conversation analysis, automatische codering van hulpverleningsgesprekken en mediation support systems. Opbrengst: overzicht van technieken, datasets, beperkingen en kennislacunes.
- **WP2 – Inhoudelijk codeboek.** Met ervaren bemiddelaars en gedragswetenschappers wordt een codeboek ontwikkeld op vier niveaus: waarneembare gebeurtenissen, interactiepatronen, professionele interventies en verloop na de interventie. Opbrengst: professioneel gedragen annotatiekader.
- **WP3 – Onderzoeksdataset.** Gefaseerde opbouw: eerst gesimuleerde en oefengesprekken (20–30 voor proof of concept), daarna authentieke gesprekken (50–100 voor modelontwikkeling). Dubbele onafhankelijke codering met meting van beoordelaarsovereenstemming.
- **WP4 – Analysemethoden.** Vijf modellen worden ontwikkeld en vergeleken — alleen tekst (A), alleen audio (B), alleen interactie (C), multimodaal (D) en sequentieanalyse (E) — om vast te stellen hoeveel iedere informatielaag werkelijk toevoegt.
- **WP5 – Prototype.** Werkende analyseomgeving met tijdlijn, themakaart, interactiekaart, kantelpuntkaarten, samenvatting en reflectieomgeving. De bemiddelaar kan analyses accepteren, corrigeren, verwijderen en waarderen; die feedback verbetert het systeem.
- **WP6 – Praktijkonderzoek.** Toetsing door bemiddelaars met verschillende ervaringsniveaus in vier condities (geen AI / alleen transcriptie / volledige AI-analyse / AI-ondersteunde supervisie).
- **WP7 – Effectonderzoek.** Vergelijkend onderzoek naar werkrelatie, evenwichtigheid, escalatie en herstel, tevredenheid van ouders en duurzaamheid van afspraken.

## 5. Mijlpalen en planning

Totale doorlooptijd tot en met de praktijkpilot: circa 13–17 maanden. De effectstudie volgt na een positieve pilot.

| Fase | Duur | Mijlpaal | Go/no-go-criterium |
|---|---|---|---|
| 1. Conceptuele verkenning | ~2 mnd | Kennisoverzicht, functionele eisen, ontwerp codeboek | Gedragen probleemdefinitie en committment praktijkpartner |
| 2. Codeboek & oefendataset | ~3 mnd | Geannoteerde oefengesprekken, gemeten beoordelaarsovereenstemming | Voldoende overeenstemming tussen deskundige codeurs |
| 3. Technische proof of concept | ~3 mnd | Werkende pipeline: transcriptie, sprekerherkenning, eerste spanningstijdlijn; modelvergelijking A–E | Detectie van spanningsveranderingen komt aantoonbaar overeen met deskundig oordeel |
| 4. Prototype analyse-app | ~2–3 mnd | Bruikbare interface met kantelpuntkaarten, interventieanalyse en rapportage | Bemiddelaars beoordelen output als herkenbaar en uitlegbaar |
| 5. Praktijkpilot | ~3–6 mnd | Gebruikservaringen, vergelijking met deskundige observaties, verbeterd prototype | Aantoonbare meerwaarde voor reflectie/supervisie; beheersbare foutlast |
| 6. Effectstudie | vervolg | Vergelijkend onderzoek naar professionele vaardigheden en bemiddelingsresultaten | Positieve pilotresultaten en financiering vervolgfase |

## 6. Beoogde onderzoekspartners

Het project vraagt een interdisciplinair consortium. Onderstaande partnertypen zijn beoogd; er zijn nog geen toezeggingen.

| Partnertype | Rol in het project |
|---|---|
| Jeugdhulp- of mediationorganisatie (praktijkpartner) | Inbreng van ervaren ouderschapsbemiddelaars, casuïstiek, oefen- en (later) praktijkgesprekken; toetsing van bruikbaarheid; deelname aan pilot |
| Hogeschool-lectoraat of universitaire vakgroep | Wetenschappelijke leiding, methodologie van praktijk- en effectonderzoek, codeboekontwikkeling, studentprojecten en publicaties |
| AI/NLP-partner (onderzoeksgroep of bedrijf) | Spraaktechnologie, taalmodellen, multimodale analyse, ontwikkeling van de analysemodellen en het prototype |
| Beroepsgroep van mediators / familierecht­professionals | Professionele validatie van het codeboek, aansluiting bij beroepsstandaarden, disseminatie en draagvlak |
| Gedragswetenschappelijke expertise (systeemtherapie, conflictdynamiek) | Inhoudelijke duiding van interactiepatronen, escalatie- en hersteltheorie, begeleiding van annotatie |

Uitgangspunt: bemiddelaars nemen vanaf de eerste fase deel aan de ontwikkeling. Een technisch goed model is onvoldoende wanneer categorieën, visualisaties en suggesties niet aansluiten bij het professionele denken en handelen.

## 7. Begroting (posten, bedragen in te vullen)

Bedragen zijn bewust opengelaten; de invulling hangt af van het gekozen kanaal (subsidieregeling, samenwerkingsvorm of interne pilot), tarieven en cofinanciering.

| Kostenpost | Eenheid / omvang | Fase(n) | Bedrag |
|---|---|---|---|
| Projectleiding en -coördinatie | uren per maand, gehele looptijd | 1–5 | … |
| Inzet ouderschapsbemiddelaars (interviews, codering, pilot) | uren per bemiddelaar | 1–5 | … |
| Gedragswetenschapper / systeemtherapeutisch deskundige | uren | 1–3, 5 | … |
| Methodoloog praktijk- en effectonderzoek | uren | 1–2, 5–6 | … |
| AI/NLP-specialist(en) en audioanalyse | uren | 3–5 | … |
| Softwareontwikkelaar(s) | uren | 3–5 | … |
| UX-ontwerper | uren | 4–5 | … |
| Annotatie en dubbele codering (incl. training codeurs) | per geannoteerd gespreksuur | 2–3 | … |
| Opname-apparatuur (microfoons, evt. camera's) | eenmalig | 2 | … |
| Transcriptie- en rekeninfrastructuur (ASR, opslag, GPU/cloud) | per maand | 3–5 | … |
| Acteurs / simulatiegesprekken voor de oefendataset | per dagdeel | 2 | … |
| Juridisch/ethisch advies en toestemmingsprocedures | eenmalig + uren | 1–2, 5 | … |
| Disseminatie (publicaties, presentaties, trainingsmodule) | stelpost | 5–6 | … |
| Onvoorzien | % van totaal | — | … |

## 8. Risico's en mitigatie

| Risico | Mitigatie |
|---|---|
| Onjuiste interpretatie van signalen (hard praten ≠ spanning) | Signalen altijd combineren en afzetten tegen de persoonlijke uitgangswaarde van de spreker; hypotheses i.p.v. conclusies |
| Verwarring tussen intense emotie en escalatie | Niet emotie willen dempen, maar toetsen of ouders nog kunnen luisteren, reflecteren en samenwerken |
| Overbelasting van de bemiddelaar door te veel meldingen | Prioriteren: alleen de belangrijkste kantelpunten tonen; bruikbaarheid expliciet meten in WP6 |
| Bevestigingsbias door één AI-interpretatie | Altijd alternatieve verklaringen en betrouwbaarheidsindicatie tonen; correctiemogelijkheid voor de bemiddelaar |
| Gebrek aan geannoteerde trainingsdata voor dit domein | Gefaseerde datasetopbouw (simulatie → oefening → praktijk) en codeboekontwikkeling als volwaardig werkpakket |

Daarnaast gelden culturele en persoonlijke verschillen in spreekstijl als doorlopend aandachtspunt, en wordt het verschil tussen samenhang en oorzaak (interventie → spanningsafname) steeds als "mogelijke samenhang" gerapporteerd.

## 9. Eindproducten en vervolg

Het project levert op: (1) een onderbouwd model van gespreksdynamiek bij ouderschapsbemiddeling, (2) een codeboek voor escalatie, herstel, interactie en interventies, (3) een geannoteerde onderzoeksdataset, (4) een werkend prototype met spanningstijdlijn, thema- en interactieanalyse en kantelpuntkaarten, (5) een reflectie- en supervisiemethodiek, (6) een trainingsmodule voor beginnende en ervaren bemiddelaars, en (7) aanbevelingen voor vervolgonderzoek en implementatie.

Een interactieve schets van hoe de analyseomgeving eruit kan zien — spanningstijdlijn, themakaart, interactiekaart, kantelpuntkaarten, gesprekssamenvatting en longitudinaal overzicht, gevuld met fictieve data — is opgenomen als [`dashboard-schets.html`](dashboard-schets.html).

Na een positieve pilot en effectstudie is doorontwikkeling denkbaar richting subtiele realtime-ondersteuning tijdens gesprekken en gerichte feedback en psycho-educatie voor ouders; beide vallen buiten de scope van dit plan.
