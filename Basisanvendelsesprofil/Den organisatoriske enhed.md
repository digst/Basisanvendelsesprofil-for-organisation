# Den organisatoriske enhed

(indsæt billede)
 
## Den organisatoriske enheds identifikation og beskrivelse
 
#### intern identifikation
##### _Vokabular-definition og beskrivelser_
URI	http://purl.org/dc/terms/identifier
Term	identifikator
Beskrivelse	Anbefalet bedste praksis er at identificere ressourcen ved hjælp af en streng, der er i overensstemmelse med et formelt identifikationssystem.
Kommentar	En entydig reference til ressourcen inden for en given kontekst.
Eksempel	Eksempler omfatter International Standard Book Number (ISBN), Digital Object Identifier (DOI) og Uniform Resource Name (URN). Stabile identifikatorer bør angives som HTTP-URI'er.
Domæne	rdfs:Resource
Udfaldsrum	rdfs:Literal
Profilens kontekstrestriktioner og annotationer 
Definition	[fra informationsmodel]
Den centrale, brugervendte nøgle for organisationsenheden
Kommentar	[fra informationsmodel]
anvendes eksempelvis i sundhedssektoren, hvor alle afdelinger er angivet efter et nummersystem.
Den brugervendte nøgle kan skifte over tid, hvis er kommer nye nummer-/nøglesystemer.
Domæne	org:OrganizationalUnit
Udfaldsrum	xsd:string
Multiplicitet	1 - 1

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
Alternativ term	[fra informationsmodel]
afdelingsnavn
Definition	[fra informationsmodel]
alment anvendt navn for en organisationsenhed
Kommentar	[fra informationsmodel]
Organisationsenheders navn tildeles af organisationen
Anvendelsesnote	Bruges til at angive den organisatoriske enheds primære navn.
Eksempel	[fra informationsmodel]
o	"Bogholderiet"
o	Projekt "ny organisationsstandard"
o	"Hæmatologisk afdeling"
- ...
Domæne	org:OrganizationalUnit
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
Definition	[fra informationsmodel]
et andet navn for organisationsenheden end det alment foretrukne
Kommentar	[fra informationsmodel]
Ofte opstår der alment kendte forkortelser eller alternative navne for organisationsenheder - især hvis det officielle navn er meget langt eller ikke så mundret.
Anvendelsesnote	Bruges til at angive et accepteret - men ikke foretrukket - navn for den organisatoriske enhed.
Eksempel	[fra informationsmodel]
navn: "Digitalisering og Arkitektur"
alternavtivt navn: "DIA"
navn: EKSEMPEL SØGES
Udfaldsrum	rdf:langString
Multiplicitet	0 - *

p-nummer-reference
Et ’p-nummer’ identificerer et sted, en lokation hvor en virksomhed har aktivitet. Ofte ses et p-nummer dog tilknyttet direkte til en instans af ’Formel organisation’ eller ’Organisatorisk enhed’, hvilket formelt set ikke er korrekt. For at håndtere denne brug er egenskaben ’p-nummer-reference’ dannet.
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/registered-business/productionUnitCodeReference
Term	p-nummer-reference
Definition	En repræsentation af et produktionsenhedsnummer, anvendt som reference til produktionsenheden
Domæne	rdfs:Resource
Udfaldsrum	xsd:string
Profilens kontekstrestriktioner og annotationer 
Domæne	org:OrganizationalUnit
Udfaldsrum	xsd:string
Multiplicitet	0 - *

Historik for den organisatoriske enhed
 
oprettelsesdato
Vokabular-definition og beskrivelser
URI	http://schema.org/foundingDate

Term	grundlæggelsesdato  
Alternativ term	oprettelsesdato
Kommentar	den dato organisationen blev oprettet
Domæne	schema:Organization
Udfaldsrum	schema:Date
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel]
den dato organisationsenheden blev oprettet
Anvendelsesnote	I schema.org anvendes termen ’organisation’ bredt og dækker også over ’organisatorisk enhed’. Anvendt i denne sammenhæng angiver egenskaben den dato hvorpå den organisatoriske enhed blev oprettet.
Domæne	org:OrganizationalUnit
Udfaldsrum	xsd:date
Multiplicitet	0 - 1

