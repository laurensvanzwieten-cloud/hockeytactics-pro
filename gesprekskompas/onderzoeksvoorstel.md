# Onderzoeksvoorstel

## AI-ondersteunde gespreksanalyse voor ouderschapsbemiddeling

**Werktitel van het project:** Gesprekskompas — AI-ondersteunde gespreksanalyse voor ouderschapsbemiddeling

> Bijbehorende documenten in deze map:
> - [`projectplan.md`](projectplan.md) — compact projectplan (~5 pagina's) op basis van dit voorstel
> - [`dashboard-schets.html`](dashboard-schets.html) — interactieve schets van de analyse-app met fictieve data
> - [`app.html`](app.html) — werkend prototype: plak een transcript en het dashboard wordt automatisch gevuld (regelgebaseerd, optioneel met AI)

---

## 1. Samenvatting

Ouderschapsbemiddeling bestaat voor een belangrijk deel uit het herkennen en beïnvloeden van complexe gespreksprocessen. Een bemiddelaar luistert niet alleen naar wat ouders zeggen, maar let ook op de manier waarop zij spreken, op stemverheffing, stiltes, onderbrekingen, herhalingen, verwijten, terugtrekgedrag, emotionele reacties en verschuivingen in de spanning.

Veel van deze signalen worden momenteel door de bemiddelaar intuïtief waargenomen. Er bestaat echter nauwelijks een systematische manier om achteraf zichtbaar te maken:

- wanneer de spanning in een gesprek toenam of afnam;
- welke onderwerpen en formuleringen daarmee samenhingen;
- welke interactiepatronen tussen ouders zichtbaar werden;
- welke interventies van de bemiddelaar de spanning versterkten of verminderden;
- welke vragen of gesprekstechnieken op een bepaald moment behulpzaam hadden kunnen zijn;
- en welke kennis ouders nodig hebben om meer grip te krijgen op hun eigen communicatie.

Dit onderzoeksvoorstel richt zich op de ontwikkeling en toetsing van een AI-ondersteunde gespreksanalysetool voor ouderschapsbemiddeling. De tool neemt in eerste instantie geen beslissingen en neemt de rol van de bemiddelaar niet over. De AI functioneert als een digitale observator en reflectieassistent.

Een opgenomen gesprek wordt getranscribeerd en vervolgens geanalyseerd op meerdere informatielagen:

1. de letterlijke inhoud van het gesprek;
2. thema's, belangen, behoeften, standpunten en terugkerende formuleringen;
3. stemkenmerken zoals tempo, volume, toonhoogte, pauzes en veranderingen daarin;
4. interactiekenmerken zoals onderbrekingen, spreektijd, beurtwisseling en escalatiepatronen;
5. eventueel zichtbare non-verbale signalen uit videobeelden;
6. het handelen van de bemiddelaar en de reactie die daarop volgt.

De uitkomsten worden weergegeven in een analyseomgeving met onder meer een spanningstijdlijn, thematische kaarten, interactiepatronen, gemarkeerde kantelpunten en mogelijke interventies.

Het uiteindelijke doel is te onderzoeken of een dergelijke tool kan bijdragen aan:

- betere reflectie door bemiddelaars;
- snellere ontwikkeling van professionele gespreksvaardigheden;
- betere herkenning van escalatie- en herstelpatronen;
- meer doelgerichte supervisie en intervisie;
- meer grip voor ouders op hun onderlinge communicatie;
- en uiteindelijk effectievere en veiligere ouderschapsbemiddeling.

---

## 2. Aanleiding

Ouderschapsbemiddeling bij complexe scheidingen vraagt van een bemiddelaar dat deze tegelijkertijd aandacht heeft voor inhoud, emotie, onderlinge interactie, veiligheid, samenwerking en het perspectief van het kind.

Tijdens een gesprek kunnen verschillende processen door elkaar lopen. Een ogenschijnlijk praktisch onderwerp, zoals de overdracht van de kinderen, kan verbonden zijn met onderliggende thema's als erkenning, vertrouwen, controle, verlies, angst, gelijkwaardigheid of ervaren onrecht.

De bemiddelaar moet voortdurend inschatten:

- waar het gesprek op inhoudsniveau over gaat;
- welke onderliggende betekenis het onderwerp voor beide ouders heeft;
- welke spanning ontstaat;
- of ouders nog in staat zijn om naar elkaar te luisteren;
- of een interventie nodig is;
- welke interventie op dat moment passend is;
- en wanneer de aandacht opnieuw naar het kind of naar een concreet besluit kan worden gebracht.

Dit gebeurt grotendeels in het moment. Daardoor is het voor bemiddelaars moeilijk om alle gesprekspatronen tegelijk waar te nemen en achteraf nauwkeurig te reconstrueren.

AI kan mogelijk een deel van deze observatielast ondersteunen. Onderzoek in aangrenzende gebieden laat zien dat AI al gebruikt wordt voor het automatisch coderen van therapeutische gespreksinterventies, het herkennen van gedrag binnen motiverende gespreksvoering, het samenvatten van gesprekken en het analyseren van verbale en non-verbale interacties. Er bestaan bovendien Nederlandstalige en tweetalige datasets waarin gespreksuitingen zijn gekoppeld aan professionele gedragscodes. Denkbaar is daarmee een systeem dat niet de hulpverlener vervangt, maar als digitale gespreksobservator gedragingen classificeert, belangrijke signalen markeert en mogelijke volgende interventietypen voorspelt.

Voor ouderschapsbemiddeling lijkt een geïntegreerde en inhoudelijk gevalideerde toepassing van deze technieken echter nog nauwelijks beschikbaar. De voorlopige verkenning wijst vooral op losse bouwstenen, maar niet op een compleet systeem waarin taal, stem, interactie, spanning, professionele interventies en bemiddelingsdoelen gezamenlijk worden geanalyseerd.

---

## 3. Probleemstelling

Bemiddelaars beschikken tijdens en na gesprekken over veel relevante informatie, maar deze informatie is vluchtig, moeilijk systematisch te ordenen en sterk afhankelijk van menselijke aandacht en interpretatie.

Daardoor kunnen belangrijke patronen onopgemerkt blijven, zoals:

- terugkerende escalatie bij specifieke onderwerpen;
- het herhaaldelijk onderbreken of corrigeren van één ouder;
- subtiele terugtrekking of afname van deelname;
- snelle verschuivingen van praktische onderwerpen naar oude conflicten;
- formuleringen die bij de andere ouder defensiviteit oproepen;
- interventies van de bemiddelaar waarna ouders juist rustiger of gespannener reageren;
- momenten waarop een ouder toenadering zoekt, maar dit door de ander niet wordt herkend;
- en momenten waarop het perspectief van het kind uit het gesprek verdwijnt.

Er is behoefte aan een instrument dat deze processen zichtbaar maakt zonder te suggereren dat AI de gedachten, emoties of bedoelingen van ouders met zekerheid kan vaststellen.

De kern van het probleem is daarom:

> **"Hoe kan AI waarneembare gesprekskenmerken systematisch analyseren en vertalen naar bruikbare, toetsbare hypotheses waarmee bemiddelaars hun gesprekken beter kunnen begrijpen, evalueren en sturen?"**

---

## 4. Doelstelling

Het doel van het onderzoek is het ontwerpen, ontwikkelen en evalueren van een prototype van een AI-ondersteunde gespreksanalysetool voor ouderschapsbemiddeling.

De tool moet bemiddelaars helpen om:

1. veranderingen in de interactiespanning te herkennen;
2. de relatie tussen gespreksthema's en spanningsveranderingen zichtbaar te maken;
3. terugkerende communicatiepatronen te identificeren;
4. de effecten van bemiddelingsinterventies te onderzoeken;
5. mogelijke alternatieve interventies te formuleren;
6. ouders gerichte feedback en psycho-educatie te geven;
7. en over meerdere gesprekken heen ontwikkeling of terugval zichtbaar te maken.

Het onderzoek richt zich nadrukkelijk op ondersteuning van professioneel handelen. De AI wordt niet ontwikkeld als autonome beoordelaar, diagnosticus of vervanger van de bemiddelaar.

---

## 5. Centrale onderzoeksvraag

> **Op welke wijze kan een multimodale AI-gespreksanalysetool bijdragen aan het herkennen, begrijpen en beïnvloeden van spanning, interactiepatronen en herstelbewegingen tijdens ouderschapsbemiddeling?**

### Deelvragen

#### Technische deelvragen

1. Welke informatie kan betrouwbaar uit audio-opnamen van bemiddelingsgesprekken worden gehaald?
2. Welke aanvullende waarde hebben videobeelden ten opzichte van uitsluitend audio en transcriptie?
3. Welke stemkenmerken hangen samen met door deskundigen waargenomen veranderingen in spanning?
4. Hoe kunnen spreektijd, onderbrekingen, stiltes, overlap en beurtwisseling automatisch worden herkend?
5. Hoe kunnen gespreksthema's en spanningsveranderingen op een gezamenlijke tijdlijn worden weergegeven?
6. Kan AI onderscheid leren maken tussen escalatie, tijdelijke emotionele betrokkenheid en constructieve confrontatie?
7. In hoeverre verbetert een combinatie van tekst, stem, interactie en beeld de analyse ten opzichte van transcriptanalyse alleen?

#### Inhoudelijke deelvragen

8. Welke gesprekskenmerken beschouwen ervaren ouderschapsbemiddelaars als signalen van oplopende spanning?
9. Welke kenmerken wijzen volgens hen op herstel, reflectie, erkenning of toenemende samenwerking?
10. Welke terugkerende interactiepatronen zijn relevant voor ouderschapsbemiddeling?
11. Welke interventies gebruiken bemiddelaars om deze patronen te beïnvloeden?
12. Welke reacties van ouders kunnen worden gebruikt om het directe effect van een interventie te beoordelen?
13. Welke informatie moet de AI presenteren om voor een bemiddelaar werkelijk bruikbaar te zijn?
14. Welke feedback kan aan ouders worden gegeven zonder hen vast te zetten in etiketten of veronderstelde intenties?

#### Professionele deelvragen

15. Leidt AI-feedback tot betere zelfreflectie van bemiddelaars?
16. Kunnen beginnende bemiddelaars met behulp van de tool sneller professionele gespreksvaardigheden ontwikkelen?
17. Ondersteunt de tool supervisie, intervisie en methodische kwaliteitsbewaking?
18. Verandert het gebruik van de tool de keuze en timing van interventies?
19. Leidt gebruik van de tool tot meer constructieve gesprekken of duurzamere afspraken?

---

## 6. Uitgangspunten

### 6.1 Waarneembare signalen staan centraal

De AI moet zo veel mogelijk beginnen bij observeerbare gegevens:

- wie spreekt;
- welke woorden worden gebruikt;
- hoe snel iemand spreekt;
- hoe lang iemand spreekt;
- waar stiltes vallen;
- waar mensen elkaar onderbreken;
- hoe stemvolume en toonhoogte veranderen;
- en welke reactie volgt op een uitspraak of interventie.

Pas daarna mag de AI hypotheses formuleren over mogelijke betekenis.

De tool moet bijvoorbeeld **niet** stellen:

> "Deze ouder is boos omdat hij controle wil houden."

Een betere formulering is:

> "Na het onderwerp 'wijziging van de zorgregeling' nam het stemvolume toe, werd het spreektempo hoger en volgden drie onderbrekingen. Mogelijke hypothese: dit onderwerp roept spanning op rond voorspelbaarheid, zeggenschap of ervaren ongelijkheid."

### 6.2 Spanning is geen eenvoudige emotie

Een hoge mate van emotionele activering is niet automatisch negatief. Emotie kan ook wijzen op betrokkenheid, verdriet, opluchting of een belangrijk inzicht.

Daarom wordt in dit onderzoek bij voorkeur gesproken over:

- interactiespanning;
- gespreksactivatie;
- escalatierisico;
- herstelbewegingen;
- en gespreksbelasting.

De AI moet geen emotionele diagnoses stellen, maar veranderingen en combinaties van signalen markeren.

### 6.3 AI genereert hypotheses

De uitkomsten zijn bespreekbare hypotheses en geen objectieve waarheden. De bemiddelaar moet steeds kunnen zien waarop een conclusie is gebaseerd.

Bij iedere analyse hoort daarom:

- het gemarkeerde gespreksfragment;
- de gebruikte taalsignalen;
- de relevante stem- of interactiekenmerken;
- een betrouwbaarheidsindicatie;
- mogelijke alternatieve verklaringen;
- en een mogelijkheid voor de bemiddelaar om de analyse te corrigeren.

### 6.4 Eerst achteraf analyseren, daarna eventueel live ondersteunen

De eerste versie van de tool wordt ontwikkeld voor analyse na afloop van het gesprek.

Dit heeft drie voordelen:

1. de bemiddelaar wordt tijdens het gesprek niet afgeleid;
2. analyses kunnen rustig worden gecontroleerd;
3. eerst kan worden vastgesteld welke signalen voldoende betrouwbaar en bruikbaar zijn.

Pas in een latere onderzoeksfase wordt onderzocht of subtiele realtimeondersteuning mogelijk is.

---

## 7. Conceptueel model van de gespreksanalysetool

De voorgestelde tool bestaat uit vijf analyselagen.

### Laag 1 – Gespreksregistratie

Het gesprek wordt opgenomen met:

- één centrale microfoon of meerdere richtmicrofoons;
- eventueel afzonderlijke audiokanalen per deelnemer;
- eventueel één of meer camera's;
- en een tijdcodering waarmee tekst, audio en beeld exact aan elkaar worden gekoppeld.

Bij voorkeur worden de stemmen van beide ouders en de bemiddelaar afzonderlijk geregistreerd. Dit maakt sprekerherkenning en analyse van onderbrekingen nauwkeuriger.

### Laag 2 – Transcriptie en sprekerherkenning

De opname wordt automatisch omgezet naar tekst.

De software bepaalt:

- welke deelnemer spreekt;
- wanneer een spreekbeurt begint en eindigt;
- waar sprake is van overlap;
- waar pauzes vallen;
- welke woorden onzeker zijn herkend;
- en op welk moment iedere uitspraak plaatsvindt.

De bemiddelaar kan de transcriptie waar nodig corrigeren.

### Laag 3 – Multimodale analyse

#### A. Inhoudelijke analyse

De AI herkent mogelijke gespreksthema's, zoals:

- zorgregeling;
- overdrachtsmomenten;
- vakantie;
- financiën;
- school;
- medische beslissingen;
- opvoedregels;
- communicatie;
- nieuwe partners;
- vertrouwen;
- veiligheid;
- erkenning;
- zeggenschap;
- gelijkwaardigheid;
- en het perspectief van het kind.

Daarnaast kan de AI zoeken naar taalpatronen, waaronder:

- beschuldigingen;
- generalisaties zoals "altijd" en "nooit";
- intentietoeschrijvingen;
- sarcasme;
- dreigementen;
- herhalingen;
- defensieve rechtvaardigingen;
- correcties;
- vermijding;
- erkenning;
- samenvatting;
- zelfreflectie;
- verantwoordelijkheid nemen;
- toekomstgerichte taal;
- oplossingsvoorstellen;
- en herstelpogingen.

#### B. Analyse van stemkenmerken

De tool onderzoekt veranderingen in:

- spreektempo;
- volume;
- toonhoogte;
- toonhoogtevariatie;
- stemintensiteit;
- pauzeduur;
- ademhalingsmomenten;
- haperingen;
- versnellingen;
- vertragingen;
- en veranderingen ten opzichte van de persoonlijke uitgangswaarde van de spreker.

Een hogere stem of sneller spreken hoeft niet automatisch spanning te betekenen. De betekenis wordt onderzocht in combinatie met inhoud, interactie en verloop.

#### C. Analyse van interactie

De tool brengt onder meer in kaart:

- verdeling van spreektijd;
- lengte van spreekbeurten;
- frequentie van onderbrekingen;
- wie wie onderbreekt;
- mate van overlap;
- vragen die niet worden beantwoord;
- onderwerpen die worden vermeden;
- herhaalde terugkeer naar hetzelfde punt;
- reactievertraging;
- wederzijdse erkenning;
- herstel na een conflictmoment;
- en de mate waarin ouders rechtstreeks of via de bemiddelaar communiceren.

#### D. Visuele analyse

In een latere onderzoeksfase kunnen videobeelden worden gebruikt voor het onderzoeken van:

- veranderingen in lichaamshouding;
- wegkijken of toenadering;
- gezichtsactiviteit;
- gespannen of ontspannen houding;
- knikken en afwijzende bewegingen;
- synchronisatie tussen gesprekspartners;
- en veranderingen na een interventie.

Onderzoek naar motiverende gespreksvoering laat zien dat dynamiek in gezichtsuitdrukkingen gekoppeld kan worden aan verschillende typen uitspraken van cliënten en hulpverleners. Dit ondersteunt het idee dat beeldanalyse aanvullende informatie kan geven, maar niet dat een afzonderlijke gezichtsuitdrukking een eenduidige betekenis heeft.

### Laag 4 – Detectie van patronen en kantelpunten

De verschillende signalen worden samengevoegd op een tijdlijn.

De tool markeert bijvoorbeeld:

- start van een spanningsstijging;
- vermoedelijke aanleiding;
- betrokken gespreksthema;
- uitspraken die de spanning verder verhogen;
- reactie van de andere ouder;
- interventie van de bemiddelaar;
- en het verdere verloop van de spanning.

Hierdoor kan een sequentie zichtbaar worden zoals:

> Onderwerp schoolkeuze → correctie door ouder A → stemverheffing ouder B → onderbreking door ouder A → generalisatie over het verleden → samenvatting door bemiddelaar → vertraging spreektempo → formulering van onderliggende zorg → afname van onderbrekingen.

De analyse richt zich daarmee niet alleen op losse uitspraken, maar vooral op opeenvolgende interactiepatronen.

### Laag 5 – Professionele ondersteuning

De AI formuleert mogelijke reflectievragen en interventies, zoals:

- "Welke onderliggende zorg lijkt hier nog niet erkend?"
- "Kan de bemiddelaar eerst vertragen en beide ouders afzonderlijk laten samenvatten?"
- "Is het behulpzaam om onderscheid te maken tussen het concrete verzoek en de betekenis die eraan wordt gegeven?"
- "Kan worden teruggekeerd naar het belang van het kind?"
- "Is dit een moment voor erkenning, begrenzing, structurering of concretisering?"
- "Welke poging tot toenadering is mogelijk gemist?"
- "Welke vraag kan helpen om van standpunt naar belang te bewegen?"
- "Is het gesprek nog voldoende wederkerig, of moet eerst de gespreksstructuur worden hersteld?"

Onderzoek naar geautomatiseerde premediation laat overigens zien dat een AI die een deelnemer te vaak bevestigt, een positie juist kan versterken in plaats van flexibiliteit te bevorderen. Dat onderstreept dat interventies niet alleen vriendelijk of empathisch moeten klinken, maar ook moeten worden getoetst op hun effect op perspectiefverbreding en conflictflexibiliteit.

---

## 8. Weergave in de analyse-app

### 8.1 De spanningstijdlijn

Een grafiek toont het verloop van de interactiespanning gedurende het gesprek.

De grafiek bevat afzonderlijke lijnen voor:

- ouder A;
- ouder B;
- de gezamenlijke interactie;
- en eventueel de bemiddelaar.

Op de tijdlijn worden belangrijke gebeurtenissen gemarkeerd:

- nieuw onderwerp;
- duidelijke spanningsstijging;
- onderbreking;
- lange stilte;
- interventie;
- herstelbeweging;
- afspraak;
- en terugval.

### 8.2 De themakaart

De themakaart laat zien:

- hoeveel tijd aan ieder onderwerp is besteed;
- bij welke onderwerpen de meeste spanning ontstond;
- welke onderwerpen constructief besproken konden worden;
- en welke onderwerpen herhaaldelijk terugkeerden zonder besluit.

### 8.3 De interactiekaart

Deze weergave toont bijvoorbeeld:

- verdeling van spreektijd;
- onderbrekingen per deelnemer;
- vragen en antwoorden;
- directe communicatie tussen ouders;
- communicatie via de bemiddelaar;
- en wederzijdse erkenning.

### 8.4 Kantelpuntkaarten

Voor ieder belangrijk moment wordt een kaart aangemaakt met:

1. het relevante transcriptfragment;
2. audio of video van het fragment;
3. gemeten veranderingen;
4. de voorlopige AI-hypothese;
5. de interventie van de bemiddelaar;
6. de reactie die daarop volgde;
7. mogelijke alternatieve interventies;
8. reflectievragen voor supervisie of intervisie.

### 8.5 Gesprekssamenvatting

De tool maakt na afloop een gestructureerde samenvatting van:

- besproken onderwerpen;
- belangen en zorgen per ouder;
- overeenkomsten;
- openstaande geschilpunten;
- gemaakte afspraken;
- momenten van escalatie;
- momenten van samenwerking;
- ingezette bemiddelingsinterventies;
- en aandachtspunten voor een volgend gesprek.

LLM-onderzoek laat zien dat gesprekken al selectief kunnen worden samengevat op afzonderlijke professionele componenten. Voor ouderschapsbemiddeling is daarom een domeinspecifiek samenvattingsmodel denkbaar, mits de uitkomsten aan het oorspronkelijke gesprek controleerbaar gekoppeld blijven.

### 8.6 Ontwikkeling over meerdere gesprekken

Bij meerdere gesprekken kan een longitudinaal overzicht worden gemaakt:

- neemt de wederzijdse onderbreking af;
- worden uitspraken concreter;
- ontstaat meer toekomstgerichte taal;
- kan sneller van standpunt naar belang worden bewogen;
- lukt het beter om het perspectief van het kind vast te houden;
- en herstellen ouders sneller na een spanningsmoment?

---

## 9. Onderzoeksopzet

Het onderzoek wordt uitgevoerd in zeven werkpakketten.

### Werkpakket 1 – Verkenning van bestaande kennis en technologie

Er wordt een systematische verkenning uitgevoerd naar:

- automatische transcriptie en sprekerherkenning;
- conversation analysis;
- affective computing;
- speech emotion recognition;
- multimodale interactieanalyse;
- automatische codering van hulpverleningsgesprekken;
- motiverende gespreksvoering;
- therapeutische procesanalyse;
- mediation support systems;
- conflictanalyse;
- en AI-ondersteunde supervisie.

Een relevant vertrekpunt is onderzoek waarin machine learning wordt gebruikt om onderhandelings- en bemiddelingsgesprekken te ordenen, thema's te extraheren en conflictontwikkelingen inzichtelijk te maken. Daarbij wordt het belang benadrukt van interdisciplinaire ontwikkeling samen met professionals uit het werkveld.

**Opbrengst:** een overzicht van:

- beschikbare technieken;
- meetbare signalen;
- bestaande datasets;
- theoretische modellen;
- bewezen toepassingen;
- beperkingen;
- en ontbrekende kennis voor ouderschapsbemiddeling.

### Werkpakket 2 – Ontwikkeling van een inhoudelijk codeboek

Er wordt samen met ervaren bemiddelaars, gedragswetenschappers en onderzoekers een codeboek ontwikkeld.

Het codeboek bevat ten minste vier niveaus.

#### Niveau A – Waarneembare gebeurtenissen

Bijvoorbeeld:

- onderbreking;
- stilte;
- stemverheffing;
- versnelling;
- herhaling;
- verandering van onderwerp;
- vraag;
- verwijt;
- erkenning;
- samenvatting;
- en afspraak.

#### Niveau B – Interactiepatronen

Bijvoorbeeld:

- aanval en verdediging;
- claim en tegenclaim;
- rechtvaardiging en correctie;
- escalatie door intentietoeschrijving;
- terugtrekken en najagen;
- coalitievorming met de bemiddelaar;
- competitief slachtofferschap;
- gemiste toenadering;
- herstel;
- en gezamenlijke probleemoplossing.

#### Niveau C – Professionele interventies

Bijvoorbeeld:

- vertragen;
- structureren;
- begrenzen;
- samenvatten;
- concretiseren;
- reframen;
- erkenning geven;
- meerzijdige partijdigheid tonen;
- perspectiefwisseling;
- belangen onderzoeken;
- kindperspectief activeren;
- circulaire vragen stellen;
- en afspraken operationaliseren.

#### Niveau D – Verloop na de interventie

Bijvoorbeeld:

- directe spanningsafname;
- tijdelijke spanningsafname;
- verdieping;
- defensieve reactie;
- toename van samenwerking;
- verschuiving naar een nieuw verwijt;
- terugtrekking;
- of geen zichtbaar effect.

**Opbrengst:** een professioneel gedragen annotatie- en beoordelingskader voor AI-analyse.

### Werkpakket 3 – Opbouw van een onderzoeksdataset

Het onderzoek kan gefaseerd beginnen met:

1. gesimuleerde bemiddelingsgesprekken;
2. trainingsgesprekken en rollenspellen;
3. bestaande geanonimiseerde oefenopnamen;
4. en vervolgens authentieke bemiddelingsgesprekken.

Voor een eerste proof of concept kunnen ongeveer twintig tot dertig zorgvuldig gevarieerde oefengesprekken worden gebruikt.

Voor betrouwbare modelontwikkeling is uiteindelijk een grotere dataset nodig, bijvoorbeeld vijftig tot honderd volledige gesprekken, aangevuld met afzonderlijk geannoteerde fragmenten.

Er moet variatie aanwezig zijn in:

- type conflict;
- intensiteit;
- fase van bemiddeling;
- ervaring van de bemiddelaar;
- gespreksstijl van ouders;
- en uitkomst van het gesprek.

Minimaal twee onafhankelijke deskundigen coderen dezelfde fragmenten. De overeenstemming tussen beoordelaars wordt gemeten. Verschillen worden besproken en gebruikt om het codeboek te verbeteren.

### Werkpakket 4 – Ontwikkeling van analysemethoden

Er worden verschillende modellen ontwikkeld en vergeleken.

- **Model A – Tekstanalyse:** gebruikt alleen de transcriptie.
- **Model B – Audioanalyse:** gebruikt stemkenmerken en timing, zonder inhoudelijke interpretatie.
- **Model C – Interactieanalyse:** gebruikt beurtwisseling, onderbrekingen, stiltes en spreektijd.
- **Model D – Multimodale analyse:** combineert tekst, audio, interactie en eventueel video.
- **Model E – Sequentieanalyse:** onderzoekt niet alleen losse momenten, maar patronen van gebeurtenissen voor en na een spanningsverandering.

Door deze modellen te vergelijken kan worden vastgesteld hoeveel iedere informatielaag werkelijk toevoegt.

### Werkpakket 5 – Ontwikkeling van het prototype

Op basis van de resultaten wordt een werkend prototype ontwikkeld met:

- opname-import;
- automatische transcriptie;
- sprekerherkenning;
- tijdlijn;
- thematische analyse;
- spanningsindicatoren;
- kantelpuntkaarten;
- interventieanalyse;
- gesprekssamenvatting;
- en een reflectieomgeving.

De bemiddelaar moet analyses kunnen:

- accepteren;
- corrigeren;
- verwijderen;
- aanvullen;
- en waarderen op bruikbaarheid.

Deze feedback wordt gebruikt om het systeem verder te verbeteren.

### Werkpakket 6 – Praktijkonderzoek

Het prototype wordt getest door bemiddelaars met verschillende ervaringsniveaus.

Mogelijke onderzoekscondities zijn:

1. reguliere reflectie zonder AI;
2. reflectie met transcriptie;
3. reflectie met volledige AI-analyse;
4. supervisie met behulp van AI-gemarkeerde fragmenten.

Onderzocht wordt of AI-ondersteuning leidt tot:

- het herkennen van meer relevante gespreksmomenten;
- grotere overeenstemming met deskundige beoordelaars;
- betere onderbouwing van interventiekeuzes;
- snellere professionele ontwikkeling;
- en betere vervolgstrategieën.

### Werkpakket 7 – Effectonderzoek

Na de haalbaarheidsfase kan een vergelijkend onderzoek worden uitgevoerd.

Hierbij worden gesprekken met en zonder AI-ondersteunde reflectie vergeleken op:

- kwaliteit van de werkrelatie;
- ervaren evenwichtigheid;
- duidelijkheid van afspraken;
- mate van escalatie;
- herstel na spanning;
- tevredenheid van ouders;
- ervaren grip op communicatie;
- en duurzaamheid van afspraken.

---

## 10. Hypothesen

Het onderzoek toetst onder andere de volgende verwachtingen.

**Hypothese 1.** Een multimodaal model dat tekst, stem en interactie combineert, herkent door deskundigen beoordeelde spanningsveranderingen beter dan een model dat alleen de transcriptie analyseert.

**Hypothese 2.** Veranderingen ten opzichte van de persoonlijke uitgangswaarde van een spreker zijn informatiever dan algemene normen voor volume, toonhoogte en spreektempo.

**Hypothese 3.** Opeenvolgende interactiepatronen voorspellen escalatie en herstel beter dan losse woorden of afzonderlijke gezichtsuitdrukkingen.

**Hypothese 4.** AI-feedback na afloop van een gesprek is in de eerste ontwikkelfase bruikbaarder en minder belastend dan realtime aanwijzingen.

**Hypothese 5.** Bemiddelaars vertrouwen AI-analyses meer wanneer zij kunnen zien op welke concrete fragmenten en signalen deze zijn gebaseerd.

**Hypothese 6.** Beginnende bemiddelaars profiteren relatief sterk van systematische feedback op beurtwisseling, vraagstelling, samenvatting en timing.

**Hypothese 7.** Ervaren bemiddelaars profiteren vooral van patroonherkenning over meerdere gesprekken en van vergelijking tussen hun interventies en de reacties van ouders.

**Hypothese 8.** AI-ondersteunde reflectie verbetert de professionele gespreksvoering wanneer de tool alternatieve hypotheses presenteert in plaats van één definitieve interpretatie.

---

## 11. Beoordelingscriteria

### Technische kwaliteit

De technische modellen worden beoordeeld op:

- kwaliteit van transcriptie;
- juiste herkenning van sprekers;
- detectie van overlap en onderbrekingen;
- herkenning van gespreksthema's;
- nauwkeurigheid van gedragsclassificaties;
- tijdige detectie van spanningsveranderingen;
- overeenstemming met deskundige beoordelaars;
- en kalibratie van betrouwbaarheidsindicaties.

### Professionele bruikbaarheid

Bemiddelaars beoordelen:

- herkenbaarheid;
- relevantie;
- begrijpelijkheid;
- uitlegbaarheid;
- volledigheid;
- aantal foutieve waarschuwingen;
- hoeveelheid overbodige informatie;
- invloed op reflectie;
- invloed op voorbereiding van vervolggesprekken;
- en bruikbaarheid voor intervisie en supervisie.

### Effect op bemiddelingsvaardigheden

Onderzocht wordt of bemiddelaars beter worden in:

- timing van interventies;
- formuleren van open vragen;
- bewaken van evenwicht;
- herkennen van onderliggende belangen;
- begrenzen van destructieve interactie;
- benutten van herstelpogingen;
- en terugbrengen van het kindperspectief.

---

## 12. Benodigde deskundigheid

Voor het project is een interdisciplinair team nodig met minimaal:

- ervaren ouderschapsbemiddelaars;
- gedragswetenschappers of systeemtherapeutisch deskundigen;
- experts in gespreksanalyse;
- onderzoekers op het gebied van conflictdynamiek;
- AI- en NLP-specialisten;
- specialisten in audioanalyse;
- softwareontwikkelaars;
- UX-ontwerpers;
- data-analisten;
- en methodologen voor praktijk- en effectonderzoek.

Bemiddelaars moeten vanaf het begin deelnemen aan de ontwikkeling. Een technisch goed model is onvoldoende wanneer de categorieën, visualisaties en suggesties niet aansluiten bij het daadwerkelijke professionele denken en handelen.

---

## 13. Voorgestelde fasering

### Fase 1 – Conceptuele verkenning

*Duur: circa twee maanden*

- literatuur- en technologiestudie;
- interviews met bemiddelaars;
- beschrijving van relevante gespreksprocessen;
- eerste functionele eisen;
- en ontwerp van het codeboek.

### Fase 2 – Codeboek en oefendataset

*Duur: circa drie maanden*

- verzamelen of opnemen van oefengesprekken;
- annoteren van fragmenten;
- meten van overeenstemming tussen deskundigen;
- en aanscherpen van definities.

### Fase 3 – Technische proof of concept

*Duur: circa drie maanden*

- transcriptie;
- sprekerherkenning;
- themaherkenning;
- stem- en interactieanalyse;
- eerste spanningstijdlijn;
- en vergelijking van analysemodellen.

### Fase 4 – Prototype van de analyse-app

*Duur: circa twee tot drie maanden*

- ontwikkeling van gebruikersinterface;
- kantelpuntkaarten;
- interventieanalyse;
- rapportage;
- en feedbackmogelijkheden.

### Fase 5 – Praktijkpilot

*Duur: circa drie tot zes maanden*

- gebruik door bemiddelaars;
- verzamelen van gebruikerservaringen;
- vergelijking met deskundige observaties;
- en verbetering van het prototype.

### Fase 6 – Effectstudie

Na een positieve pilot kan worden onderzocht of structureel gebruik daadwerkelijk leidt tot betere professionele vaardigheden en betere bemiddelingsresultaten.

---

## 14. Verwachte risico's en onderzoeksuitdagingen

Hoewel privacy en gegevensbescherming in dit voorstel niet centraal staan, bestaan er verschillende andere inhoudelijke uitdagingen.

### Onjuiste interpretatie van signalen

Een verhoogd stemvolume kan spanning betekenen, maar ook enthousiasme, slechthorendheid of een persoonlijke spreekstijl. Daarom moet de AI signalen combineren en vergelijken met het normale patroon van de betreffende persoon.

### Verwarring tussen spanning en escalatie

Een intens emotioneel gesprek kan juist constructief zijn. De tool moet daarom niet proberen emotie te verminderen, maar onderzoeken of ouders nog kunnen luisteren, reflecteren en samenwerken.

### Culturele en persoonlijke verschillen

Non-verbaal gedrag, stiltes, directe taal en stemgebruik verschillen tussen personen, gezinnen en culturele contexten.

### Overbelasting van de bemiddelaar

Een dashboard met tientallen waarschuwingen maakt de bemiddelaar niet beter. De tool moet prioriteren en vooral de belangrijkste kantelpunten tonen.

### Bevestigingsbias

Wanneer de AI één interpretatie geeft, kan de bemiddelaar die te snel overnemen. Daarom moeten alternatieve verklaringen zichtbaar blijven.

### Gebrek aan goede trainingsdata

Ouderschapsbemiddeling kent nog geen algemeen aanvaarde, uitgebreid geannoteerde dataset. Het ontwikkelen van een betrouwbaar codeboek en een kwalitatieve dataset vormt daarom een essentieel onderdeel van het onderzoek.

### Verschil tussen correlatie en oorzaak

Wanneer de spanning afneemt na een interventie, betekent dit niet automatisch dat de interventie de oorzaak was. Het systeem moet dergelijke relaties beschrijven als mogelijke samenhang.

---

## 15. Beoogde eindproducten

Het project levert uiteindelijk op:

1. een wetenschappelijk en professioneel onderbouwd model van gespreksdynamiek bij ouderschapsbemiddeling;
2. een codeboek voor escalatie, herstel, interactie en bemiddelingsinterventies;
3. een geannoteerde onderzoeksdataset;
4. een werkend prototype van een AI-gespreksanalysetool;
5. een visuele spanningstijdlijn;
6. een thematische en interactionele gespreksanalyse;
7. een systeem voor reflectie op interventies;
8. een trainingsmodule voor beginnende en ervaren bemiddelaars;
9. een methode voor AI-ondersteunde intervisie en supervisie;
10. en aanbevelingen voor vervolgonderzoek en implementatie.

---

## 16. Toekomstbeeld

In de uiteindelijke toepassing importeert de bemiddelaar na een gesprek de opname. Binnen korte tijd ontstaat een interactief gespreksverslag.

De bemiddelaar ziet bijvoorbeeld:

> "De hoogste gezamenlijke interactiespanning ontstond tussen minuut 31 en 36 tijdens het onderwerp 'wijziging van de vakantiedagen'. Beide ouders gingen sneller spreken. Ouder A onderbrak ouder B viermaal. Ouder B gebruikte tweemaal een generalisatie over het verleden. Na een samenvatting en een vraag naar de onderliggende zorg nam het spreektempo af en konden beide ouders een concreet belang formuleren."

Vervolgens toont de tool:

- het oorspronkelijke fragment;
- de signalen waarop de analyse is gebaseerd;
- alternatieve verklaringen;
- het waarschijnlijke effect van de interventie;
- en vragen voor professionele reflectie.

Over meerdere gesprekken kan de bemiddelaar zien dat ouders bijvoorbeeld minder vaak onderbreken, sneller herstellen of beter in staat zijn om hun zorgen zonder beschuldiging te formuleren.

De tool wordt daarmee geen digitale scheidsrechter die bepaalt wie gelijk heeft. Het wordt een instrument dat zichtbaar maakt hoe het gesprek verloopt, waar het vastloopt, waar beweging ontstaat en welke bijdrage de bemiddelaar daaraan levert.

---

## 17. Conclusie

De voorgestelde AI-gespreksanalysetool heeft de potentie om een tot nu toe grotendeels intuïtief professioneel proces beter zichtbaar en onderzoekbaar te maken.

De grootste meerwaarde ligt waarschijnlijk niet in het automatisch herkennen van één specifieke emotie of intentie. De meerwaarde ligt in het combineren van:

- woorden;
- stemveranderingen;
- beurtwisseling;
- gespreksthema's;
- opeenvolgende reacties;
- non-verbaal gedrag;
- en interventies van de bemiddelaar.

Wanneer deze informatie zorgvuldig wordt gekoppeld aan professionele kennis over ouderschapsbemiddeling, kan een systeem ontstaan dat bemiddelaars helpt om niet alleen terug te kijken op wat er is besproken, maar vooral op wat er tussen mensen gebeurde.

Daarmee kan AI bijdragen aan systematischer leren, nauwkeuriger reflecteren en beter getimede interventies, terwijl de menselijke bemiddelaar verantwoordelijk blijft voor betekenisgeving, relatievorming en professionele besluitvorming.

Een compacte uitwerking van dit voorstel — inclusief begrotingsposten, typen onderzoekspartners en concrete mijlpalen — is opgenomen in [`projectplan.md`](projectplan.md). Een visuele schets van het beoogde dashboard is te vinden in [`dashboard-schets.html`](dashboard-schets.html).
