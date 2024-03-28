# Profilens udgangspunkt og tilblivelse
Denne anvendelsesprofil er det foreløbige resultat af forslaget ’Fællesoffentlig standard for Organisation’, der blev vedtaget af ’Udvalget for arkitektur og standarder’ (UAS) på 6. møde 8 juni 2021. Forslagets hovedindhold var:


>#### Forslag 
>Initiativet har til formål at gøre det lettere at udveksle organisationsoplysninger mellem myndigheder og på tværs af sektorer. Det skal ske ved at skabe én fælles forståelse af hvad organisation er og >hvilke informationer der beskriver en organisation. Der tages afsæt i aktuelle behov og eksisterende erfaringer med forskellige standarder for at beskrive organisationer på tværs af sektorer. 
>
>#### Baggrund 
>Organisationsoplysninger er en fast bestanddel af de offentlige it-løsninger. Oplysninger er særlige relevante når rettigheder skal håndteres, data skal kommunikeres og handlinger skal dokumenteres. >Organisation dækker over flere forskellige aspekter som fx organisationens hierarkiske struktur, kontaktoplysninger, ansvar, roller, opgaver m.fl. Det vil være op til de forskellige anvendelsesscenarier at >afgøre hvilke aspekter der er nødvendige. 
>
>Der anvendes flere forskellige måder at beskrive organisationer på tværs i det offentlige i dag. På sundhedsområdet er det standarden SOR der er bredt anvendt, i kommunerne er det OIO Organisation og i >projekter under FODS har FDA-profilen været anvendt. 
>
>Manglen på fælles sprog om de offentlige organisationer udfordrer kvaliteten i de tværgående processer mellem myndigheder og har bl.a. afledte udfordringer i forhold til at adressere de korrekte >medarbejdere på tværs af myndigheder samt i forhold til at håndtere sikkerhedsmæssige aspekter som fx at håndhæve rettigheder i fælles it-løsninger. Udfordringerne er anerkendt på tværs af såvel stat, >regioner og kommuner - handling efterspørges af alle parter. 
>
>Initiativet skal derfor afdække centrale anvendelsesmæssige behov på tværs af stat, kommuner, regioner med udgangspunkt i erfaringer med førnævnte standarder. Behovsafdækningen skal lede til etablering af >en fællesoffentlig standard til at beskrive organisationer - standarden udarbejdes efter retningslinjerne i de fællesoffentlige regler for modellering (FDA modelregler). For at sikre sammenhæng til >eksisterende- og kommende EU-standardisering, kan en fællesoffentlig standard evt. tage afsæt i den eksisterende FDA-profil for Organisation (baseret på internationale standarder).
>
>Fokus i initiativet er på at frembringe en MVP (Minimum Viable Product) som sikrer at centrale dele af oplysninger om organisationer kan deles mellem myndigheder. MVP’en kan derefter videreudvikles med fx >profiler til at understøtte særlige usecases, fastlæggelse af klassifikationer og/eller etablering af en egentlig referencearkitektur for organisation. 
>
>#### Strategisk ophæng 
>Initiativet understøtter såvel den overordnede vision om en sammenhængene offentlig sektor, samt flere hovedprincipper fra Hvidbogen om Fællesoffentlig digital arkitektur. Et fælles sprog om organisationer >vil højne sammenhængen i den offentlige sektor ved at lette deling og anvendelse af efterspurgte grundlæggende informationer. Et fælles sprog vil ligeledes understøtte målet om at kommunikere effektivt >samt understøtte en sikker håndtering af adgang til fortrolige data.
>
>Det har været længe været en ambition at have en fællesoffentlig standard for Organisation.
>
Med udgangspunkt i det vedtagne forslag blev der dannet en referencegruppe med henblik på at få afdækket centrale anvendelsesmæssige behov på tværs af stat, kommuner, regioner.

Behovsafdækningen resulterede i dokumentet ’Brugerbehov til Fællesoffentlig standard for Organisation’ (reference 1). 

Ud fra brugerbehovene blev der udformet en begrebsmodel som en informationsmodel for organisation. Informationsmodellen startede med at favne stort set alle registrerede behov i en relativt omfattende model, men endte med at fokusere på de centrale elementer for en organisationsmodel. Det er denne seneste model, ’FOOM - kernemodel for organisation’ (reference 2), der har dannet grundlag for udformningen af nærværende anvendelsesprofil. (’FOOM’ står her for ’<ins>**F**</ins>ælles<ins>**o**</ins>ffentlig <ins>**O**</ins>rganisations<ins>**m**</ins>odel’.)

### Profilens anvendelse af eksisterende materiale
I det forslag UAS vedtog stod:

_”For at sikre sammenhæng til eksisterende- og kommende EU-standardisering, kan en fællesoffentlig standard evt. tage afsæt i den eksisterende FDA-profil for Organisation (baseret på internationale standarder).”_