nedlæggelsesdato
Vokabular-definition og beskrivelser
URI	http://schema.org/dissolutionDate

Term	nedlæggelsesdato
Kommentar	den dato organisationen blev nedlagt
Domæne	schema:Organization
Udfaldsrum	schema:Date
Profil-restriktioner og annotationer 
Alternativ term	opløsningsdato
Definition	[fra informationsmodel]
Den dato organisationsenheden bliver nedlagt
Kommentar	[fra informationsmodel]
nedlæggelsesdatoen skal være lig med eller senere end oprettelsesdatoen
Anvendelsesnote	I schema.org anvendes termen ’organisation’ bredt og dækker også over ’organisatorisk enhed’. Anvendt i denne sammenhæng angiver den dato hvorpå den organisatoriske enhed blev nedlagt.
Domæne	org:OrganizationalUnit
Udfaldsrum	xsd:date
Multiplicitet	0 - 1

Typer af organisatoriske enheder
 
klassifikation
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/org#classification

Term	klassifikation
Kommentar	Angiver en klassifikation for denne Organisation inden for et klassifikationsskema. Udvidelsesvokabularer ønsker måske at specialisere denne egenskab til at have et område svarende til et specifikt `skos:ConceptScheme`. Denne egenskab er under diskussion og kan blive revideret eller fjernet - i mange tilfælde kategoriseres organisationer bedst ved at definere et underklassehierarki i et udvidelsesordforråd.
Domæne	org:Organization
Udfaldsrum	skos:Concept
Profil-restriktioner og annotationer 
Definition	Angiver en klassifikation for denne [organisatoriske enhed] inden for et eller andet klassifikationssystem..
Definition	[fra informationsmodel]
beskriver den slags organisationsenhed der er tale om
Kommentar	[fra informationsmodel]
Kan anvendes til at imødekomme forskellige forretningsregler, som retter sig mod typen af Organisationsenhed
Eksempel	[fra informationsmodel]
SOR-enhedstyper:
- klinisk-administrativt niveau
- økonomi
- ...
Domæne	org:OrganizationalUnit
Udfaldsrum	ovx:OrganizationalUnitType
Multiplicitet	0 - *

Organisatorisk enhedstype (klasse)
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/organisation/extension/-OrganizationalUnitType
Term	Organisatoriske enhedstype
Definition	Klassifikation af organisationstyper.
Eksempel	Typer af organisatoriske enheder:
Afdeling
Kontor
Team
Underklasse af	skos:Concept
Profilens kontekstrestriktioner og annotationer 

foretrukken term
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
Anvendelsesnote	Bruges til at angive den organisatoriske enheds foretrukne navn. Det antages at organisationer selv er ophav til enhedens navn. Navnet kan angives på flere sprog og dermed give flere forekomster af egenskaben skos:prefLabel for den enkelte organisation.
Udfaldsrum	rdf:langString
Multiplicitet	1 - *

alternativ term
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
Anvendelsesnote	Bruges til at angive et accepteret - men ikke foretrukkent - navn for den organisatoriske enhed.
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
Domæne	ovx:OrganizationalUnitType
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
Domæne	ovx:OrganizationalUnitType
Udfaldsrum	ovx:OrganizationalUnitType
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
Domæne	ovx:OrganizationalUnitType
Udfaldsrum	ovx:OrganizationalUnitType
Multiplicitet	0 - *

 
Kontaktoplysninger
En organisation kan kontaktes af eksterne på forskellige måder. Kontakten kan ske ved ved personligt fremmøde til en besøgsadresse eller ved at sende post til postadresse. Kontakten kan også foretages via telefon, fax, e-mail eller en dedikeret webside. 
I basisprofilen er alle de nævnte kontaktformer repræsenteret både i relation til den formelle organisation og i relation til organisatoriske enheder. Kontaktformerne er både repræsenteret som direkte tilknyttet en organisation eller en organisatoriske enhed, samt – hvor der er behov for det – tilknyttet som mere kvalificeret information. Kvalificeret information betyder i denne sammenhæng at der til kontaktformen, eksempelvis et telefonnummer, tilføjes data der giver mere information, eksempelvis hvilke tidspunkter der kan ringes på.
Både direkte tilknyttet kontaktinformation og kvalificeret kontaktinformation beskrives efterfølgende.

 

