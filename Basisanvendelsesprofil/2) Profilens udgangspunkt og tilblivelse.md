ifikt # Profilens udgangspunkt og tilblivelse
Denne anvendelsesprofil er det foreløbige resultat af forslaget _Fællesoffentlig standard for Organisation_, der blev vedtaget af ’Udvalget for arkitektur og standarder’ (UAS) på 6. møde 8 juni 2021. Forslagets hovedindhold var:


>#### Forslag 
>Initiativet har til formål at gøre det lettere at udveksle organisationsoplysninger mellem myndigheder og på tværs af sektorer. Det skal ske ved at skabe én fælles forståelse af hvad organisation er og  hvilke informationer der beskriver en organisation. Der tages afsæt i aktuelle behov og eksisterende erfaringer med forskellige standarder for at beskrive organisationer på tværs af sektorer. 
>
>#### Baggrund 
>Organisationsoplysninger er en fast bestanddel af de offentlige it-løsninger. Oplysninger er særlige relevante når rettigheder skal håndteres, data skal kommunikeres og handlinger skal dokumenteres.  Organisation dækker over flere forskellige aspekter som fx organisationens hierarkiske struktur, kontaktoplysninger, ansvar, roller, opgaver m.fl. Det vil være op til de forskellige anvendelsesscenarier at  afgøre hvilke aspekter der er nødvendige. 
>
>Der anvendes flere forskellige måder at beskrive organisationer på tværs i det offentlige i dag. På sundhedsområdet er det standarden SOR der er bredt anvendt, i kommunerne er det OIO Organisation og i  projekter under FODS har FDA-profilen været anvendt. 
>
>Manglen på fælles sprog om de offentlige organisationer udfordrer kvaliteten i de tværgående processer mellem myndigheder og har bl.a. afledte udfordringer i forhold til at adressere de korrekte  medarbejdere på tværs af myndigheder samt i forhold til at håndtere sikkerhedsmæssige aspekter som fx at håndhæve rettigheder i fælles it-løsninger. Udfordringerne er anerkendt på tværs af såvel stat,  regioner og kommuner - handling efterspørges af alle parter. 
>
>Initiativet skal derfor afdække centrale anvendelsesmæssige behov på tværs af stat, kommuner, regioner med udgangspunkt i erfaringer med førnævnte standarder. Behovsafdækningen skal lede til etablering af  en fællesoffentlig standard til at beskrive organisationer - standarden udarbejdes efter retningslinjerne i de fællesoffentlige regler for modellering (FDA modelregler). For at sikre sammenhæng til  eksisterende- og kommende EU-standardisering, kan en fællesoffentlig standard evt. tage afsæt i den eksisterende FDA-profil for Organisation (baseret på internationale standarder).
>
>Fokus i initiativet er på at frembringe en MVP (Minimum Viable Product) som sikrer at centrale dele af oplysninger om organisationer kan deles mellem myndigheder. MVP’en kan derefter videreudvikles med fx  profiler til at understøtte særlige usecases, fastlæggelse af klassifikationer og/eller etablering af en egentlig referencearkitektur for organisation. 
>
>#### Strategisk ophæng 
>Initiativet understøtter såvel den overordnede vision om en sammenhængene offentlig sektor, samt flere hovedprincipper fra Hvidbogen om Fællesoffentlig digital arkitektur. Et fælles sprog om organisationer  vil højne sammenhængen i den offentlige sektor ved at lette deling og anvendelse af efterspurgte grundlæggende informationer. Et fælles sprog vil ligeledes understøtte målet om at kommunikere effektivt >samt understøtte en sikker håndtering af adgang til fortrolige data.
>
>Det har været længe været en ambition at have en fællesoffentlig standard for Organisation.

Med udgangspunkt i det vedtagne forslag blev der dannet en referencegruppe med henblik på at få afdækket centrale anvendelsesmæssige behov på tværs af stat, kommuner, regioner.

Behovsafdækningen resulterede i dokumentet _Brugerbehov til Fællesoffentlig standard for Organisation_ [^1]. 

Ud fra brugerbehovene blev der udformet en begrebsmodel som en informationsmodel for organisation. Informationsmodellen startede med at favne stort set alle registrerede behov i en relativt omfattende model, men endte med at fokusere på de centrale elementer for en organisationsmodel. Det er denne seneste model, _FOOM - kernemodel for organisation_ [^2], der har dannet grundlag for udformningen af nærværende anvendelsesprofil. (’FOOM’ står her for ’<ins>**F**</ins>ælles<ins>**o**</ins>ffentlig <ins>**O**</ins>rganisations<ins>**m**</ins>odel’.)

### Profilens anvendelse af eksisterende materiale
I det forslag UAS vedtog stod:

_”For at sikre sammenhæng til eksisterende- og kommende EU-standardisering, kan en fællesoffentlig standard evt. tage afsæt i den eksisterende FDA-profil for Organisation (baseret på internationale standarder).”_

Den FDA-profil der henvises til er baseret på _The Organization Ontology_ [^3] (ORG) og _Core Public Organisation Vocabulary_ [^4] (CPOV). I den nuværende første udgave af basisprofilen er ORG stadig en væsentlig kilde til elementer der indgår i profilen, mens der aktuelt ikke er medtaget elementer specifikt fra CPOV. Der er til gengæld gjort brug af en anden specifikation fra EU, _Core Location Vocabulary_ [^5]  (LOCN) >til standardiseret angivelse af lokation og adresse. 

