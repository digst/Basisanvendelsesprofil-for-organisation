# Den formelle organisations egenskaber

<p align="center">
  <img  alt="Model over den formelle organisations egenskaber" src="PNG/Den-formelle-organisations-egenskaber.png">
</p>

## Organisationens identifikation og beskrivelse

<p align="center">
  <img  alt="Model over formel organisation identifikation og beskrivels" src="PNG/Formel-organisation-identifikation-og-beskrivelse.png">
</p>

#### foretrukken term
##### _Vokabular-definition og beskrivelser_
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

##### _Profilens kontekstrestriktioner og annotationer_ 
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
    <td>[fra informationsmodel] <ul> <li>"Digitaliseringsstyrelsen"</li> <li>"Næstved Sygehus"</li> <li>"Holbæk kommune"</li> <li>"FDF-spejderne i Vejle"</li></ul>
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

#### alternativ term
##### _Vokabular-definition og beskrivelser_
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

##### _Profilens kontekstrestriktioner og annotationer_ 
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
        [fra informationsmodel] </br>
	navn: "Digitaliseringsstyrelsen" </br> alternativt navn: "Digst" </br>
        navn: "Styrelsen for dataforsyning og effektivisering"  </br> alternativtNavn: "SDFE"
	</td>
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

#### beskrivelse
##### _Vokabular-definition og beskrivelser_
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

##### _Profilens kontekstrestriktioner og annotationer_
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

#### cvr-nummer
##### _Vokabular-definition og beskrivelser_
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

##### _Profilens kontekstrestriktioner og annotationer_
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


#### p-nummer-reference
##### _Vokabular-definition og beskrivelser_
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


##### _Profilens kontekstrestriktioner og annotationer_	
<table>
<tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
</tr>	
</table>

#### myndighedskode
##### _Vokabular-definition og beskrivelser_
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
        <td>[fra informationsmodel (klassen Myndighed)] Entydig kode for en myndighed </td>
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

</table>


##### _Profilens kontekstrestriktioner og annotationer_
<table>
<tr>
    <td>Domæne</td>
    <td>org:FormalOrganization</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>xsd:string</td>
</tr>
<tr>
    <td>Multiplicitet</td>
    <td> 0 - 1</td>
</tr>
</table>
 
#### EAN
EAN er ikke en del af informationsmodellen, men er lovpligtig at anvende for offentlige organisationer. EAN foreslås derfor som egenskab på ’Formel organisation’. (rettelse) FLYT TIL KONTAKTINFORMATION

##### _Vokabular-definition og beskrivelser_
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

##### _Profilens kontekstrestriktioner og annotationer_
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

<p align="center">
  <img  alt="Model over organisationens historie" src="PNG/Organisationens-historie.png">
</p>

#### oprettelsesdato

##### _Vokabular-definition og beskrivelser_

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
    <td>Domæne</td>
    <td>schema:Organization</td>
</tr>
<tr>
    <td>Udfaldsrum</td>
    <td>schema:Date</td>
</tr>
</table>
	
##### _Profilens kontekstrestriktioner og annotationer_
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

#### nedlæggelsesdato
##### _Vokabular-definition og beskrivelser_
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
        <td>Domæne</td>
        <td>schema:Organization</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>schema:Date</td>
    </tr>
</table>

##### _Profilens kontekstrestriktioner og annotationer_
<table>
 <tr>
        <td>Alternativ term</td>
        <td>Opløsningsdato</td>
    </tr>
    <tr>
        <td>Alternativ term</td>
        <td>[fra informationsmodel]</br>ophørsdato</td>
    </tr>
    <tr>
        <td>Definition</td>
        <td>[fra informationsmodel]</br>Den dato organisationen ophører med at eksistere.</td>
    </tr>
    <tr>
        <td>Kommentar</td>
        <td>[fra informationsmodel]</br>Organisationen kan ikke ophøre med at eksistere så længe der er aktive Organisationsenheder eller -medlemmer i den.</td>
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

![Model over typer af organisatorisk enhed](PNG/Type-af-organisatorisk-enhed.png)