Direkte relateret kontaktinformation
 
telefon
Vokabular-definition og beskrivelser
URI	http://schema.org/telephone

Term	telefon
Kommentar	Telefonnummeret
Domæne	schema:Organization  eller schema:Person  eller schema:ContactPoint  eller schema:Place
Udfaldsrum	schema:Text  eller schema:URL  eller schema:Role
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel (klassen Myndighed)]
Telefonummer til myndighed
Definition	[fra informationsmodel (klassen Telefon]
telefonnummer som tilhører et bestemt abonnement
Beskrivelse	Et telefonnummer er en talkode bestående af et antal cifre, der identificerer et telefonabonnement eller en teletjeneste. Nummeret bruges til at kontakte abonnenten eller tjenesten.
Domæne	org:FormalOrganization eller org:OrganizationalUnit 
Udfaldsrum	xsd:string
Multiplicitet	0 - *

e-mail
Vokabular-definition og beskrivelser
URI	http://schema.org/email

Term	e-mail
Kommentar	E-mail adresse
Domæne	schema:Organization  eller schema:Person  eller schema:ContactPoint
Udfaldsrum	schema:Text eller schema:URL eller schema:Role
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel (klassen Myndighed)]
Elektronisk kontaktadresse på myndighed
Definition	[fra informationsmodel (klassen Mail)]
adresse der identificerer en elektronisk postkasse til hvilken meddelelser kan leveres
Kommentar	[fra informationsmodel (klassen Mail)]
opbygget af et brugernavn og et servernavn adskilt af @
Domæne	org:FormalOrganization eller org:OrganizationalUnit
Udfaldsrum	xsd:string
Multiplicitet	0 - *

faxnummer
Vokabular-definition og beskrivelser
URI	http://schema.org/faxNumber

Term	faxnummer
Kommentar	Fax-nummeret
Domæne	schema:Place eller schema:Organization eller schema:Person eller schema:ContactPoint
Udfaldsrum	schema:Text eller schema:URL eller schema:Role
Profil-restriktioner og annotationer 
Domæne	org:FormalOrganization eller org:OrganizationalUnit
Udfaldsrum	xsd:string
Multiplicitet	0 - *

webside
Vokabular-definition og beskrivelser
URI	http://xmlns.com/foaf/0.1/page

