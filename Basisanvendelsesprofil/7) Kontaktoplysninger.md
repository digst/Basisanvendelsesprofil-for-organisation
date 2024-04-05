# Kontaktoplysninger
En organisation kan kontaktes af eksterne på forskellige måder. Kontakten kan ske ved ved personligt fremmøde til en besøgsadresse eller ved at sende post til postadresse. Kontakten kan også foretages via telefon, fax, e-mail eller en dedikeret webside. 

I basisprofilen er alle de nævnte kontaktformer repræsenteret både i relation til den formelle organisation og i relation til organisatoriske enheder. Kontaktformerne er både repræsenteret som direkte tilknyttet en organisation eller en organisatoriske enhed, samt – hvor der er behov for det – tilknyttet som mere kvalificeret information. Kvalificeret information betyder i denne sammenhæng at der til kontaktformen, eksempelvis et telefonnummer, tilføjes data der giver mere information, eksempelvis hvilke tidspunkter der kan ringes på.

Både direkte tilknyttet kontaktinformation og kvalificeret kontaktinformation beskrives efterfølgende.

(indsæt billede) 

## Direkte relateret kontaktinformation

(indsæt billede)
 
#### telefon
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/telephone</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>telefon</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Telefonnummeret</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:Organization eller schema:Person eller schema:ContactPoint eller schema:Place</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:Text eller schema:URL eller schema:Role</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Myndighed)]</td>
  </tr>
  <tr>
    <td>Telefonnummer til myndighed</td>
    <td></td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Telefon)]</td>
  </tr>
  <tr>
    <td>telefonnummer som tilhører et bestemt abonnement</td>
    <td></td>
  </tr>
  <tr>
    <td>Beskrivelse</td>
    <td>Et telefonnummer er en talkode bestående af et antal cifre, der identificerer et telefonabonnement eller en teletjeneste. Nummeret bruges til at kontakte abonnenten eller tjenesten.</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>org:FormalOrganization eller org:OrganizationalUnit</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>xsd:string</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
  </tr>
</table>


#### e-mail
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/email</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>e-mail</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>E-mail adresse</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:Organization<br>eller schema:Person<br>eller schema:ContactPoint</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:Text<br>eller schema:URL<br>eller schema:Role</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Myndighed)]</td>
  </tr>
  <tr>
    <td>Elektronisk kontaktadresse på myndighed</td>
    <td></td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Mail)]</td>
  </tr>
  <tr>
    <td>adresse der identificerer en elektronisk postkasse til hvilken meddelelser kan leveres</td>
    <td></td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>[fra informationsmodel (klassen Mail)]</td>
  </tr>
  <tr>
    <td>opbygget af et brugernavn og et servernavn adskilt af @</td>
    <td></td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>org:FormalOrganization eller org:OrganizationalUnit</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>xsd:string</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
  </tr>
</table>


#### faxnummer
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/faxNumber</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>faxnummer</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Fax-nummeret</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:Place eller schema:Organization eller schema:Person eller schema:ContactPoint</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:Text eller schema:URL eller schema:Role</td>
  </tr>
  <tr>
    <td>Profil-restriktioner og annotationer</td>
    <td></td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>org:FormalOrganization eller org:OrganizationalUnit</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>xsd:string</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
  </tr>
</table>

#### webside
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://xmlns.com/foaf/0.1/page</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>side</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>En side eller et dokument om denne ting</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>foaf:Document</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Term</td>
    <td>webside</td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen VirtuelLokation]</td>
  </tr>
  <tr>
    <td>HTML-weblink til at tilgå den virtuelle lokation</td>
    <td></td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
  </tr>
</table>

### Dokument (klasse)
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://xmlns.com/foaf/0.1/Document</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>Dokument</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Et dokument</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Kommentar</td>
    <td>Document-klassen repræsenterer de ting, der, bredt opfattet, er 'dokumenter'</td>
  </tr>
</table>

Kontaktformen adresse beskrives I kapitlet ‘Lokation og adresse’.
Kvalificeret kontaktinformation
 
## Kvalificeret kontaktinformation (klasse)

(indsæt billede)

