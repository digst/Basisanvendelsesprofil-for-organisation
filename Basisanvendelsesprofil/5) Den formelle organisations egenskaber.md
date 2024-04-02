# Den formelle organisations egenskaber

(billede) 

## Organisationens identifikation og beskrivelse
 

**foretrukken term**
_**Vokabular-definition og beskrivelser**_
<table>
<tr>
    <td>URI</td>
    <td>http://www.w3.org/2004/02/skos/core#prefLabel</td>
</tr>
<tr>
    <td>Term</td>
    <td>foretrukken term</td>
</tr>
<tr>
    <td>Definition</td>
    <td>Den foretrukne leksikalske betegnelse for en ressource på et givet sprog.</td>
</tr>
<tr>
    <td>Kommentar</td>
    <td>En ressource har ikke mere end én værdi af skos:prefLabel pr. sprogtag. <br> Range for skos:prefLabel er klassen af RDF ’plain literals’. <br> skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte egenskaber.</td>
</tr>
<tr>
    <td>Domæne</td>
    <td>rdfs:Resource</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>xsd:string eller rdf:langString (tidligere angivet som rdf:PlainLiteral)</td>
</tr>
<tr>
    <td>Underegenskab af</td>
    <td>rdfs:label</td>
</tr>
</table>

_**Profilens kontekstrestriktioner og annotationer**_ 
<table>
<tr>
    <td>Definition</td>
    <td><span style="color🚙">[fra informationsmodel] alment anvendt navn for en organisation</span></td>
</tr>
<tr>
    <td>Kommentar</td>
    <td><span style="color🚙">[fra informationsmodel]Ofte vil organisationens navn være det samme som man finder i CVR-registret eller Myndighedsregistret, når der er tale om virksomheders og myndigheders navne.</span></td>
</tr>
<tr>
    <td>Anvendelsesnote</td>
    <td>Bruges til at angive organisationens primære - ofte juridisk anerkendte - navn. Det antages at organisationer kun har et enkelt navn eller en enkelt betegnelse som det foretrukne, eventuelt med oversatte versioner på andre sprog. Med andre ord kan primære navne angives på flere sprog og dermed give flere forekomster af egenskaben skos:prefLabel for den enkelte organisation.</td>
</tr>
<tr>
    <td>Eksempel</td>
    <td><span style="color🚙">[fra informationsmodel] <br> o "Digitaliseringsstyrelsen" <br> o "Næstved Sygehus" <br> o "Holbæk kommune" <br> o "FDF-spejderne i Vejle</span>"
    </td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>rdf:langString</td>
</tr>
<tr>
    <td>Multiplicitet</td>
    <td>1 - *</td>
</tr>
</table>

**alternativ term**
_**Vokabular-definition og beskrivelser**_
<table>
<tr>
    <td>URI</td>
    <td>http://www.w3.org/2004/02/skos/core#altLabel</td>
</tr>
<tr>
    <td>Foretrukken term</td>
    <td>alternativ term</td>
</tr>
<tr>
    <td>Definition</td>
    <td>En alternativ leksikalsk term for en ressource.</td>
</tr>
<tr>
    <td>Kommentar</td>
    <td>Range for skos:altLabel er klassen af RDF ’plain literals’. <br> skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte egenskaber.</td>
</tr>
<tr>
    <td>Eksempel</td>
    <td>Akronymer, forkortelser, stavevarianter og uregelmæssige flertals-/entalsformer kan inkluderes blandt de alternative betegnelser for et begreb. Fejlstavede termer er normalt inkluderet som skjulte etiketter (se skos:hiddenLabel).</td>
</tr>
<tr>
    <td>Domæne</td>
    <td>rdfs:Resource</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>xsd:string eller rdf:langString (tidligere angivet som rdf:PlainLiteral)</td>
</tr>
<tr>
    <td>Underegenskab af</td>
    <td>rdfs:label</td>
</tr>
</table>

_**Profilens kontekstrestriktioner og annotationer**_ 
<table>
<tr>
    <td>Definition</td>
    <td><span style="color🚙">[fra informationsmodel] <br> et andet navn for organisationen end det alment foretrukne</span></td>
</tr>
<tr>
    <td>Kommentar</td>
    <td><span style="color🚙">[fra informationsmodel] <br> Ofte opstår der alment kendte forkortelser eller alternative navne for organisationer - især hvis det officielle navn er meget langt eller ikke så mundret</span></td>
</tr>
<tr>
    <td>Anvendelsesnote</td>
    <td>Bruges til at angive et accepteret - men ikke foretrukkent - navn for organisationen.></td>