Term	side
Kommentar	En side eller et dokument om denne ting
Udfaldsrum	foaf:Document
Profil-restriktioner og annotationer 
Term	webside
Definition	[fra informationsmodel (klassen VirtuelLokation]
HTML-weblink til at tilgå den virtuelle lokation
Multiplicitet	0 - *

Dokument (klasse)
Vokabular-definition og beskrivelser
URI	http://xmlns.com/foaf/0.1/Document

Term	Dokument
Kommentar	Et dokument
Profil-restriktioner og annotationer 
Kommentar	Document-klassen repræsenterer de ting, der, bredt opfattet, er 'dokumenter'

Kontaktformen adresse beskrives I kapitlet ‘Lokation og adresse’.
Kvalificeret kontaktinformation
 
Kvalificeret kontaktinformation (klasse)
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/organisation/extension/-QualifiedContactInformation

Term	kvalificeret kontaktinformation
Definition	Information om kontaktmetode samt hvilke muligheder og begrænsninger der er ved brug af den pågældende kontaktmetode.
Profilens kontekstrestriktioner og annotationer 
Alternativ term	[fra informationsmodel (klassen Kontaktinformation)]
kontaktpunkt
Definition	[fra informationsmodel (klassen Kontaktinformation)]
Beskriver de forskellige kontaktformer, der er tilgængelige for Organisationer, Organisationsenheder og Organisationsmedlemmer
Kommentar	[fra informationsmodel (klassen Kontaktinformation)]
Kan omhandle fysiske steder som adresser, lokaler, men også virtuelle som sociale medier, email, DigitalPost mv.
Eksempel	[fra informationsmodel (klassen Kontaktinformation)]
- fysisk adresse
- elektronisk adresse
- email
....

værdi
Vokabular-definition og beskrivelser
URI	http://www.w3.org/1999/02/22-rdf-syntax-ns#value

Term	værdi
Kommentar	Idiomatisk egenskab brugt til strukturerede værdier.
Domæne	rdfs:Resource
Udfaldsrum	rdfs:Resource
Profil-restriktioner og annotationer 
Anvendelsesnote	Værdien eller indholdet af den specifikke kontaktform.
Eksempel	Hvis det valgte emne fra ’ovx:ContactForm’ er valgt til ’Telefon’ kan værdien være ’12 34 56 78’.
Domæne	ovx:QualifiedContactInformation
Udfaldsrum	rdfs:Literal
Multiplicitet	1 - 1

kontaktemne
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/organisation/extension/contactSubject

Term	kontaktemne
Definition	Emne kontaktfmetoden er velegnet til at få information om eller på anden måde få håndteret.
Profil-restriktioner og annotationer 
Udfaldsrum	rdf:langString
Multiplicitet	0 - *

bemærkning
Vokabular-definition og beskrivelser
URI	http://www.w3.org/1999/02/22-rdf-syntax-ns#comment

Term	kommentar
Kommentar	En beskrivelse af subjekt ressourcen.
Profil-restriktioner og annotationer 
Term	bemærkning 
Definition	[fra informationsmodel (klassen Kontaktinformation)]
beskriver supplerende forhold omkring den enkelte type af kontakt
Definition	[fra informationsmodel (klassen Kontaktinformation)]
anvendes til at beskrive regler og principper for anvendelse af den enkelte kontaktform
Kommentar	[fra informationsmodel (klassen Kontaktinformation)]
Giver mulighed for at angive særlige forhold, afvigelser eller andet relevant information der knytter sig til den enkelte kontakttype.
Kommentar	[fra informationsmodel (klassen Kontaktinformation)]
Der kan være regler/principper som gælder for samtlige kontakttyper, men der kan også være særlige politikker der kun gør sig gældende i forhold til en specifik kontakttype..
Anvendelsesnote	Bemærkninger vedrørende kontaktinformationen
Eksempel	[fra informationsmodel (klassen Kontaktinformation)]
Benyt indgangen i parkeringskælderen
Eksempel	[fra informationsmodel (klassen Kontaktinformation)]
- email besvares inden for 5 hverdage.
Udfaldsrum	rdf:langString
Multiplicitet	0 - *

type
Vokabular-definition og beskrivelser
URI	http://purl.org/dc/terms/type

Term	type
Beskrivelse	Anbefalet bedste praksis er at bruge et kontrolleret ordforråd, såsom DCMI Type Vocabulary [DCMITYPE]. For at beskrive ressourcens filformat, fysiske medium eller dimensioner skal du bruge Format-elementet.
Kommentar	Ressourcens art eller genre.
Domæne	rdfs:Resource
Udfaldsrum	rdfs:Class
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel (klassen Kontaktinformation)]
anvendes til at klassificere de forskellige typer af kontaktpunkter
Kommentar	[fra informationsmodel (klassen Kontaktinformation)]
omhandler fx fysiske steder som adresser, lokaler, men også virtuelle som sociale medier, email, DigitalPost mv.
Anvendelsesnote	Udpeger typen af kontaktform
Eksempel	[fra informationsmodel (klassen Kontaktinformation)]
- hovedtelefonnummer
- emailadresse
- digitalPostadresse
- vareindlevering
- besøgsadresse
- fakturaadresse-EAN
- fakturaadresse-post
- ...
Domæne	ovx:QualifiedContactInformation
Udfaldsrum	ovx:ContactForm
Multiplicitet	1 - 1