##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>https://data.gov.dk/model/core/organisation/extension/-QualifiedContactInformation</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>kvalificeret kontaktinformation</td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>Information om kontaktmetode samt hvilke muligheder og begrænsninger der er ved brug af den pågældende kontaktmetode.</td>
  </tr>
</table>

##### _Profilens kontekstrestriktioner og annotationer_ 
<table>
  <tr>
    <td>Alternativ term</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]</td>
  </tr>
  <tr>
    <td>kontaktpunkt</td>
    <td></td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]</td>
  </tr>
  <tr>
    <td>Beskriver de forskellige kontaktformer, der er tilgængelige for Organisationer, Organisationsenheder og Organisationsmedlemmer</td>
    <td></td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>Kan omhandle fysiske steder som adresser, lokaler, men også virtuelle som sociale medier, email, DigitalPost mv.</td>
  </tr>
  <tr>
    <td>Eksempel</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>- fysisk adresse<br>- elektronisk adresse<br>- email</td>
  </tr>
</table>

#### værdi
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://www.w3.org/1999/02/22-rdf-syntax-ns#value</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>værdi</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Idiomatisk egenskab brugt til strukturerede værdier.</td>
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

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Anvendelsesnote</td>
    <td>Værdien eller indholdet af den specifikke kontaktform.</td>
  </tr>
  <tr>
    <td>Eksempel</td>
    <td>Hvis det valgte emne fra ’ovx:ContactForm’ er valgt til ’Telefon’ kan værdien være ’12 34 56 78’.</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>ovx:QualifiedContactInformation</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>rdfs:Literal</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>1 - 1</td>
  </tr>
</table>

#### kontaktemne
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>https://data.gov.dk/model/core/organisation/extension/contactSubject</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>kontaktemne</td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>Emne kontaktfmetoden er velegnet til at få information om eller på anden måde få håndteret.</td>
  </tr>
  <tr>
    <td>Profil-restriktioner og annotationer</td>
    <td></td>
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

#### bemærkning
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://www.w3.org/1999/02/22-rdf-syntax-ns#comment</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>kommentar</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>En beskrivelse af subjekt ressourcen.</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Term</td>
    <td>bemærkning</td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>beskriver supplerende forhold omkring den enkelte type af kontakt</td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>anvendes til at beskrive regler og principper for anvendelse af den enkelte kontaktform</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>Giver mulighed for at angive særlige forhold, afvigelser eller andet relevant information der knytter sig til den enkelte kontakttype.</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>Der kan være regler/principper som gælder for samtlige kontakttyper, men der kan også være særlige politikker der kun gør sig gældende i forhold til en specifik kontakttype.</td>
  </tr>
  <tr>
    <td>Anvendelsesnote</td>
    <td>Bemærkninger vedrørende kontaktinformationen</td>
  </tr>
  <tr>
    <td>Eksempel</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>Benyt indgangen i parkeringskælderen</td>
  </tr>
  <tr>
    <td>Eksempel</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>- email besvares inden for 5 hverdage.</td>
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

#### type
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://purl.org/dc/terms/type</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>type</td>
  </tr>
  <tr>
    <td>Beskrivelse</td>
    <td>Anbefalet bedste praksis er at bruge et kontrolleret ordforråd, såsom DCMI Type Vocabulary [DCMITYPE]. For at beskrive ressourcens filformat, fysiske medium eller dimensioner skal du bruge Format-elementet.</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Ressourcens art eller genre.</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>rdfs:Resource</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>rdfs:Class</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>anvendes til at klassificere de forskellige typer af kontaktpunkter</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>omhandler fx fysiske steder som adresser, lokaler, men også virtuelle som sociale medier, email, DigitalPost mv.</td>
  </tr>
  <tr>
    <td>Anvendelsesnote</td>
    <td>Udpeger typen af kontaktform</td>
  </tr>
  <tr>
    <td>Eksempel</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>- hovedtelefonnummer<br>- emailadresse<br>- digitalPostadresse<br>- vareindlevering<br>- besøgsadresse<br>- fakturaadresse-EAN<br>- fakturaadresse-post<br>- ...</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>ovx:QualifiedContactInformation</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>ovx:ContactForm</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>1 - 1</td>
  </tr>
</table>