</tr>
<tr>
    <td>Eksempel</td>
    <td>
        <span style="color🚙">[fra informationsmodel] <br> navn: "Digitaliseringsstyrelsen" alternativt navn: "Digst"<br>
        <span style="color🚙">[fra informationsmodel] <br> navn: "Styrelsen for dataforsyning og effektivisering"  <br> alternativtNavn: "SDFE"</span></td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>rdf:langString</td>
</tr>
<tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
</tr>
</table>

**beskrivelse**
_**Vokabular-definition og beskrivelser**_
<table>
<tr>
    <td>URI</td>
    <td>http://purl.org/dc/terms/description</td>
</tr>
<tr>
    <td>Term</td>
    <td>beskrivelse</td>
</tr>
<tr>
    <td>Beskrivelse</td>
    <td>Beskrivelsen kan omfatte, men er ikke begrænset til: et abstrakt, en indholdsfortegnelse, en grafisk repræsentation eller en fritekstberetning af ressourcen.</td>
</tr>
<tr>
    <td>Kommentar</td>
    <td>En redegørelse for ressourcen.</td>
</tr>
<tr>
    <td>Domæne</td>
    <td>rdfs:Resource</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>rdfs:Resource</td>
</tr>
</table>

_**Profilens kontekstrestriktioner og annotationer**_
<table>
<tr>
    <td>Beskrivelse</td>
    <td><span style="color🚙">[fra informationsmodel] <br> letforståelig forklaring på organisationens virke.</span></td>
</tr>
<tr>
    <td>Kommentar</td>
    <td><span style="color🚙">[fra informationsmodel] <br> Beskrivelsen skal gerne formuleres således at den er forståelig af andre end dem, der arbejder i organisationen, da formålet netop er at udenforstående skal kunne få en vis indsigt i organisationens virke og formål.</span></td>
</tr>
<tr>
    <td>Anvendelsesnote</td>
    <td>Bruges til at angive en tekstbaseret beskrivelse af organisationens formål og arbejde</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>rdf:langString</td>
</tr>
<tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
</tr>
</table>


**cvr-nummer**
_**Vokabular-definition og beskrivelser**_
<table>
<tr>
    <td>URI</td>
    <td>https://data.gov.dk/model/core/registered-business/registeredBusinessCode</td>
</tr>
<tr>
    <td>Term</td>
    <td>cvr-nummer</td>
</tr>
<tr>
    <td>Definition</td>
    <td>Unikt nummer der identificerer en juridisk enhed registreret i CVR-registeret.</td>
</tr>
<tr>
    <td>Domæne</td>
    <td>org:FormalOrganization</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>xsd:string</td>
</tr>
<tr>
    <td>Underegenskab af</td>
    <td>dct:identifier</td>
</tr>
</table>

_**Profilens kontekstrestriktioner og annotationer**_
<table>
<tr>
    <td>Definition</td>
    <td><span style="color🚙">[fra informationsmodel (klassen Virksomhed)] <br> En virksomheds forretningsnøgle</span></td>
</tr>
<tr>
    <td>Multiplicitet</td>
    <td>0 - 1</td>
</tr>
</table>


**p-nummer-reference**
_**Vokabular-definition og beskrivelser**_
<table>
<tr>
    <td>URI</td>
    <td>https://data.gov.dk/model/core/registered-business/productionUnitCodeReference</td>
</tr>
<tr>
    <td>Term</td>
    <td>p-nummer-reference</td>
</tr>
<tr>
    <td>Definition</td>
    <td>En repræsentation af et produktionsenhedsnummer, anvendt som reference til produktionsenheden.</td>
</tr>
<tr>
    <td>Anvendelsesnote</td>
    <td>Et ’p-nummer’ identificerer et sted, en lokation hvor en virksomhed har aktivitet. Ofte ses et p-nummer dog tilknyttet direkte til en instans af ’Formel organisation’ eller ’Organisatorisk enhed’, hvilket formelt set ikke er korrekt. For at håndtere denne brug er egenskaben ’p-nummer-reference’ dannet.</td>
</tr>
<tr>
    <td>Domæne</td>
    <td>rdfs:Resource</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>xsd:string</td>
</tr>
</table>


_**Profilens kontekstrestriktioner og annotationer**_	
<table>
<tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
</tr>	
</table>

**myndighedskode**
_**Vokabular-definition og beskrivelser**_
<table width="100%">
<tr>
    <td>URI</td>
    <td>https://data.gov.dk/model/core/organisation/extension/authorityCode</td>