Den FDA-profil der henvises til er baseret på ’The Organization Ontology’   (ORG) og ’Core Public Organisation Vocabulary’   (CPOV). I den nuværende første udgave af basisprofilen er ORG stadig en væsentlig kilde til elementer der indgår i profilen, mens der aktuelt ikke er medtaget elementer fra CPOV. Der er til gengæld gjort brug af en anden specifikation fra EU, Core Location Vocabulary   (LOCN) >til standardiseret angivelse af lokation og adresse. 

I processen er der gjort brug af modellerne for henholdsvis ’Fælleskommunalt Organisationssystem’ (FK-ORG) og ’Sundhedsvæsenets Organisationsregister’ (SOR) for at sammenholde basisprofilen med modeller der anvendes i konkrete systemer. 

## Basisprofiler, API-profiler og udvikling
(Grøn kasse)
NOTE: 
Det anbefales at læse dokumentet ’Anvendelsesprofiler for semantisk interoperabilitet’ for bedre forståelse af efterfølgende information.

(Orange kasse)
Til ovenstående note vil der blive tilføjet et link til anden side i GitHub.


Den fællesoffentlige organisationsmodel udformes som en basisprofil der derefter kan inddrages efter behov til API-profiler for de it-systemer der ønsker at indgå i et semantisk interoperabelt fællesoffentligt landskab.

Basisprofil for organisation vil på den måde blive en semantisk byggeblok der kan bygges videre på af de anvendende systemer. Der vil eksempelvis for FK-ORG og SOR kunne defineres API-profiler hvor de centrale elementer genbruges direkte fra basisprofilen, mens de mere systemspecifikke elementer tilføjes API-profilen. 

Basisprofilen er ikke tænkt som en statisk størrelse. Profilen vil kunne ændres, vi kunne få tilføjes nye elementer i hele profilens levetid. Den primære kilde til fornyelse vil komme fra de API-profiler der benyttes basisprofilen. Hvis det vurderes at to eller flere API-profiler har et sammenfald i funktion OG hvis den funktion vurderes at ville give basisprofilen øget værdi, så fornys basisprofilen. 

## Anvendte vokabularer
I profilen er der anvendt et udvalg af vokabularer. 

For at lette læsbarheden i dokumentet, angives URIer i deres ’QName’ form med enkelte undtagelser. Præfiks og navnrum for de anvendte vokabularer er listet herunder.

(tabel, følgende linjer er indholdet)

| præfiks              | navneområde | titel |
| :---------------- | :------ | :---- |
| rdf      |   http://www.w3.org/1999/02/22-rdf-syntax-ns# 	   | Resource Description Framework |
| rdfs           |   http://www.w3.org/2000/01/rdf-schema#    | RDF Schema  |
| owl    | http://www.w3.org/2002/07/owl#  | Web Ontology Language |
| xsd |  http://www.w3.org/2001/XMLSchema#   | XML Schema |
| vann |  https://vocab.org/vann/  |	VANN: A vocabulary for annotating vocabulary descriptions |
| skos |  http://www.w3.org/2004/02/skos/core#  | Simple Knowledge Organization System  |
| org |  http://www.w3.org/ns/org#  | Organization Ontology |
| cv |  http://data.europa.eu/m8g/  | e-Government Core Vocabulary |
| foaf | http://xmlns.com/foaf/0.1/ | Friend of a Friend |
| dct | http://purl.org/dc/terms/  | Dublin Core Metadata Terms |
| prov | http://www.w3.org/ns/prov#    | The PROV Ontology |
| locn | http://www.w3.org/ns/locn# | Location Core Vocabulary |
| schema | http://schema.org/ | Schema.org |

Følgende vokabularer og de angivne præfikser samt navnerum er oprettet til understøttelse af foreslåede funktioner i anvendelsesprofilen og skal derfor betragtes som værende under udvikling. De er derfor dels ikke stabile og kan ændres eller helt udgå, dels ikke nødvendigvis overholdende ’Retningslinjer for stabile http-URIer’.

| præfiks              | navneområde | titel |
| :---------------- | :------ | :---- |
| ovx      | https://data.gov.dk/model/core/organisation/extension/ | Organization Vocabulary Extension |
| dagi     |  https://data.gov.dk/model/core/dagi/ | Danmarks Administrative Geografiske Inddeling |
| dar           | https://data.gov.dk/model/core/dar/ | Adresseregisteret |
| cvr    | https://data.gov.dk/model/core/registered-business/ | Vokabular for CVR |
| auth | https://data.gov.dk/model/core/authority/  | Vokabular til beskrivelse af myndigheder |

## Vejledning til diagrammer samt definitioner og beskrivelser 
(Orange kasse)
Her indsættes kort beskrivelse  +  link til anden side i GitHub.


 