#### klassifikation
##### _Vokabular-definition og beskrivelser_
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


##### _Profilens kontekstrestriktioner og annotationer_ 

<table>
    <tr>
        <td>Definition</td>
        <td>[fra informationsmodel (klassen Myndighed)]</br>
Type af myndighed </td>
    </tr>
    <tr>
        <td>Kommentar</td>
        <td>[fra informationsmodel] </br> 
Typer af myndighed:</br>
00 = ukendt myndighed</br>
04 = personregisterfører</br>
05 = kommuner</br>
07 = fiktive kommuner (f.eks. ATP)</br>
10 = domstole</br>
14 = valgkontoret</br>
15 = statsforvaltninger m.fl.</br>
16 = justitsministeriet</br>
17 = indfødsretskontoret</br>
18 = udlændingeservice</br>
20 = anerkendte trossamfund</br>
25 = sogne</br>
30 = lande</br>
35 = politi</br>
39 = CPR kontoret (kongelige)</br>
40 = regioner (sygehuse)</br>
41 = borgere (flytning via venteregisteret)</br>
42 = borgere (flytning direkte)</br>
43 = udtrækskunder</br>
45 = skattecentre</br>
50 = IT-leverandører samt FORPAS</br>
55 = værnepligtsregistrerende myndighed</br>
70 = ministerier</br>
71 = kirkeministeriet</br>
75 = landsdel</br>
80 = stifter</br>
85 = provstier</br>
98 = øvre kommune, København 102</br>
99 = maskinel myndighedskode
</td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>org:FormalOrganization</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>ovx:FormalOrganizationType</td>
    </tr>
    <tr>
        <td>Multiplicitet</td>
        <td>0 - *</td>
    </tr>
</table>


### Type af formel organisation (klasse)
[Vi bør nok også anvende en underklasse af ConceptScheme til at indholde det samlede udvalg af organisationstyper. Vi bør måske kunne inddrage decentrale organisationsklassifikationer] (farve, gul farve her)

##### _Vokabular-definition og beskrivelser_
<table>
    <tr>
        <td>URI</td>
        <td>https://data.gov.dk/model/core/organisation/extension/FormalOrganizationType</td>
    </tr>
    <tr>
        <td>Term</td>
        <td>Type af formel organisation</td>
    </tr>
    <tr>
        <td>Definition</td>
        <td>Klassifikation af organisationstyper</td>
    </tr>
    <tr>
        <td>Beskrivelse</td>
        <td>[Fyld ind her]</td>
    </tr>
    <tr>
        <td>Eksempel</td>
        <td>
            Typer af organisationer:<br>
            - Offentlig myndighed<br>
            &nbsp;&nbsp;- Kommune<br>
            &nbsp;&nbsp;- Region<br>
            &nbsp;&nbsp;- Statslig myndighed<br>
            &nbsp;&nbsp;&nbsp;&nbsp;- Folketinget<br>
            &nbsp;&nbsp;&nbsp;&nbsp;- Ministerie<br>
            &nbsp;&nbsp;&nbsp;&nbsp;- Styrelse<br>
            - Offentligretligt organ<br>
            - Virksomhed<br>
            - Interesseorganisation<br>
            - Politisk parti
        </td>
    </tr>
    <tr>
        <td>Underklasse af</td>
        <td>skos:Concept</td>
    </tr>
</table>

##### _Profilens kontekstrestriktioner og annotationer_
<table>
	<tr>
		<td>Anvendelsesnote</td>
		<td>[Fyld ind her]</td>
	</tr>
</table>

#### **foretrukken betegnelse**
##### _**Vokabular-definition og beskrivelser**_
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
        <td>En ressource har ikke mere end én værdi af skos:prefLabel pr. sprogtag. Range for skos:prefLabel er klassen af RDF ’plain literals’. skos:prefLabel, skos:altLabel, og skos:hiddenLabel er parvis disjunkte egenskaber.</td>
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