adgangsrettighed
Vokabular-definition og beskrivelser
URI	http://purl.org/dc/terms/accessRights
Term	adgangsrettighed
Beskrivelse	Adgangsrettigheder kan omfatte oplysninger om adgang eller begrænsninger baseret på privatliv, sikkerhed eller andre politikker.
Kommentar	Oplysninger om, hvem der kan få adgang til ressourcen eller en indikation af dens sikkerhedsstatus.
Udfaldsrum	dct:RightsStatement
Underegenskab af	dct:rights
Profil-restriktioner og annotationer 

Adgangsrettighed (klasse)
Autoritetstabellen for adgangsrettigheder er et kontrolleret ordforråd, der viser adgangsrettigheder eller begrænsninger til ressourcer. Det er designet til, men ikke begrænset til, DCAT-beskrivelser af datasæt. Denne myndighedstabel vedligeholdes af Publications Office of the European Union på EU Vocabularies-webstedet.
http://publications.europa.eu/resource/authority/access-right 
Vokabular-definition og beskrivelser
URI	http://purl.org/dc/terms/RightsStatement
Term	Rettighedserklæring
Kommentar	En erklæring om de intellektuelle ejendomsrettigheder (IPR) i eller over en ressource, et juridisk dokument, der giver officiel tilladelse til at gøre noget med en ressource, eller en erklæring om adgangsrettigheder.
Profil-restriktioner og annotationer 

Kontaktform (klasse)
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/organisation/extension/ContactForm

Term	Kontaktform
Definition	Klassifikation indeholdende mulige kontaktformer.
Eksempel	Typer kan være:
Adresse
	Besøgsadresse
	Postadresse
	Aktivitetsadresse
	Vareindlevering
E-mail
	Forretningsmail
	Privat mail
Faxnummer
Telefon
Webside
Underklasse af	skos:Concept
Profilens kontekstrestriktioner og annotationer 
Definition	[fra informationsmodel (klassen Kontaktinformation)]
anvendes til at klassificere de forskellige typer af kontaktpunkter
Kommentar	[fra informationsmodel (klassen Kontaktinformation)]
omhandler fx fysiske steder som adresser, lokaler, men også virtuelle som sociale medier, email, DigitalPost mv.
Eksempel	[fra informationsmodel (klassen Kontaktinformation)]
- hovedtelefonnummer
- emailadresse
- digitalPostadresse
- vareindlevering
- besøgsadresse
- fakturaadresse-EAN
- fakturaadresse-post
- ...

timer tilgængelige
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/organisation/extension/hoursAvailable

Term	timer tilgængelige
Definition	Anvendes til at beskrive åbningstider for kontaktformen
Domæne	ovx:QualifiedContactInformation
Udfaldsrum	schema:OpeningHoursSpecification
Profil-restriktioner og annotationer 
Multiplicitet	0 - *

Specifikation af åbningstider (klasse)
Vokabular-definition og beskrivelser
URI	http://schema.org/OpeningHoursSpecification

Term	Specifikation af åbningstider
Kommentar	En struktureret værdi, der giver information om åbningstiderne for et sted eller en bestemt tjeneste inde på et sted.
Stedet er åbent, hvis egenskaben ’opens’ er angivet og lukket ellers.
Hvis værdien for egenskaben ’closes’ er mindre end værdien for ’opens’ egenskaben, så antages timeintervallet at strække sig over den næste dag.
Underklasse af	schema:StructuredValue
Profilens kontekstrestriktioner og annotationer 
Definition	[fra informationsmodel (klassen Åbningstid)]
giver information om åbningstider som en del af beskrivelsen for en kontaktoplysning

åbner
Vokabular-definition og beskrivelser
URI	http://schema.org/opens