I processen er der gjort brug af modellerne for henholdsvis _Fælleskommunalt Organisationssystem_ (FK-ORG) og _Sundhedsvæsenets Organisationsregister_ (SOR) for at sammenholde basisprofilen med modeller der anvendes i konkrete systemer. 

## Basisprofiler, API-profiler og udvikling
> [!NOTE]  
> Det anbefales at læse dokumentet _Anvendelsesprofiler for semantisk interoperabilitet_ for at opnå en bedre forståelse af den efterfølgende information.
> Denne note skal tilføjes link til anden side i GitHub.


Den fællesoffentlige organisationsmodel udformes som en basisprofil der derefter kan inddrages efter behov til API-profiler for de it-systemer der ønsker at indgå i et semantisk interoperabelt fællesoffentligt landskab.

Basisprofil for organisation vil på den måde blive en semantisk byggeblok der kan bygges videre på af de anvendende systemer. Der vil eksempelvis for FK-ORG og SOR kunne defineres API-profiler hvor de centrale elementer genbruges direkte fra basisprofilen, mens de mere systemspecifikke elementer tilføjes API-profilen. 

Basisprofilen er ikke tænkt som en statisk størrelse. Profilen vil kunne ændres, vi kunne få tilføjes nye elementer i hele profilens levetid. Den primære kilde til fornyelse vil komme fra de API-profiler der benyttes basisprofilen. Hvis det vurderes at to eller flere API-profiler har et sammenfald i funktion OG hvis den funktion vurderes at ville give basisprofilen øget værdi, så fornys basisprofilen. 

## Anvendte vokabularer
I profilen er der anvendt et udvalg af vokabularer. 

For at lette læsbarheden i dokumentet, angives URIer i deres ’QName’ form med enkelte undtagelser. Præfiks og navnrum for de anvendte vokabularer er listet herunder.

<table>
<tr>
    <td><b>præfiks</b></td>
    <td><b>navneområde</b></td>
    <td><b>titel</b></td>
</tr>
<tr>
    <td>rdf</td>
    <td>http://www.w3.org/1999/02/22-rdf-syntax-ns#</td>
    <td>Resource Description Framework</td>
</tr>
<tr>
    <td>rdfs</td>
    <td>http://www.w3.org/2000/01/rdf-schema#</td>
    <td>RDF Schema</td>
</tr>
<tr>
    <td>owl</td>
    <td>http://www.w3.org/2002/07/owl#</td>
    <td>Web Ontology Language</td>
</tr>
<tr>
    <td>xsd</td>
    <td>http://www.w3.org/2001/XMLSchema#</td>
    <td>XML Schema</td>
</tr>
<tr>
    <td>vann</td>
    <td>https://vocab.org/vann/</td>
    <td>VANN: A vocabulary for annotating vocabulary descriptions</td>
</tr>
<tr>
    <td>skos</td>
    <td>http://www.w3.org/2004/02/skos/core#</td>
    <td>Simple Knowledge Organization System</td>
</tr>
<tr>
    <td>org</td>
    <td>http://www.w3.org/ns/org#</td>
    <td>Organization Ontology</td>
</tr>
<tr>
    <td>cv</td>
    <td>http://data.europa.eu/m8g/</td>
    <td>e-Government Core Vocabulary</td>
</tr>
<tr>
    <td>foaf</td>
    <td>http://xmlns.com/foaf/0.1/</td>
    <td>Friend of a Friend</td>
</tr>
<tr>
    <td>dct</td>
    <td>http://purl.org/dc/terms/</td>
    <td>Dublin Core Metadata Terms</td>
</tr>
<tr>
    <td>prov</td>
    <td>http://www.w3.org/ns/prov#</td>
    <td>The PROV Ontology</td>
</tr>
<tr>
    <td>locn</td>
    <td>http://www.w3.org/ns/locn#</td>
    <td>Location Core Vocabulary</td>
</tr>
<tr>
    <td>schema</td>
    <td>http://schema.org/</td>
    <td>Schema.org</td>
</tr>
</table>


Følgende vokabular og det angivne præfiks samt navnerum er oprettet til understøttelse af foreslåede funktioner i anvendelsesprofilen og skal derfor betragtes som værende under udvikling. Det er derfor dels ikke stabilt, kan ændres eller helt udgå, dels ikke nødvendigvis overholdende ’Retningslinjer for stabile http-URIer’.

<table>
<tr>
    <td><b>præfiks</b></td>
    <td><b>navneområde</b></td>
    <td><b>titel</b></td>
</tr>
<tr>
    <td>ovx</td>
    <td>https://data.gov.dk/model/core/organisation/extension/</td>
    <td>Organization Vocabulary Extension</td>
</tr>
</table>

## Vejledning til diagrammer samt definitioner og beskrivelser 
(Orange kasse)
Her indsættes kort beskrivelse  +  link til anden side i GitHub.


 
[^1]: https://github.com/digst/ORG-AP-DK/blob/main/releases/v.1.0/business/Brugerbehov%20til%20F%C3%A6llesoffentlig%20standard%20for%20Organisation%20%E2%80%93%202022-02-18_KL20221014.docx
[^2]: https://github.com/digst/ORG-AP-DK/blob/main/releases/v.1.0/business/FOOM%20-%20f%C3%A6llesoffentligOrganisationsmodel%20v07.docx
[^3]: https://www.w3.org/TR/vocab-org/
[^4]: https://semiceu.github.io/CPOV/releases/2.00/
[^5]: https://semiceu.github.io/Core-Location-Vocabulary/releases/2.00/


