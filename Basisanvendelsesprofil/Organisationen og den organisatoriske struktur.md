# Organisationen og den organisatoriske struktur

(billede)
 
Organisationer vil i de fleste tilfælde have en organisatorisk struktur, oftest en hierarkisk form. 
En organisation kan bestå af flere underorganisationer der hver for sig har en specifik identitet, fx kan et ministerium bestå af flere underordnede styrelser.
En organisation kan være inddelt i mindre organisationsenheder hvis eksistens er afhængig af organisationen, fx en afdeling i en større organisation. Organisationer består typisk af mange afdelinger, kontorer, enheder, teams, grupper osv. En organisationsenhed kan også have underordnede enheder.
Organisationer kan indbyrdes have andre former for relationer end de der udtrykkes i form af under- og overorganisatoriske forhold, fx finansiering eller kæderelationer.
En organisation kan klassificeres som værende af en bestemt organisationstype. I forhold til offentlige organisationer kunne det fx være kommune, region, ministerier, styrelser og mange af de andre former for offentlige organisationer, der er en væsentlig del af hverdagen i det offentlige organisationslandskab.
Organisationen og dens dele
I den organisatoriske struktur indgår to helt centrale klasser:
Den klasse der repræsenterer organisationen som den helhed der normalt tænkes på når der refereres til organisationen. Klassen for den formelle organisation.
Den klasse der repræsentere afgrænsede dele af organisationen. Klassen for organisatoriske enheder.
Formel organisation (klasse)
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/org#FormalOrganization

Term	Formel organisation
Kommentar	En organisation, der er anerkendt i verden bredt set, især i juridiske jurisdiktioner, med tilhørende rettigheder og ansvar. Eksempler inkluderer et selskab, velgørenhed, regering eller kirke.
Anvendelsesnote	Bemærk, at dette er en superklasse af `gr:BusinessEntity`, og det anbefales at bruge GoodRelations-vikabularet til at betegne Business-klassifikationer såsom DUNS eller NAICS.
Underklasse af	foaf:Organization
org:Organization 

Profilens kontekstrestriktioner og annotationer 
Alternativ term	Organisation
Definition	[Fra Informationsmodel]
En organisation, der er bredt anerkendt i omverdenen, med tilhørende rettigheder og ansvar
Eksempel	[Fra Informationsmodel]
Organisationer kan ofte nedbrydes i hierarkiske strukturer
Organisationen er "rammen" for alle de øvrige elementer (Organisationsenheder, Organisationsmedlemmer og deres indbyrdes relationer)
Eksempel: 
o	et aktieselskab 
o	en statslig styrelse
o	en velgørende forening
o	en kirkelig forening
- ....

Organisatorisk enhed (klasse)
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/org#OrganizationalUnit
Term	Organisatorisk enhed
Kommentar	En organisation, såsom en afdeling eller supportenhed, som er en del af en større organisation og kun har fuld anerkendelse inden for den pågældende organisations kontekst. Navnlig vil enheden ikke blive betragtet som en juridisk enhed i sig selv.
Anvendelsesnote	Enheder kan være store og komplekse og indeholde andre enheder. Alternative navne: Afdeling
Underklasse af	foaf:Organization
org:Organization
Profilens kontekstrestriktioner og annotationer 
Alternativ term	Afdeling
Definition	[Fra informationsmodel]
en afdeling eller enhed i en organisation
Kommentar	[Fra informationsmodel]
organisationsenheder kan være mere eller mindre permanente. Eksempelvis kan der oprettes en organisationsenhed til et projekt, hvorefter den opløses, når projektet er slut. Eller en organisationsenhed kan være en permanent del af organisationen, som f.eks. "bogholderiet".
Fælles for organisationsenheder er, at de har til formål at have noget at samle organisationsmedlemmer i og kan omtale som noget kendt i organisationen.
Eksempel	[Fra informationsmodel]
o	Bogholderiet
o	Projekt "ny organisationsstandard"
o	Hæmatologisk afdeling
- ...

Typer af ’Formel organisation’ og ’Organisatorisk enhed’
Det foreslås i første udgave af basisprofilen at undlade inddragelse af klasser som ’Myndighed’ og ’Virksomhed’. Klassen ’Formel organisation’ har fået tilføjet en egenskab der peger på en klassifikation af organisationstyper, der blandt andet kan indeholde både ’Myndighed’ og ’Virksomhed’ og andre relevante typeangivelser, eksempelvis ’Region’, ’Kommune’ og ’Statslig styrelse’.
Fra ORG genanvendes org:classification til at angive typen af organisation.

 