</tr>
<tr>
    <td>Term</td>
    <td>myndighedskode</td>
</tr>
<tr>
    <td>Definition</td>
    <td>Entydig kode for en myndighed</span></td>
</tr>
<tr>
	<td>Definition</td>
        <td><span style="color🚙">[fra informationsmodel (klassen Myndighed)] Entydig kode for en myndighed </span></td>
</tr>
<tr>
    <td>Kommentar</td>
    <td><span style="color🚙">[fra informationsmodel (klassen Myndighed)]</span><br> Myndighedskode er et tre- eller fire-cifret tal, der beskriver en myndighed. Enhver myndighedskode tilhører en bestemt myndighed og refererer til myndigheders data i CPR</td>
</tr>
<tr>
    <td>Anvendelsesnote</td>
    <td>Myndighedskoder kendes også som kommunekoder og regionskoder. Kommunekoder og regionskoder udgør begge delmængder af myndighedskoder.</td>
</tr>
<tr>
    <td>Domæne</td>
    <td>org:FormalOrganization</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>xsd:string</td>
</tr>
<tr>
    <td>Underegenskab af</td>
    <td>dct:identifier</td>
</tr>
<tr>
    <td>Profilens kontekstrestriktioner og annotationer</td>
    <td>Multiplicitet 0 - 1</td>
</tr>
</table>


**EAN**
EAN er ikke en del af informationsmodellen, men er lovpligtig at anvende for offentlige organisationer. EAN foreslås derfor som egenskab på ’Formel organisation’. (rettelse) FLYT TIL KONTAKTINFORMATION

_**Vokabular-definition og beskrivelser**_
<table>
<tr>
    <td>URI</td>
    <td>https://schema.org/globalLocationNumber</td>
</tr>
<tr>
    <td>Term</td>
    <td>globalLocationNumber</td>
</tr>
<tr>
    <td>Kommentar</td>
    <td>
        Global Location Number (GLN, nogle gange også omtalt som International Location Number eller ILN) for den respektive organisation, person eller sted. GLN er et 13-cifret nummer, der bruges til at identificere parter og fysiske lokationer.
    </td>
</tr>
<tr>
    <td>Domæne</td>
    <td>schema:Organization eller schema:Person eller schema:Place</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>xsd:string</td>
</tr>
<tr>
    <td>Underegenskab af</td>
    <td>schema:identifier</td>
</tr>
</table>

_**Profilens kontekstrestriktioner og annotationer**_
<table>
<tr>
    <td>Foretrukken term</td>
    <td>EAN</td>
</tr>
<tr>
    <td>Anvendelsesnote</td>
    <td>EAN-lokationsnummeret er et nummer, der entydigt identificerer den pågældende "indehaver" af nummeret. "EAN" står for "European Article Numbering". Et EAN-nummer er lig med et GLN-nummer (Global Location Number). <br>
Da betegnelsen EAN-nummer er gennemgående på fakturaer, blanketter og i fakturahåndteringssystemer, er denne betegnelse også benyttet i anvendelsesprofilen.</td>
</tr>
<tr>
    <td>Multiplicitet</td>
    <td>0 - 1</td>
</tr>
</table>


## Organisationens historik
 
**oprettelsesdato**

(indsæt billede)

_**Vokabular-definition og beskrivelser**_

<table>
<tr>
    <td>URI</td>
    <td>http://schema.org/foundingDate</td>
</tr>
<tr>
    <td>Term</td>
    <td>grundlæggelsesdato</td>
</tr>
<tr>
    <td>Kommentar</td>
    <td>Den dato, hvor denne organisation blev grundlagt.</td>
</tr>
<tr>
    <td>Domæne (inkluderer)</td>
    <td>schema:Organization</td>
</tr>
<tr>
    <td>Udfaldsrum (inkluderer)</td>
    <td>schema:Date</td>
</tr>
<tr>
    <td>Udfaldsrum (inkluderer)</td>
    <td>schema:Date</td>
</tr>
</table>
	