### adgangsrettighed
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://purl.org/dc/terms/accessRights</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>adgangsrettighed</td>
  </tr>
  <tr>
    <td>Beskrivelse</td>
    <td>Adgangsrettigheder kan omfatte oplysninger om adgang eller begrænsninger baseret på privatliv, sikkerhed eller andre politikker.</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Oplysninger om, hvem der kan få adgang til ressourcen eller en indikation af dens sikkerhedsstatus.</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>dct:RightsStatement</td>
  </tr>
  <tr>
    <td>Underegenskab af</td>
    <td>dct:rights</td>
  </tr>
</table>


##### _Adgangsrettighed (klasse)_
Autoritetstabellen for adgangsrettigheder er et kontrolleret ordforråd, der viser adgangsrettigheder eller begrænsninger til ressourcer. Det er designet til, men ikke begrænset til, DCAT-beskrivelser af datasæt. Denne myndighedstabel vedligeholdes af Publications Office of the European Union på EU Vocabularies-webstedet.

http://publications.europa.eu/resource/authority/access-right 

##### _Vokabular-definition og beskrivelser_
URI	http://purl.org/dc/terms/RightsStatement
Term	Rettighedserklæring
Kommentar	En erklæring om de intellektuelle ejendomsrettigheder (IPR) i eller over en ressource, et juridisk dokument, der giver officiel tilladelse til at gøre noget med en ressource, eller en erklæring om adgangsrettigheder.
##### _Profil-restriktioner og annotationer_

### Kontaktform (klasse)
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>https://data.gov.dk/model/core/organisation/extension/ContactForm</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>Kontaktform</td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>Klassifikation indeholdende mulige kontaktformer.</td>
  </tr>
  <tr>
    <td>Eksempel</td>
    <td>Typer kan være:
      <ul>
        <li>Adresse
          <ul>
            <li>Besøgsadresse</li>
            <li>Postadresse</li>
            <li>Aktivitetsadresse</li>
            <li>Vareindlevering</li>
          </ul>
        </li>
        <li>E-mail
          <ul>
            <li>Forretningsmail</li>
            <li>Privat mail</li>
          </ul>
        </li>
        <li>Faxnummer</li>
        <li>Telefon</li>
        <li>Webside</li>
      </ul>
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
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>anvendes til at klassificere de forskellige typer af kontaktpunkter</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>omhandler fx fysiske steder som adresser, lokaler, men også virtuelle som sociale medier, email, DigitalPost mv.</td>
  </tr>
  <tr>
    <td>Eksempel</td>
    <td>[fra informationsmodel (klassen Kontaktinformation)]<br>- hovedtelefonnummer<br>- emailadresse<br>- digitalPostadresse<br>- vareindlevering<br>- besøgsadresse<br>- fakturaadresse-EAN<br>- fakturaadresse-post<br>- ...</td>
  </tr>
</table>

#### timer tilgængelige
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>https://data.gov.dk/model/core/organisation/extension/hoursAvailable</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>timer tilgængelige</td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>Anvendes til at beskrive åbningstider for kontaktformen</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>ovx:QualifiedContactInformation</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:OpeningHoursSpecification</td>
  </tr>
  <tr>
    <td>Profil-restriktioner og annotationer</td>
    <td></td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>0 - *</td>
  </tr>
</table>

### Specifikation af åbningstider (klasse)
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/OpeningHoursSpecification</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>Specifikation af åbningstider</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>En struktureret værdi, der giver information om åbningstiderne for et sted eller en bestemt tjeneste inde på et sted. Stedet er åbent, hvis egenskaben ’opens’ er angivet og lukket ellers. Hvis værdien for egenskaben ’closes’ er mindre end værdien for ’opens’ egenskaben, så antages timeintervallet at strække sig over den næste dag.</td>
  </tr>
  <tr>
    <td>Underklasse af</td>
    <td>schema:StructuredValue</td>
  </tr>
</table>

##### _Profilens kontekstrestriktioner og annotationer_ 
<table>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Åbningstid)]<br>giver information om åbningstider som en del af beskrivelsen for en kontaktoplysning</td>
  </tr>
</table>