Term	åbner
Kommentar	Stedets eller tjenestens åbningstid på den eller de givne dag(e) i ugen.
Domæne	schema:OpeningHoursSpecification
Udfaldsrum	schema:Time
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel (klassen Åbningstid)]
det tidspunkt lokationen eller tjenesten åbner på den eller de angivne ugedage
Anvendelsesnote	Åbningstid for den kontakt der repræsenteres i den kvalificerede kontaktinformation
Domæne	schema:OpeningHoursSpecification
Udfaldsrum	xsd:time
Multiplicitet	1 - 1

lukker
Vokabular-definition og beskrivelser
URI	http://schema.org/closes

Term	lukker
Kommentar	Stedets eller tjenestens lukketid på den eller de givne dag(e) i ugen.
Domæne	schema:OpeningHoursSpecification
Udfaldsrum	schema:Time
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel (klassen Åbningstid)]
det tidspunkt lokationen eller tjenesten lukker på den eller de angivne ugedage
Anvendelsesnote	Lukketid for den kontakt der repræsenteres i den kvalificerede kontaktinformation
Domæne	schema:OpeningHoursSpecification
Udfaldsrum	xsd:time
Multiplicitet	1 - 1

gælder fra
Vokabular-definition og beskrivelser
URI	http://schema.org/validFrom

Term	gælder fra
Kommentar	Den dato, hvor varen bliver gyldig.
Domæne	schema:Permit  eller  schema:Certification  eller  schema:MonetaryAmount  eller  schema:Offer  eller  schema:OpeningHoursSpecification  eller  schema:LocationFeatureSpecification  eller  schema:Demand  eller  schema:PriceSpecification
Udfaldsrum	schema:DateTime  eller  schema:Date
Profil-restriktioner og annotationer 
Anvendelsesnote	Den dato, hvor den kvalificerede kontaktinformation bliver gyldig.
Udfaldsrum	xsd:dateTime
Multiplicitet	0 - 1

gælder indtil
Vokabular-definition og beskrivelser
URI	http://schema.org/validThrough

Term	gælder indtil
Domæne	schema:PriceSpecification  eller  schema:MonetaryAmount  eller  schema:JobPosting  eller  schema:Offer  eller   schema:OpeningHoursSpecification  eller  schema:LocationFeatureSpecification  eller  schema:Demand
Udfaldsrum	schema:DateTime  eller  schema:Date
Profil-restriktioner og annotationer 
Anvendelsesnote	Den dato, hvor den kvalificerede kontaktinformation bliver ugyldig
Udfaldsrum	xsd:dateTime
Multiplicitet	0 - 1

ugedag
Vokabular-definition og beskrivelser
URI	http://schema.org/dayOfWeek

Term	ugedag
Kommentar	Den ugedag, som disse åbningstider er gældende for.
Domæne	schema:OpeningHoursSpecification  eller  schema:EducationalOccupationalProgram
Udfaldsrum	schema:DayOfWeek  eller  schema:Text  eller  schema:URL  eller  schema:Role
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel (klassen Åbningstid)]
bestemt dag i ugen
Domæne	schema:OpeningHoursSpecification
Udfaldsrum	schema:DayOfWeek
Multiplicitet	1 - 1

Ugedag (klasse)
Vokabular-definition og beskrivelser
URI	http://schema.org/DayOfWeek

Term	Ugedag
Kommentar	Ugedagen, bruges eksempelvis til at angive, hvilken dag åbningstiderne for en OpeningHoursSpecification refererer til.
Oprindeligt blev URLer fra ’GoodRelations’ brugt (til ‘Monday’, ‘Tuesday’, ’Wednesday’, ’Thursday’ ’Friday’, ’Saturday’, ’Sunday’ plus en særlig post til ’PublicHolidays’; disse er nu blevet integreret direkte i schema.org.
Underklasse af	schema:Enumeration
Profilens kontekstrestriktioner og annotationer 
Anvendelsesnote	Enumeration bestående af:
Friday
Monday
PublicHolidays
Saturday
Sunday
Thursday
Tuesday
Wednesday