**Profilens kontekstrestriktioner og annotationer**
<table>
    <tr>
        <td>URI</td>
        <td>http://schema.org/foundingDate</td>
    </tr>
    <tr>
        <td>Term</td>
        <td>grundlæggelsesdato</td>
    </tr>
    <tr>
        <td>Alternativ term</td>
        <td>Oprettelsesdato</td>
    </tr>
    <tr>
        <td>Alternativ term</td>
        <td>oprettelsesdato [fra informationsmodel]</td>
    </tr>
    <tr>
        <td>Definition</td>
        <td>den dato organisationen blev grundlagt eller oprettet [fra informationsmodel]</td>
    </tr>
    <tr>
        <td>Anvendelsesnote</td>
        <td>Bruges til at angive den dato hvorpå organisationen blev oprettet</td>
    </tr>
    <tr>
        <td>Kommentar</td>
        <td>Den dato, hvor denne organisation blev grundlagt.</td>
    </tr>
    <tr>
        <td>Domæne (inkluderer)</td>
        <td>schema:Organization</td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>org:FormalOrganization</td>
    </tr>
    <tr>
        <td>Udfaldsrum (inkluderer)</td>
        <td>schema:Date</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>xsd:date</td>
    </tr>
    <tr>
        <td>Multiplicitet</td>
        <td>0 - 1</td>
    </tr>
</table>

**nedlæggelsesdato**
_**Vokabular-definition og beskrivelser**_
<table>
    <tr>
        <td>URI</td>
        <td>http://schema.org/dissolutionDate</td>
    </tr>
    <tr>
        <td>Term</td>
        <td>nedlæggelsesdato</td>
    </tr>
    <tr>
        <td>Kommentar</td>
        <td>dato, hvor denne organisation blev opløst.</td>
    </tr>
    <tr>
        <td>Domæne (inkluderer)</td>
        <td>schema:Organization</td>
    </tr>
    <tr>
        <td>Udfaldsrum (inkluderer)</td>
        <td>schema:Date</td>
    </tr>
    <tr>
        <td>Alternativ term</td>
        <td>Opløsningsdato</td>
    </tr>
    <tr>
        <td>Alternativ term</td>
        <td>ophørsdato, nedlæggelsesdato [fra informationsmodel]</td>
    </tr>
    <tr>
        <td>Definition</td>
        <td>Den dato organisationen ophører med at eksistere [fra informationsmodel]</td>
    </tr>
    <tr>
        <td>Kommentar</td>
        <td>Organisationen kan ikke ophøre med at eksistere så længe der er aktive Organisationsenheder eller -medlemmer i den. [fra informationsmodel]</td>
    </tr>
    <tr>
        <td>Anvendelsesnote</td>
        <td>Bruges til at angive den dato hvorpå organisationen blev nedlagt</td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>org:FormalOrganization</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>xsd:date</td>
    </tr>
    <tr>
        <td>Multiplicitet</td>
        <td>0 - 1</td>
    </tr>
</table>


## Typer af formelle organisationer

(indsæt billede)

#### **klassifikation**
##### _**Vokabular-definition og beskrivelser**_
<table>
    <tr>
        <td>URI</td>
        <td>http://www.w3.org/ns/org#classification</td>
    </tr>
    <tr>
        <td>Term</td>
        <td>klassifikation</td>
    </tr>
    <tr>
        <td>Kommentar</td>
        <td>Angiver en klassifikation for denne organisation inden for et eller andet klassifikationssystem. Bemærk, at det også er tilladt for applikationer at definere underklasser af org:Organisation som et middel til at repræsentere organisatoriske kategorier.</td>
    </tr>
    <tr>
        <td>Anvendelsesnote</td>
        <td>Udbyggende vokabularer ønsker måske at specialisere denne egenskab til at have et område svarende til et specifikt skos:ConceptScheme</td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>org:Organization</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>skos:Concept</td>
    </tr>
</table>


_**Profilens kontekstrestriktioner og annotationer**_ 
Definition	[fra informationsmodel (klassen Myndighed)]
Type af myndighed  
Kommentar	[fra informationsmodel]
Typer af myndighed:
00 = ukendt myndighed
04 = personregisterfører
05 = kommuner
07 = fiktive kommuner (f.eks. ATP)
10 = domstole
14 = valgkontoret
15 = statsforvaltninger m.fl.
16 = justitsministeriet
17 = indfødsretskontoret
18 = udlændingeservice
20 = anerkendte trossamfund
25 = sogne
30 = lande
35 = politi
39 = CPR kontoret (kongelige)
40 = regioner (sygehuse)
41 = borgere (flytning via venteregisteret)
42 = borgere (flytning direkte)
43 = udtrækskunder
45 = skattecentre
50 = IT-leverandører samt FORPAS
55 = værnepligtsregistrerende myndighed
70 = ministerier
71 = kirkeministeriet
75 = landsdel
80 = stifter
85 = provstier
98 = øvre kommune, København 102
99 = maskinel myndighedskode
Domæne	org:FormalOrganization
Udfaldsrum	ovx:FormalOrganizationType
Multiplicitet	0 - *