#### åbner
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/opens</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>åbner</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Stedets eller tjenestens åbningstid på den eller de givne dag(e) i ugen.</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:OpeningHoursSpecification</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:Time</td>
  </tr>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Åbningstid)]<br>det tidspunkt lokationen eller tjenesten åbner på den eller de angivne ugedage</td>
  </tr>
  <tr>
    <td>Anvendelsesnote</td>
    <td>Åbningstid for den kontakt der repræsenteres i den kvalificerede kontaktinformation</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>1 - 1</td>
  </tr>
</table>

#### lukker
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/closes</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>lukker</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Stedets eller tjenestens lukketid på den eller de givne dag(e) i ugen.</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:OpeningHoursSpecification</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:Time</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Åbningstid)]<br>det tidspunkt lokationen eller tjenesten lukker på den eller de angivne ugedage</td>
  </tr>
  <tr>
    <td>Anvendelsesnote</td>
    <td>Lukketid for den kontakt der repræsenteres i den kvalificerede kontaktinformation</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:OpeningHoursSpecification</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>xsd:time</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>1 - 1</td>
  </tr>
</table>

#### gælder fra
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/validFrom</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>gælder fra</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Den dato, hvor varen bliver gyldig.</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:Permit eller schema:Certification eller schema:MonetaryAmount eller schema:Offer eller schema:OpeningHoursSpecification eller schema:LocationFeatureSpecification eller schema:Demand eller schema:PriceSpecification</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:DateTime eller schema:Date</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Anvendelsesnote</td>
    <td>Den dato, hvor den kvalificerede kontaktinformation bliver gyldig.</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>xsd:dateTime</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>0 - 1</td>
  </tr>
</table>

#### gælder indtil
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/validThrough</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>gælder indtil</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:PriceSpecification eller schema:MonetaryAmount eller schema:JobPosting eller schema:Offer eller schema:OpeningHoursSpecification eller schema:LocationFeatureSpecification eller schema:Demand</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:DateTime eller schema:Date</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_ 
<table>
  <tr>
    <td>Anvendelsesnote</td>
    <td>Den dato, hvor den kvalificerede kontaktinformation bliver ugyldig.</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>xsd:dateTime</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>0 - 1</td>
  </tr>
</table>

#### ugedag
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/dayOfWeek</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>ugedag</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Den ugedag, som disse åbningstider er gældende for.</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:OpeningHoursSpecification eller schema:EducationalOccupationalProgram</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:DayOfWeek eller schema:Text eller schema:URL eller schema:Role</td>
  </tr>
</table>

##### _Profil-restriktioner og annotationer_
<table>
  <tr>
    <td>Definition</td>
    <td>[fra informationsmodel (klassen Åbningstid)]<br>bestemt dag i ugen</td>
  </tr>
  <tr>
    <td>Domæne</td>
    <td>schema:OpeningHoursSpecification</td>
  </tr>
  <tr>
    <td>Udfaldsrum</td>
    <td>schema:DayOfWeek</td>
  </tr>
  <tr>
    <td>Multiplicitet</td>
    <td>1 - 1</td>
  </tr>
</table>

### Ugedag (klasse)
##### _Vokabular-definition og beskrivelser_
<table>
  <tr>
    <td>URI</td>
    <td>http://schema.org/DayOfWeek</td>
  </tr>
  <tr>
    <td>Term</td>
    <td>Ugedag</td>
  </tr>
  <tr>
    <td>Kommentar</td>
    <td>Ugedagen, bruges eksempelvis til at angive, hvilken dag åbningstiderne for en OpeningHoursSpecification refererer til. Oprindeligt blev URLer fra ’GoodRelations’ brugt (til ‘Monday’, ‘Tuesday’, ’Wednesday’, ’Thursday’ ’Friday’, ’Saturday’, ’Sunday’ plus en særlig post til ’PublicHolidays’; disse er nu blevet integreret direkte i schema.org.</td>
  </tr>
  <tr>
    <td>Underklasse af</td>
    <td>schema:Enumeration</td>
  </tr>
</table>

##### _Profilens kontekstrestriktioner og annotationer_ 
<table>
  <tr>
    <td>Anvendelsesnote</td>
    <td>Enumeration bestående af: <br><br>Friday<br>Monday<br>PublicHolidays<br>Saturday<br>Sunday<br>Thursday<br>Tuesday<br>Wednesday</td>
  </tr>
</table>


