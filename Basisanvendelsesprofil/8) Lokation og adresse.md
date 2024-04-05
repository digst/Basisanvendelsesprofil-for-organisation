# Lokation og adresse
 
## Lokationen
Med anvendelsesprofilen kan en organisations fysiske placering angives enten direkte med en adresse eller via angivelse af et sted hvor organisationen holder til. Det sted organisationen holder til kan også tilføjes en adresse. 
Fra vokabularet Location Core Vocabulary anvendes egenskaben locn:address til at angive en direkte forbindelse mellem organisationen og en adresse. Fra samme vokabular anvendes også klassen locn:Address, der er defineret for at være kompatibel med INSPIREs krav til adresser.
En organisation og en organisationsenheds fysiske placering kan angives. En organisation kan også have flere forskellige fysiske placeringer.
Placeringen kan fx angives med en adresse.
 

lokation
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#location 

Term	lokation 
Beskrivelse	Knytter en ressource til den tilsvarende placering.
Anvendelsesnote	At erklære placeringsforholdet indebærer kun, at domænet har en eller anden forbindelse til en placering i tid eller rum. Det betyder ikke, at ressourcen nødvendigvis er på det sted på det tidspunkt, hvor påstanden fremsættes.
Domæne	rdfs:Resource 
Udfaldsrum	dct:Location
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel (klassen Organisation]]
beskriver hvor en organisation er beliggende
Definition	[fra informationsmodel (klassen Organisationsenhed]]
beskriver hvor en organisationsenhed er beliggende
Kommentar	[fra informationsmodel (klassen Organisation]]
Det kan både være et fysisk og et virtuelt sted
Denne relation kan evt. baseres på CVR''s adresserelation, hvis organisationen beskriver en virksomheds organisationsstruktur.
Kommentar	[fra informationsmodel (klassen Organisationsenhed]
Det kan både være et fysisk og et virtuelt sted.
Domæne	org:FormalOrganization  eller  org:OrganizationalUnit
Udfaldsrum	dct:Location
Multiplicitet	0 - *

Lokation (klasse)
Vokabular-definition og beskrivelser
URI	http://purl.org/dc/terms/Location

Term	Lokation
Kommentar	Et spatialt område eller navngivet sted.
Underklasse af	dct:LocationPeriodOrJurisdiction
Profilens kontekstrestriktioner og annotationer 
Definition	[fra informationsmodel (klassen Sted)]
en fysisk eller virtuel lokation, hvor organisationen kan kontaktes
Kommentar	Dette er nøgleklassen for ISA Program Location Core Vocabulary og repræsenterer enhver placering, uanset størrelse eller anden begrænsning.

geografisk identifikator
Vokabular-definition og beskrivelser
URI	http://www.w3.org/2000/01/rdf-schema#seeAlso

Term	se også
Kommentar	Yderligere information om subjektressourcen.
Domæne	rdfs:Resource
Udfaldsrum	rdfs:Resource
Profil-restriktioner og annotationer 
Term	geografisk identifikator
Anvendelsesnote	GeoNames.org leverer stabile, bredt anerkendte identifikatorer for mere end 10 millioner geografiske navne, der kan bruges som links til yderligere information. For eksempel identificerer http://sws.geonames.org/593116/ den litauiske hovedstad Vilnius. Desværre kan disse URI'er ikke let udledes automatisk, da URI-skemaet bruger simple numeriske koder. At finde en GeoNames identifikator for en placering er næsten altid en manuel proces. Hvor sådanne identifikatorer er kendte eller kan findes, anbefales det dog, at de bruges. Hvor Location Class bruges til at identificere et land, hvis geonavnene URI ikke er kendt, anbefales det at bruge DBpedia URI'er i formen http://dbpedia.org/resource/ISO\_3166-1:XX hvor XX er ISO 3166 to tegn kode for landet.
EU's Publikationskontor afviger fra ISO 3166-1 og bruger EL og UK for henholdsvis Grækenland og Storbritannien. DBpedia holder sig til ISO-koderne, og derfor er de korrekte URI'er for disse lande: - http://dbpedia.org/resource/ISO\_3166-1:GR - http://dbpedia.org/resource/ISO\_3166-1 :GB selv når det geografiske navn er angivet som EL eller UK.
Domæne	dct:Location
Udfaldsrum	xsd:anyURI
Multiplicitet	0 - 1

geografisk navn
URI	http://www.w3.org/ns/locn#geographicName 

Betegnelse (EN)	geographic name
Definition (EN)	A textual description for a Location.
Anvendelsesnote (EN)	The INSPIRE Data Specification on Geographical Names provides a detailed model for describing a 'named place', including methods for providing multiple names in multiple scripts. INSPIRE's definition is the following: Names of areas, regions, localities, cities, suburbs, towns or settlements, or any geographical or topographical feature of public or historical interest. This is beyond what is necessary for the Core Location Vocabulary but, importantly, the concept of a geographic name used here is consistent..
A geographic name is a proper noun applied to a spatial object. Taking the example used in the INSPIRE document (page 18), the following are all valid geographic names for the Greek capital: - "Aθnνa"@gr-Grek (the Greek endonym written in the Greek script) - "Athína"@gr-Latn (the standard Romanisation of the endonym) - "Athens"@en (the English language exonym) INSPIRE has a detailed (XML-based) method of providing metadata about a geographic name and in XML-data sets that may be the most appropriate method to follow. When using the Core Location Vocabulary in data sets that are not focussed on environmental/geographical data (the use case for INSPIRE), the Code datatype or a simple language identifier may be used to provide such metadata. 
The country codes defined in ISO 3166 may be used as geographic names and these are generally preferred over either the long form or short form of a country's name (as they are less error prone). The Publications Office of the European Union recommends the use of ISO 3166-1 codes for countries in all cases except two: - use 'UK' in preference to the ISO 3166 code GB for the United Kingdom; - use 'EL' in preference to the ISO 3166 code GR for Greece. Where a country has changed its name or no longer exists (such as Czechoslovakia, Yugoslavia etc.) use the ISO 3166-3 code.
Udfaldsrum	rdf:langString
Multiplicitet
0 - *
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#geographicName

Term	geografisk navn
Beskrivelse	En tekstbeskrivelse for en placering.
Anvendelsesnote	INSPIRE-dataspecifikationen om geografiske navne giver en detaljeret model til at beskrive et 'navngivet sted', herunder metoder til at angive flere navne i flere scripts. INSPIREs definition er følgende: Navne på områder, regioner, lokaliteter, byer, forstæder, byer eller bygder eller ethvert geografisk eller topografisk træk af offentlig eller historisk interesse. Dette er ud over, hvad der er nødvendigt for Core Location Vocabulary, men vigtigst af alt er konceptet med et geografisk navn, der bruges her, konsekvent.
Et geografisk navn er et egennavn anvendt på et rumligt objekt. Med eksemplet brugt i INSPIRE-dokumentet (side 18), er følgende alle gyldige geografiske navne for den græske hovedstad: - "Aθnνa"@gr-Grek (det græske endonym skrevet i den græske skrift) - "Athína"@gr- Latn (standardromaniseringen af endonymet) - "Athens"@en (det engelsksprogede eksonym) INSPIRE har en detaljeret (XML-baseret) metode til at levere metadata om et geografisk navn og i XML-datasæt, der kan være den mest passende metode at følge. Når du bruger Core Location Vocabulary i datasæt, der ikke er fokuseret på miljømæssige/geografiske data (brugssagen for INSPIRE), kan kodedatatypen eller en simpel sprogidentifikator bruges til at levere sådanne metadata.
Landekoderne defineret i ISO 3166 kan bruges som geografiske navne, og disse foretrækkes generelt frem for enten den lange form eller den korte form af et lands navn (da de er mindre fejltilbøjelige). Den Europæiske Unions Publikationskontor anbefaler brugen af ISO 3166-1-koder for lande i alle tilfælde undtagen to: - Brug 'UK' frem for ISO 3166-koden GB for Det Forenede Kongerige; - Brug "EL" frem for ISO 3166-koden GR for Grækenland. Hvis et land har skiftet navn eller ikke længere eksisterer (såsom Tjekkoslovakiet, Jugoslavien osv.), skal du bruge ISO 3166-3-koden.
Domæne	dct:Location
Udfaldsrum	rdf:langString
Profil-restriktioner og annotationer 
Domæne	dct:Location
Udfaldsrum	rdf:langString
Multiplicitet	0 - *

p-nummer
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/registered-business/productionUnitCode

Term	p-nummer
Definition	Et entydigt identifikationsnummer for en lokation hvor en juridisk enhed har aktivitet.
Ækvivalent egenskab	
Profil-restriktioner og annotationer 
Udfaldsrum	xsd:string
Multiplicitet	0 - *


 
Adressen
 

adresse
Vokabular-definition og beskrivelser
URI	http://w3.org/ns/locn#address

Term	adresse
Definition	Knytter en ressource til den tilsvarende adresse.
Anvendelsesnote	At erklære adresseforholdet indebærer, at ressourcen har en adresse
Domæne	rdfs:Resource
Udfaldsrum	locn:Address
Profil-restriktioner og annotationer 
Kommentar	Noter at det vil være muligt at definerer specialiseringer af locn:address til specifikke adressetyper, eksempelvis ’besøgsadresse’, ’postadresse’, aktivitetsadresse og andre der findes behov for. 
Domæne	org:FormalOrganization  eller  org:OrganizationalUnit  eller  dct:Location
Udfaldsrum	locn:Address
Multiplicitet	0 - *


Adresse (klasse)
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#Address

Term	Adresse
Definition	Et spatialt objekt, der på en menneskelig læsbar måde identificerer en fast placering.
Anvendelsesnote	En "adresserepræsentation" som konceptuelt defineret af INSPIRE-adresserepræsentationens datatype: "Repræsentation af et geografisk adresseobjekt til brug i eksterne applikationsskemaer, der skal inkludere den grundlæggende adresseinformation på en læsbar måde.".
Repræsentationen af adresser varierer meget fra det ene lands postsystem til det andet. Selv inden for lande er der næsten altid eksempler på adresser, der ikke er i overensstemmelse med den angivne nationale standard. ISO 19160-1 giver dog en metode, hvorigennem forskellige adresser kan konverteres fra en konceptuel model til en anden.
Denne specifikation var stærkt baseret på INSPIRE-adresserepræsentationens datatype. Det er bemærkelsesværdigt, at hvis en adresse er angivet ved hjælp af den detaljerede opdeling foreslået af egenskaberne for denne klasse, så vil den være INSPIRE-konform. Til dette meget granulerede sæt af egenskaber tilføjer vi yderligere to egenskaber:
- fuld adresse (den komplette adresse som en formateret streng)
- addressID (en unik identifikator for adressen).
Den første af disse giver udgivere mulighed for blot at angive den komplette adresse som én streng, med eller uden formatering. Dette er analogt med vCards etiketegenskab.
Adresse-ID'et er en del af INSPIRE-retningslinjerne og giver en hook, der kan bruges til at knytte adressen til en alternativ repræsentation, såsom vCard eller OASIS xAL.
Profilens kontekstrestriktioner og annotationer 
Definition	[fra Grunddatamodel, objekttype: Adresse]
En struktureret betegnelse som angiver en særskilt adgang til et areal, en bygning eller en del af en bygning, efter reglerne i adressebekendtgørelsen.
Definition	[fra informationsmodel, klassen Adresse (1)]
et sted hvor man kan finde virksomheden, udtrykt som en traditionel adresse
Definition	[fra informationsmodel, klassen Adresse (2)]
En struktureret betegnelse som angiver en særskilt adgang til et areal, en bygning eller en del af en bygning, efter reglerne i adressebekendtgørelsen.
Kommentar	[fra Grunddatamodel, objekttype: Adresse]
en sammensat betegnelse, som udpeger og benævner en bestemt adgangsvej til et ubebygget areal, en bygning, en del af en bygning, et teknisk anlæg eller lignende. Reglerne for fastsættelse af adresser findes i adressebekendtgørelsen. BEK nr 271 af 13/04/2018. 
Kommentar	[fra informationsmodel (klassen Adresse (1))]
Kan være dels en dansk adresse udtrykt ved enten et DAR-objekt eller en Cpr-adresse eller det kan være en udenlandsk/simpel adresse udtrykt ved 5 linjers fritekst.
Kommentar	[fra informationsmodel (klassen Adresse (2))]
En adresse fastsættes for at angive en bestemt adgang til et areal, fx. en byggegrund, en bygning eller en del af en bygning, fx en bolig- eller erhvervsenhed i en bygning. Reglerne for fastsættelse af adresser findes i adressebekendtgørelsen.
Link til byggeblok Adresse:
Danmarks adresser(DAR) v2.0.0 - Grunddata informationsmodel

Eksempel	[fra Grunddatamodel, objekttype: Adresse]
adressebetegnelse: Gimles Allé 14, 2300 København S adressebetegnelse: Vestergade 4B, st. th, Strib, 5500 Middelfart

vejnavn
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#thoroughfare

Term	vejnavn
Definition	Navnet på en passage eller vej igennem fra et sted til et andet.
Kommentar	Bruges til at angive den del af adressen som repræsenterer vejens navn.
Anvendelsesnote	En færdselsåre er normalt en gade, men det kan være en vandvej eller en anden funktion. For eksempel "Avenue des Champs-Élysées".
Domæne	locn:Address
Udfaldsrum	rdf:langString
Profil-restriktioner og annotationer 
Domæne	locn:Address
Udfaldsrum	rdf:langString
Multiplicitet	0 - 1

positionsindikator
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#locatorDesignator

Term	positionsindikator
Definition	Et antal eller en sekvens af tegn, der entydigt identificerer lokalisatoren inden for det relevante omfang.
Kommentar	I enklere vendinger er dette bygningsnummer, lejlighedsnummer osv. For en adresse som "Lejlighed 3, 17 Bridge Street", er lokalisatoren "lejlighed 3, 17".
Anvendelsesnote	Bruges til at angive husnummer, dørbetegnelse, etagebetegnelse og lignende.
Profil-restriktioner og annotationer 
Udfaldsrum	xsd:string
Multiplicitet	0 - 1

…………………………………
Egenskaben locn:locatorDesignator (positionsindikator) dækker flere egenskaber i DAR, fx. husnummertekst, etagebetegnelse og dørbetegnelse, som en samlet, sammensat tekststreng. For at bevare muligheden for at angive de nævnte tre DAR-egenskaber enkeltvis, repræsenteres disse også som valgmuligheder på klassen locn:Address. De tre egenskaber beskrives efterfølgende.
husnummertekst
Vokabular-definition og beskrivelser
URI	???????????????
Term	husnummertekst
Alternativ term	husnummer
Definition	husnummeret til adressen inklusive evt. bogstav
Domæne	locn:Address
Udfaldsrum	xsd:string
Profil-restriktioner og annotationer 
Definition	[fra Grunddatamodel, objekttype: Adresse]
husnummeret til adressen inklusive evt. bogstav
Kommentar	[fra Grunddatamodel, objekttype: Adresse]
et husnummer består af et tal 1-999 eventuelt efterfulgt af et stort bogstav. Reglerne for udformning af husnummer herunder hvilke bogstaver der kan anvendes, fremgår af adressebekendtgørelsen
Eksempel	[fra Grunddatamodel, objekttype: Adresse]
”12”, ”12A”, ”158C”
Multiplicitet	0 - 1

dørbetegnelse
Vokabular-definition og beskrivelser
URI	????????????????
Term	dørbetegnelse
Definition	Betegnelse, som angiver den adgangsdør e.l. som adressen identificerer
Domæne	locn:Address
Udfaldsrum	xsd:string
Profil-restriktioner og annotationer 
Definition	[fra Grunddatamodel, objekttype: Adresse]
betegnelse, som angiver den adgangsdør e.l. som adressen identificerer
Kommentar	[fra Grunddatamodel, objekttype: Adresse]
dørbetegnelsen angives normalt med udgangspunkt i det fælles adgangsareal på den pågældende etage (fx trappeafsats e.l.) som døren er placeret i. Reglerne for dørbetegnelsen, herunder værdisæt, fremgår af adressebekendtgørelsen. 
Eksempel	[fra Grunddatamodel, objekttype: Adresse]
”th”, ”a109”
Multiplicitet	0 - 1

etagebetegnelse
Vokabular-definition og beskrivelser
URI	???????????????
Term	etagebetegnelse
Definition	Betegnelse, som angiver hvilken etage den del af bygningen som adressen identificerer, er beliggende på
Domæne	locn:Address
Udfaldsrum	xsd:string
Profil-restriktioner og annotationer 
Definition	[fra Grunddatamodel, objekttype: Adresse]
betegnelse, som angiver hvilken etage den del af bygningen som adressen identificerer, er beliggende på
Kommentar	[fra Grunddatamodel, objekttype: Adresse]
reglerne for etagebetegnelsen, herunder værdisæt, fremgår af adressebekendtgørelsen. Stueetage angives "st", 1. og 2. sal hhv. "1", "2" osv. Kælderetagen angives "kl", etager herunder "k2", "k3" osv. Betegnelserne 0 eller -1 osv. må ikke anvendes
Eksempel	[fra Grunddatamodel, objekttype: Adresse]
”st”
Multiplicitet	0 - 1

…………………………………
supplerende bynavn
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#addressArea  

Term	supplerende bynavn
Definition	Navnet på et geografisk område, der grupperer adresser.
Anvendelsesnote	Dette vil typisk være en del af en by, et kvarter eller en landsby, f.eks. Montmartre. Adresseområdet er ikke en administrativ enhed.
Domæne	locn:Address
Udfaldsrum	rdf:langString
Profil-restriktioner og annotationer 
Multiplicitet	0 - 1

postboks
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#poBox
Term	postboks
Definition	En placeringsbetegnelse for et postleveringssted på et postkontor, normalt et nummer.
Kommentar	INSPIREs navn for dette er "postalDeliveryIdentifier", som den bruger locator designator-egenskaben til med en type-attribut med det navn. Core Location Vocabulary adskiller postkassen for større uafhængighed af teknologi. Et eksempel på postkassenummer er "9383".
Domæne	locn:Address
Udfaldsrum	xsd:string
Profil-restriktioner og annotationer 
Multiplicitet	0 - 1

postnummer
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#postCode

Term	postnummer
Definition	Koden oprettet og vedligeholdt til postformål for at identificere en underopdeling af adresser og postleveringssteder
Kommentar	Postnumre er almindelige elementer i mange landes postadressesystemer. Et af de mange postnumre i Paris er for eksempel "75000".
Domæne	locn:Address
Udfaldsrum	xsd:string
Profil-restriktioner og annotationer 
Multiplicitet	0 - 1

postnummernavn
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#postName

Term	postnummernavn
Definition	Et navn, der er oprettet og vedligeholdt til postformål for at identificere en underopdeling af adresser og postleveringssteder.
Kommentar	Normalt en by, for eksempel "Paris".
Domæne	locn:Address
Udfaldsrum	rdf:langString
Profil-restriktioner og annotationer 
Multiplicitet	0 - 1

fuld adresse
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#fullAddress

Term	fuld adresse
Definition	Den komplette adresse skrevet som en streng.
Kommentar	Det anbefales at bruge denne egenskab, og dermed undgå misforståelser, der ellers kan opstå ved opdelingen af en adresse i dens komponenter. Denne egenskab er analog med vCards label-egenskab, men med to vigtige forskelle: (1) formatering forudsættes ikke, så det i modsætning til en vCard-etiket muligvis ikke er egnet at udskrive som en adresselabel, (2) vCards label-egenskab har et domæne af vCard-adresse; ejendommen fullAddress har ingen tilsvarende begrænsning. Et eksempel på en fuldstændig adresse er "Champ de Mars, 5 Avenue Anatole France, 75007 Paris, France"
Domæne	locn:Address
Udfaldsrum	rdf:langString
Profil-restriktioner og annotationer 
Alternativ term	[fra Grunddatamodel, objekttype: Adresse]
adressebetegnelse
Definition	[fra Grunddatamodel, objekttype: Adresse]
en læsbar struktur, som identificerer adressen fuldstændigt
Kommentar	[fra Grunddatamodel, objekttype: Adresse]
adressebetegnelse er sammensat af betegnelserne: vejnavn, husnummer, evt. etage- og dørbetegnelse, evt. supplerende bynavn samt postnummer og postbynavn. Reglerne for formateringen findes i vejledningen i fastsættelse af vejnavne og adresser. https://danmarksadresser.dk/om-adresser/saadan-gengives-en-adresse 
Eksempel	[fra Grunddatamodel, objekttype: Adresse]
”Gimles Allé 14, 2300 København S”, ”Vestergade 4B, st. th, Strib, 5500 Middelfart”
Multiplicitet	0 - 1

adresse-id
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/locn#addressID

Term	adresse-id
Definition	En globalt unik identifikator for hver forekomst af en adresse.
Kommentar	Konceptet med at tilføje en globalt unik identifikator for hver forekomst af en adresse er en afgørende del af INSPIRE-dataspecifikationen. En række EU-lande har allerede implementeret et ID (et UUID) i deres adresseregister/gazetteer, heriblandt Danmark. OASIS xAL inkluderer også en adresseidentifikator. Det er adresseidentifikatoren, der gør det muligt at repræsentere en adresse i et andet format end INSPIRE, mens den forbliver i overensstemmelse med kernevokabularet.
INSPIRE-metoden til at repræsentere adresser er meget detaljeret, designet primært til brug i adressedatabaser. Mens data, der er offentliggjort i fuld overensstemmelse med INSPIRE-datastrukturen, kan gøres tilgængelige ved hjælp af Core Location Vocabulary, er det omvendte ikke tilfældet, da Core Vocabulary tillader meget større fleksibilitet.
Mange datasæt, der inkluderer adressedata som del af information om noget andet, vil sandsynligvis have disse data i enklere formater. Disse kan være udformet til datasættets specifikke behov, følge en national norm eller gøre brug af en standard som vCard.
For at give maksimal fleksibilitet i Core Vocabulary, mens den forbliver interoperabel med INSPIRE Address Guidelines (som EU-medlemsstaterne er forpligtet til at bruge), giver Core Location Vocabulary den ekstra egenskab med fuld adresse og gør brug af INSPIRE's addressID.
Udfaldsrum	xsd:string
Profil-restriktioner og annotationer 
Multiplicitet	0 - 1

 