Som indikeret i ovenstående illustration så benyttes egenskaben org:classification til at udpege en klassifikation hvis emner repræsenterer organisationstyper. De viste emner er udelukkende eksempler på mulige typer af oranisationer. Klassifikationen kan udvides løbende efter behov.
Senere udgaver af basisprofilen vil kunne indeholde de to nævnte klasser og andre relevante specialiseringer af ’Formel organisation’, hvis der er behov for det.
’Myndighed’ vil i det tilfælde kunne repræsenteres som en klasse der både er en delmængde af klassen ’Formel organisation’ og en delmængde af klassen ’Offentlig organisation’ (https://semiceu.github.io/CPOV/releases/2.00/#Public%20Organisation ).
For ’Virksomhed’ vil klassen ’Juridisk enhed’ (https://semiceu.github.io/Core-Business-Vocabulary/releases/2.00/#Legal%20Entity ) kunne anvendes.

            

På tilsvarende måde bruges org:classification til at angive typen af organisatorisk enhed.
I kapitlerne ’Den formelle organisations egenskaber’ og ’Den organisatoriske enheds egenskaber’ beskrives de to klasser der er anvendt til typeangivelse.
Organisationens tilhørende enheder
 
enhed af 
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/org#unitOf 

Term	enhed af
Kommentar	Angiver en organisation, som denne enhed er en del af, f.eks. en afdeling inden for en større formel organisation.
Anvendelsesnote	Dette er den inverse af org:hasUnit.

Domæne	org:OrganizationalUnit
Udfaldsrum	org:Organization
Underegenskab af	org:subOrganizationOf
Modsatrettet egenskab	org:hasUnit
Profilens kontekstrestriktioner og annotationer 
Definition	[fra informationsmodel]
organisationsenheder vil altid høre til netop en Organisation
Kommentar	Angiver en formel organisation, som denne organisatoriske enhed er en del af, f.eks. en afdeling inden for en større formel organisation
Kommentar	[fra informationsmodel]
en organsation kan have mange organisatoriske enheder
Anvendelsesnote	En organisatorisk enhed skal altid være tilknyttet en og kun en formel organisation.
Udfaldsrum	org:FormalOrganization
Multiplicitet	1 - 1

øvre enhed i 
Vokabular-definition og beskrivelser
URI	https://data.gov.dk/model/core/organisation/extension/upperUnitOf 

Term	øvre enhed i
Alternativ term	top enhed i
Definition	Angiver den formelle organisation som en topenhed er en del af.
Domæne	org:OrganizationalUnit
Udfaldsrum	org:FormalOrganization
Underegenskab af	org:uniOf
Modsatrettet egenskab	ovx:hasUpperUnit
Profil-restriktioner og annotationer 
Definition	[fra informationsmodel]
markerer at denne orgaisationsenhed er den øverste i et hiererki.
Multiplicitet	0 - 1

Organisatoriske enheders indbyrdes hierarki
 
enhed af
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/org#unitOf 

Term	enhed af
Kommentar	Angiver en organisation, som denne enhed er en del af, f.eks. en afdeling inden for en større formel organisation.
Anvendelsesnote	Dette er den inverse egenskab af org:hasUnit.
Domæne	org:OrganizationalUnit
Udfaldsrum	org:Organization
Underegenskab af	org:subOrganizationOf
Modsatrettet egenskab	org:hasUnit
Profilens kontekstrestriktioner og annotationer 
Definition	[fra informationsmodel]
en organisationsenhed kan være underlagt en anden organisationsenhed
Kommentar	[fra informationsmodel]
en organisationsenhed kan indeholde 0 en eller flere enheder.
Anvendelsesnote	Anvendes fra ’Organisatorisk enhed’ til at angive en enhed (i samme organisation) som den anvende enhed er organisatorisk underlagt.
Multiplicitet	1 - 1

Organisationens relationer til andre organisationer
 
underorganisation af
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/org#subOrganizationOf 

Term	underorganisation af
Kommentar	Repræsenterer hierarkisk indhold af organisationer eller organisationsenheder. Den angiver en organisation, som indeholder denne organisation.
Domæne	org:Organization
Udfaldsrum	org:Organization
Underegenskab af	org:transitiveSubOrganizationOf
Modsatrettet egenskab	org:hasSubOrganization
Profilens kontekstrestriktioner og annotationer 
Definition	[fra informationsmodel]
en organisation kan indeholde andre organisationer
Kommentar	[fra informationsmodel]
Digitaliseringsstyrelsen er en selvstændig juridisk organisation som er en del af Finansministeriet og deres organisation
Anvendelsesnote	Bruges til at angive en hierarkisk overordnet organisation.
Domæne	org:FomalOrganization
Udfaldsrum	org:FomalOrganization
Multiplicitet	0 - 1

relateret til
Vokabular-definition og beskrivelser
URI	http://www.w3.org/ns/org#linkedTo

Term	relateret til
Kommentar	Angiver en arbitrær relation mellem to organisationer
Anvendelsesnote	Specialiseringer heraf kan bruges til fx at betegne finansiering eller forsyningskædeforhold.
Domæne	org:Organization

Udfaldsrum	org:Organization

Profilens kontekstrestriktioner og annotationer 
Anvendelsesnote	Bruges til at angive en organisation som denne organisation har en eller anden relation til.
Domæne	org:FomalOrganization
Udfaldsrum	org:FomalOrganization
Multiplicitet	0 - *