### Type af formel organisation (klasse)
[Vi bør nok også anvende en underklasse af ConceptScheme til at indholde det samlede udvalg af organisationstyper. Vi bør måske kunne inddrage decentrale organisationsklassifikationer]
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/organisation/extension/FormalOrganizationType 

Term	Type af formel organisation
Definition	Klassifikation af organisationstyper
Beskrivelse	[Fyld ind her]
Eksempel	Typer af organisationer:
Offentlig myndighed
	Kommune
	Region
	Statslig myndighed
		Folketinget
		Ministerie
		Styrelse
Offentligretligt organ
Virksomhed
Interesseorganisation
Politisk parti
Underklasse af	skos:Concept
Profilens kontekstrestriktioner og annotationer 
Anvendelsesnote	[Fyld ind her]

foretrukken betegnelse
Vokabular-definition og beskrivelser
URI	http://www.w3.org/2004/02/skos/core#prefLabel

Term	foretrukken term
Definition	Den foretrukne leksikalske betegnelse for en ressource på et givet sprog.
Kommentar	En ressource har ikke mere end én værdi af skos:prefLabel pr. sprogtag.
Range for skos:prefLabel er klassen af RDF ’plain literals’.
skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte egenskaber.
Domæne	rdfs:Resource
Udfaldsrum	xsd:string eller rdf:langString (tidligere angivet som rdf:PlainLiteral)

Underegenskab af	rdfs:label
Profilens kontekstrestriktioner og annotationer 
Domæne	ovx:FormalOrganizationType
Udfaldsrum	rdf:langString

Multiplicitet	1 - *

alternativ betegnelse
Vokabular-definition og beskrivelser
URI	http://www.w3.org/2004/02/skos/core#altLabel 

Foretrukken term	alternativ term
Definition	En alternativ leksikalsk term for en ressource.
Kommentar	Range for skos:altLabel er klassen af RDF ’plain literals’.
skos:prefLabel, skos:altLabel og skos:hiddenLabel er parvis disjunkte egenskaber.
Eksempel	Akronymer, forkortelser, stavevarianter og uregelmæssige flertals-/entalsformer kan inkluderes blandt de alternative betegnelser for et begreb. Fejlstavede termer er normalt inkluderet som skjulte etiketter (se skos:hiddenLabel).
Domæne	rdfs:Resource
Udfaldsrum	xsd:string eller rdf:langString (tidligere angivet som rdf:PlainLiteral)

Underegenskab af	rdfs:label
Profilens kontekstrestriktioner og annotationer 
Domæne	ovx:FormalOrganizationType
Udfaldsrum	rdf:langString
Multiplicitet	0 - *

definition
Vokabular-definition og beskrivelser
URI	http://www.w3.org/2004/02/skos/core#definition

Term	definition
Definition	En erklæring eller formel forklaring af betydningen af et begreb.
Domæne	rdfs:Resource
Udfaldsrum	rdfs:Resource
Underegenskab af	skos:note
Profilens kontekstrestriktioner og annotationer 
Domæne	ovx:FormalOrganizationType
Udfaldsrum	rdf:langString
Multiplicitet	0 - *

har bredere
Vokabular-definition og beskrivelser
URI	http://www.w3.org/2004/02/skos/core#broader

Term	har bredere
Definition	Relaterer et begreb til et begreb, der har en mere generel betydning
Kommentar	Efter konvention bruges skos:broader kun til at erklære en umiddelbar (dvs. direkte) hierarkisk forbindelse mellem to konceptuelle ressourcer.
Domæne	rdfs:Resource
Udfaldsrum	rdfs:Resource
Underegenskab af	skos:broaderTransitive
Modsatrettet egenskab	skos:narrower
Profilens kontekstrestriktioner og annotationer 
Domæne	ovx:FormalOrganizationType
Udfaldsrum	ovx:FormalOrganizationType
Multiplicitet	0 - 1

har smallere
Vokabular-definition og beskrivelser
URI	http://www.w3.org/2004/02/skos/core#narrower

Term	har smallere
Definition	Relaterer et begreb til et begreb, der er mere specifikt i betydning
Domæne	rdfs:Resource
Udfaldsrum	rdfs:Resource
Underegenskab af	skos:narrowerTransitive
Modsatrettet egenskab	skos:broader
Profilens kontekstrestriktioner og annotationer 
Domæne	ovx:FormalOrganizationType
Udfaldsrum	ovx:FormalOrganizationType
Multiplicitet	0 - *

 