##### _Profilens kontekstrestriktioner og annotationer_
<table>
    <tr>
     <td>Domæne</td>
    <td>ovx:FormalOrganizationType</td>
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

#### alternativ betegnelse
##### _Vokabular-definition og beskrivelser_
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
        <td>Range for skos:altLabel er klassen af RDF ’plain literals’. skos:prefLabel, skos:altLabel, og skos:hiddenLabel er parvis disjunkte egenskaber. Akronymer, forkortelser, stavevarianter og uregelmæssige flertals-/entalsformer kan inkluderes blandt de alternative betegnelser for et begreb. Fejlstavede termer er normalt inkluderet som skjulte etiketter (se skos:hiddenLabel).</td>
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

##### _Profilens kontekstrestriktioner og annotationer_
<table>
    <tr>
        <td>Domæne</td>
        <td>ovx:FormalOrganizationType</td>
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

#### definition
##### _Vokabular-definition og beskrivelser_
<table>
    <tr>
        <td>URI</td>
        <td>http://www.w3.org/2004/02/skos/core#definition</td>
    </tr>
    <tr>
        <td>Term</td>
        <td>definition</td>
    </tr>
    <tr>
        <td>Definition</td>
        <td>En erklæring eller formel forklaring af betydningen af et begreb.</td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>rdfs:Resource</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>rdfs:Resource</td>
    </tr>
    <tr>
        <td>Underegenskab af</td>
        <td>skos:note</td>
    </tr>
    <tr>
        <td>Profilens kontekstrestriktioner og annotationer</td>
        <td></td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>ovx:FormalOrganizationType</td>
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

#### har bredere
##### _Vokabular-definition og beskrivelser_
<table>
    <tr>
        <td>URI</td>
        <td>http://www.w3.org/2004/02/skos/core#broader</td>
    </tr>
    <tr>
        <td>Term</td>
        <td>har bredere</td>
    </tr>
    <tr>
        <td>Definition</td>
        <td>Relaterer et begreb til et begreb, der har en mere generel betydning</td>
    </tr>
    <tr>
        <td>Kommentar</td>
        <td>Efter konvention bruges skos:broader kun til at erklære en umiddelbar (dvs. direkte) hierarkisk forbindelse mellem to konceptuelle ressourcer.</td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>rdfs:Resource</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>rdfs:Resource</td>
    </tr>
    <tr>
        <td>Underegenskab af</td>
        <td>skos:broaderTransitive</td>
    </tr>
    <tr>
        <td>Modsatrettet egenskab</td>
        <td>skos:narrower</td>
    </tr>
    <tr>
        <td>Profilens kontekstrestriktioner og annotationer</td>
        <td></td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>ovx:FormalOrganizationType</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>ovx:FormalOrganizationType</td>
    </tr>
    <tr>
        <td>Multiplicitet</td>
        <td>0 - 1</td>
    </tr>
</table>

#### har smallere
##### _Vokabular-definition og beskrivelser_
<table>
    <tr>
        <td>URI</td>
        <td>http://www.w3.org/2004/02/skos/core#narrower</td>
    </tr>
    <tr>
        <td>Term</td>
        <td>har smallere</td>
    </tr>
    <tr>
        <td>Definition</td>
        <td>Relaterer et begreb til et begreb, der er mere specifikt i betydning</td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>rdfs:Resource</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>rdfs:Resource</td>
    </tr>
    <tr>
        <td>Underegenskab af</td>
        <td>skos:narrowerTransitive</td>
    </tr>
    <tr>
        <td>Modsatrettet egenskab</td>
        <td>skos:broader</td>
    </tr>
    <tr>
        <td>Profilens kontekstrestriktioner og annotationer</td>
        <td></td>
    </tr>
    <tr>
        <td>Domæne</td>
        <td>ovx:FormalOrganizationType</td>
    </tr>
    <tr>
        <td>Udfaldsrum</td>
        <td>ovx:FormalOrganizationType</td>
    </tr>
    <tr>
        <td>Multiplicitet</td>
        <td>0 - *</td>
    </tr>
</table>


 

