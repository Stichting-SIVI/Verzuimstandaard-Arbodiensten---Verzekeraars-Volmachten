**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Basistransactie Verzuim*

Functional message: ***Aanvraag preventieve diensten verzekeraar 2020***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

1 juli 2020

Summary

Bericht algemeen 1..1, R

Werkgever 1..\*, R

1 Communicatie 0..9, O

1 Contactpersoon 0..9, O

2 Communicatie 1..9, R

1 Werknemer 1..\*, R

2 Partner 0..1, O

2 Straatadres Nederland 0..9, O

2 Straatadres Buitenland 0..9, O

2 Communicatie 0..9, O

2 Dienstverband 1..99, R

3 Preventieve dienst 0..9, O

4 Contactpersoon 0..9, O

5 Communicatie 1..9, R

3 Arbeidsrelatie 0..1, O

BERICHT ALGEMEEN 1..1, R

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code R an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00602 Aanvraag preventieve dienst Verzekeraar --\> Arbodienst

**Versienummer bericht, code R an..5**

*xml tag:* VnrBrCd

*code list:* Versienummer bericht (subset selected)

00001 Versienummer 1

**<u>Aanmaakdatum</u>**

**Aanmaakdatum bericht R an10**

*xml tag:* AandatBr

**Aanmaaktijd bericht R an8**

*xml tag:* AantijdBr

**<u>Inzender</u>**

**Identificatie inzender R an..40**

*xml tag:* IdInzndr

Bilateraal afgesproken codering betreffende de inzender van het bericht.

**Gebruikt softwarepakket R an..35**

*xml tag:* GebrSwPakket

Beschrijving van het softwarepakket dat de aanleveraar heeft gebruikt
voor de vervaardiging van het bericht.

**<u>Ontvanger</u>**

**Identificatie ontvanger R an..40**

*xml tag:* IdOntvngr

Bilateraal afgesproken codering betreffende de ontvanger
(eindbestemming) van het bericht.

**<u>Berichtreferentie</u>**

**Berichtreferentienummer R an..512**

*xml tag:* Berrefnr

**<u>Testindicatie</u>**

**Test J/N R a1**

*xml tag:* TestJN

Geeft aan of het een testbericht betreft.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

**<u>Ontvangstbevestiging</u>**

**Ontvangstbevestiging gewenst J/N R a1**

*xml tag:* OntvngstbevJN

Geeft aan of de inzender van het bericht een ontvangstbevestiging wenst.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

WERKGEVER 1..\*, R

*WERKGEVER*

*xml tag:* Wrkgvr

Bij het beschrijven van de kenmerken van de Werkgever wordt in een
aantal gevallen de term Inhoudingsplichtige gebruikt.

**<u>Handelsnaam</u>**

**Handelsnaam organisatie R an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

**<u>Kamer van Koophandel</u>**

**Inschrijvingsnummer Kamer van Koophandel O n..8**

*xml tag:* InschrijvingsnrKvK

Een identificerend nummer dat de Kamer van Koophandel toekent aan
ondernemingen zoals vermeld in de Handelsregisterwet.

Bron: SUWI Gegevens Register

**Vestigingsnummer O n..12**

*xml tag:* VestigingsnrHandelsregister

Een identificerend nummer voor een vestiging in het Handelsregister.

Norminstantie: Handelsregister

**<u>Identificatie bij de Arbo-dienst</u>**

**Identificatie werkgever bij Arbo-dienst R an..40**

*xml tag:* IdWrkgvrArbdnst

De identificatiecode die de arbodienst heeft aangeleverd aan de
werkgever waardoor de werkgever wordt onderscheden van andere werkgevers
in de administratie van de arbodienst.

**Aansluitnummer gegevensuitwisseling Arbodienst R an..70**

*xml tag:* AansltnrGeguitwlngArbdnst

Het aansluitnummer voor de gegevensuitwisseling dat de arbodienst heeft
aangeleverd aan de werkgever waardoor de werkgever wordt onderscheden
van andere werkgevers in de administratie van de arbodienst.

**<u>Identificatie bij verzekeraar</u>**

**Identificatie werkgever bij verzekeraar O an..40**

*xml tag:* IDWrkgvrVerzekeraar

**<u>Loonbelasting / loonheffingen</u>**

**Loonheffingennummer R an..12**

*xml tag:* Lhnr

Een door de Belastingdienst toegekende identificatie voor de
administratieve eenheid waaronder de werkgever bekend is en
loonheffingen afdraagt.

COMMUNICATIE 0..9, O

*werkgever - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**<u>Soort communicatie</u>**

**Soort communicatie, code R an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

06 Zakelijk e-mail adres

08 Zakelijk vaste telefoon

10 Zakelijk mobiele telefoon

**<u>Nummer</u>**

**Nummer/adres communicatie R an..512**

*xml tag:* NrCom

CONTACTPERSOON 0..9, O

*werkgever - CONTACTPERSOON*

*xml tag:* Cntprsn

**<u>Identificerende gegevens</u>**

**Identificatie Werknemer O an..40**

*xml tag:* IdWrknmr

**Personeelsnummer O an..35**

*xml tag:* Persnr

De code waarmee de natuurlijk persoon in de loonadministratie van de
inhoudingsplichtige bekend is.

**<u>Naamgegevens</u>**

**Achternaam/Achternamen R an..200**

*xml tag:* Achternaam

Achternaam/achternamen inclusief voorvoegsel(s).

Mensen die getrouwd zijn of een geregistreerd partnerschap zijn
aangegaan, kunnen in het dagelijks leven de achternaam van hun partner
combineren met hun eigen achternaam. Aan een gecombineerde achternaam
alléén is niet te zien of het om een man of een vrouw gaat, en ook niet
welke van de twee achternamen de geboortenaam is en welke de
'aangetrouwde'. Alle combinaties zijn namelijk denkbaar. Stel dat de
heer of mevrouw Oudewater getrouwd is met de heer of mevrouw Simons, dan
kunnen zij elk in het dagelijks leven naar eigen inzicht kiezen uit een
van de volgende namen:

\- Simons

\- Oudewater

\- Simons-Oudewater

\- Oudewater-Simons

Bron: Genootschap Onze Taal

**Voorletters O a..6**

*xml tag:* Voorl

De verzameling letters die wordt gevormd door de eerste letter van alle
in volgorde voorkomende voornamen.

Bestaan uit hoofdletters, zijn aaneengesloten en bevatten geen punten.
Alleen alfabetische tekens zijn toegestaan.

Bron: Loonaangifte.

**Roepnaam O a..35**

*xml tag:* Roepnaam

Voornaam waarmee iemand wordt aangesproken.

**<u>Overige gegevens</u>**

**Geslachtsaanduiding, code O an1**

*xml tag:* GslchtCd

De sekse van een persoon, zoals bij de geboorte formeel vastgesteld of
nadien formeel gewijzigd.

Bron: NEN 1888: 2002 - Geslacht

*code list:* Geslacht (all selected)

M Man

O Onbekend/niet gespecificeerd

V Vrouw

**Rol contactpersoon, code R an2**

*xml tag:* RolCntprsnCd

*code list:* Rol contactpersoon (all selected)

01 Leidinggevende

02 Casemanager

03 Medewerker P&O

04 Vervangend leidinggevende

05 Algemeen contactpersoon

COMMUNICATIE 1..9, R

*werkgever - contactpersoon - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**<u>Soort communicatie</u>**

**Soort communicatie, code R an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

06 Zakelijk e-mail adres

08 Zakelijk vaste telefoon

10 Zakelijk mobiele telefoon

**<u>Nummer</u>**

**Nummer/adres communicatie R an..512**

*xml tag:* NrCom

WERKNEMER 1..\*, R

*werkgever - WERKNEMER*

*xml tag:* Wrknmr

Een werknemer is de natuurlijke persoon met wie een inkomstenverhouding
binnen de loonadministratie bestaat.

**<u>Identificerende gegevens</u>**

**Geboortedatum R an10**

*xml tag:* Gebdat

Datum waarop de natuurlijke persoon is geboren.

Als de geboortedatum niet bekend is moet een bestaanbare geboortedatum
worden ingevuld. Hierbij moet de volgende werkwijze worden gehanteerd:

1\. Als de dag, maand en jaar niet bekend zijn moet u het jaar schatten
en voor de dag en maand 01-07 invullen.

2\. Als de dag en de maand niet bekend zijn: 01-07-jaar

3\. Als de dag niet bekend is: 16-maand-jaar.

Bron: Loonaangifte.

**<u>Naamgegevens</u>**

**Significant deel van de achternaam R an..200**

*xml tag:* SignNm

De achternaam zonder voorvoegsels.

Het betreft de geboortenaam van de persoon (en niet van de partner)
zonder voorvoegsels, zoals opgenomen op het identiteitsbewijs.
Toevoegingen ten behoeve van de eigen administratie zijn niet
toegestaan.

Bron: Loonaangifte.

**Voorletters R a..6**

*xml tag:* Voorl

De verzameling letters die wordt gevormd door de eerste letter van alle
in volgorde voorkomende voornamen.

Bestaan uit hoofdletters, zijn aaneengesloten en bevatten geen punten.
Alleen alfabetische tekens zijn toegestaan.

Bron: Loonaangifte.

**Voorvoegsels O a..10**

*xml tag:* Voorv

De verzameling van één of meer voorzetsels en/of lidwoorden die aan het
significante deel van de achternaam vooraf gaat en daarmee gezamenlijk
de achternaam vormt.

Bron: Loonaangifte.

**Roepnaam O a..35**

*xml tag:* Roepnaam

Voornaam waarmee iemand wordt aangesproken.

**<u>Titulatuur</u>**

**Titulatuur voor de naam O an..35**

*xml tag:* TitVNm

Dit betreft een of meer titels. Een titel is de beschermde, al dan niet
van overheidswege toegekende benaming waarop een persoon krachtens zijn
opleiding, adellijke afkomst, functie of benoeming recht heeft en
waarmee in de regel tevens een waardigheid, rang of maatschappelijke
positie wordt aangeduid.

Bron: NEN 1888: 2002 - Titel

**Titulatuur achter de naam O an..35**

*xml tag:* TitANm

Dit betreft een of meer titels. Een titel is de beschermde, al dan niet
van overheidswege toegekende benaming waarop een persoon krachtens zijn
opleiding, adellijke afkomst, functie of benoeming recht heeft en
waarmee in de regel tevens een waardigheid, rang of maatschappelijke
positie wordt aangeduid.

Bron: NEN 1888: 2002 - Titel

**<u>Naamvoorkeur</u>**

**Naamvoorkeur, code R an2**

*xml tag:* NmvrkrCd

Een aanduiding voor de wijze van aanschrijving.

*code list:* Naamvoorkeur (subset selected)

01 Eigen naam

02 Naam partner

03 Naam partner gevolgd door eigen naam

04 Eigen naam gevolgd door naam partner

**<u>Overige gegevens</u>**

**Geslachtsaanduiding, code R an1**

*xml tag:* GslchtCd

De sekse van een persoon, zoals bij de geboorte formeel vastgesteld of
nadien formeel gewijzigd.

Bron: NEN 1888: 2002 - Geslacht

*code list:* Geslacht (all selected)

M Man

O Onbekend/niet gespecificeerd

V Vrouw

**<u>Identificatie</u>**

**Identificatie werknemer O an..40**

*xml tag:* IdWrknmr

Een unieke identificatie van de werknemer bij de werkgever. Een eenmaal
uitgegeven identificatie wordt niet hergebruikt.

PARTNER 0..1, O

*werkgever - werknemer - PARTNER*

*xml tag:* Prtnr

**<u>Naamgegevens</u>**

**Significant deel van de achternaam R an..200**

*xml tag:* SignNm

De achternaam zonder voorvoegsels.

Het betreft de geboortenaam van de persoon (en niet van de partner)
zonder voorvoegsels, zoals opgenomen op het identiteitsbewijs.
Toevoegingen ten behoeve van de eigen administratie zijn niet
toegestaan.

Bron: Loonaangifte.

**Voorvoegsels O a..10**

*xml tag:* Voorv

De verzameling van één of meer voorzetsels en/of lidwoorden die aan het
significante deel van de achternaam vooraf gaat en daarmee gezamenlijk
de achternaam vormt.

Bron: Loonaangifte.

STRAATADRES NEDERLAND 0..9, O

*werkgever - werknemer - STRAATADRES NEDERLAND*

*xml tag:* StrAdrNl

Een adres in Nederland dat wordt bepaald aan de hand van straatnaam en
huisnummer.

**<u>Soort adres</u>**

**Soort adres, code R an2**

*xml tag:* SrtAdrsCd

*code list:* Soort adres (subset selected)

01 Woonadres, verblijfadres of vestigingsadres

02 Postadres cq correspondentie adres

04 Tijdelijk adres

**<u>Periode geldig</u>**

**Ingangsdatum O an10**

*xml tag:* Ingdat

**Einddatum O an10**

*xml tag:* Enddat

**<u>Generiek voor adres</u>**

**Postcode R an6**

*xml tag:* Pc

De officiële Nederlandse codering, bestaande uit een numerieke
woonplaatscode een alfabetische lettercode.

Norminstantie: NEN 5825 (Postcode)

**Woonplaatsnaam R an..24**

*xml tag:* Wnpl

De door de gemeente vastgestelde naam van een woonplaats.

Norm(instantie): NEN 5825 (Woonplaatsnaam)

**<u>Specifiek voor straatadres Nederland</u>**

**Straatnaam\_ O an..80**

*xml tag:* StraatLang

De officiële door de gemeente vastgestelde naam van een straat.

Als de officiële straatnaam echter langer is dan 24 posities dan mag

deze ingekort volgens de specificaties van de BOCO-norm.

Norm(instantie)

NEN 5825 (Straatnaam)

**Huisnummer R n..5**

*xml tag:* Huisnr

De numerieke aanduiding zoals deze door de gemeente aan het object is
toegekend.

Norminstantie: NEN 5825 (Huisnummer)

**Huisnummertoevoeging O an..4**

*xml tag:* HuisToev

De alfanumerieke aanduiding achter huisnummer, zoals toegekend door de
gemeente.

Norminstantie: NEN 5825 (Huisnummertoevoeging)

STRAATADRES BUITENLAND 0..9, O

*werkgever - werknemer - STRAATADRES BUITENLAND*

*xml tag:* StrAdrBl

Een adres in het buitenland dat wordt bepaald aan de hand van straatnaam
en huisnummer.

**<u>Soort adres</u>**

**Soort adres, code R an2**

*xml tag:* SrtAdrsCd

*code list:* Soort adres (subset selected)

01 Woonadres, verblijfadres of vestigingsadres

02 Postadres cq correspondentie adres

04 Tijdelijk adres

**<u>Periode geldig</u>**

**Ingangsdatum O an10**

*xml tag:* Ingdat

**Einddatum O an10**

*xml tag:* Enddat

**<u>Generiek voor adres buitenland</u>**

**Locatieomschrijving buitenland O an..35**

*xml tag:* LocomsBtl

Een nadere aanduiding bij een buitenlands adres.

Bron: SUWI

**Postcode buitenland O an..9**

*xml tag:* PcBtl

Een door de buitenlandse postdienst vastgestelde codering voor een adres
in het buitenland.

Bron: SUWI

**Woonplaatsnaam buitenland R an..24**

*xml tag:* WnplBtl

De naam van een woonplaats in het buitenland.

Bron: SUWI

**Regionaam buitenland O an..24**

*xml tag:* RegBtl

De naam van een gebiedsdeel binnen een land.

Bron: SUWI

**Land, code R a2**

*xml tag:* LandCd

De code van een huidig land of gebiedsdeel conform ISO 3166.

Norminstantie: ISO 3166 (Entity, Alpha-2 code)

*code list:* ISO landcode (all selected)

*The codes of this codelist are documented in a separate document*

**Landnaam O an..40**

*xml tag:* Landnm

De naam van een land of een gebiedsdeel.

Bron: SUWI

**<u>Specifiek voor straatadres buitenland</u>**

**Straatnaam\_ O an..80**

*xml tag:* StraatLang

**Huisnummer buitenland R an..9**

*xml tag:* HuisnrBtl

COMMUNICATIE 0..9, O

*werkgever - werknemer - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**<u>Soort communicatie</u>**

**Soort communicatie, code R an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

05 Privé e-mail adres

06 Zakelijk e-mail adres

07 Privé vaste telefoon

08 Zakelijk vaste telefoon

09 Privé mobiele telefoon

10 Zakelijk mobiele telefoon

**<u>Nummer</u>**

**Nummer/adres communicatie R an..512**

*xml tag:* NrCom

DIENSTVERBAND 1..99, R

*werkgever - werknemer - DIENSTVERBAND*

*xml tag:* Dnstvbnd

**<u>Identificatie</u>**

**Identificatie dienstverband O an..40**

*xml tag:* IdDnstvbnd

Unieke code voor het dienstverband van de werknemer.

**<u>Personeelsnummer behorende bij het dienstverband</u>**

**Personeelsnummer O an..35**

*xml tag:* PersNr

De code waarmee de natuurlijk persoon in de administratie van de
inhoudingsplichtige bekend is.

Bron: Loonaangifte.

**<u>Contractnummer</u>**

**Contractnummer bij Arbo-dienst O an..40**

*xml tag:* CntrnrArbdnst

Het door de Arbo-dienst gebruikte contractnummer en waaronder de
desbetreffende werknemer met zijn dienstverband valt.

**<u>Beschrijving werkzaamheden</u>**

**Soort dienstverband, code O an2**

*xml tag:* SrtDnstvbndCd

Bron: ArboNed (2006)

*code list:* Soort dienstverband (all selected)

01 Normale arbeidsovereenkomst

02 Aanneming werk

03 Vertegenwoordiger

04 WSW'er

05 Stagiair

06 Thuiswerker

07 Uitzendkracht

08 Musicus / artiest /beroepssporter

09 Persoonlijke arbeid tegen beloning

10 Maatschapsvisser

11 Bestuurder van een cooperatieve vereniging

Vereniging met werknemers zelfbestuur.

12 Oproep / invalkracht

13 Vakantiewerk

14 Dienstplichtig militair

15 Ambtenaar / ABP-er

16 Deelvisser

17 Gemoedsbezwaarde

18 Topsporter

19 65-plusser

**Functiecode O an..15**

*xml tag:* Fnctcd

De code van de functie zoals die bij de klant bekend is of zoals die is
overeengekomen met de Arbo-dienst.

**Naam functie O an..35**

*xml tag:* NmFnct

**<u>Locatie</u>**

**Naam organisatie-eenheid O an..70**

*xml tag:* NmOrgeenh

**Organisatie-eenheid, code R an..70**

*xml tag:* OrgeenhCd

De code van de organisatie-eenheid, zoals die bij de klant bekend is of
zoals die is overeengekomen met de Arbo-dienst.

**Onderdeel van organisatieeenheid, code O an..70**

*xml tag:* OndOrgeenhCd

Iedere organisatie-eenheid kan weer onderdeel zijn van een andere
organisatie-eenheid.

**Onderdeel van organisatie-eenheid, naam O an..70**

*xml tag:* OndOrgeenhCdNm

Deze naam hoort bij Onderdeel van organisatie-eenheid, code

**Postcode standplaats O an..9**

*xml tag:* PcStandplts

Postcode van de standplaats waar de werknemer is tewerkgesteld.

**Verdeling, code O an..35**

*xml tag:* VrdlngCd

Bilateraal afgesproken codering ten behoeve van de verdeling van het
werk.

**<u>Gegevens over arbeidsovereenkomst</u>**

**Code contract onbepaalde / bepaalde tijd O an1**

*xml tag:* CdBepTd

Code die aangeeft of het arbeidscontract voor bepaalde of onbepaalde
tijd geldig is.

Bron: Loonaangifte.

*code list:* Code contract onbepaalde / bepaalde tijd (all selected)

B Bepaalde tijd

O Onbepaalde tijd

**<u>Beschrijving aantal uren e.d.</u>**

**Aantal contracturen per week O n..5,2**

*xml tag:* AantCtrcturenPWk

Het tussen de werkgever en werknemer vast overeengekomen aantal uren per
week zoals opgenomen in of af te leiden uit de CAO of individuele
arbeidsovereenkomst.

Bron: Loonaangifte

**Soort variabele werktijden, code O an2**

*xml tag:* SrtVarWrktdCd

Bron:

Berekening van ziekteverzuim

NVS Standaard voor verzuimregistratie

Nationale Verzuimstatistiek

November 2004

*code list:* Soort variabele werktijden (all selected)

01 Regelmatige dienst (eventueel met verschoven uren)

02 Tweeploegendienst

03 Meer dan tweeploegendiensten

04 Onregelmatige dienst (geen ploegendienst)

PREVENTIEVE DIENST 0..9, O

*werkgever - werknemer - dienstverband - PREVENTIEVE DIENST*

*xml tag:* PrevDienst

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**Ingangsdatum mutatie prev. dienst R an10**

*xml tag:* IngdatMutPrev

Datum van versturen nieuwe aanvraag of mutatie van een aanvraag
preventieve dienst.

**<u>Identificatie</u>**

**Identificatie preventieve dienst R an..40**

*xml tag:* IdPrevDienst

**<u>Preventieve dienst</u>**

**Preventieve dienst, code R an2**

*xml tag:* PreventDienst

*code list:* Preventieve dienst (subset selected)

01 Preventief spreekuur

02 Preventief medisch onderzoek (PMO)

03 Aanstellingskeuring

04 Periodieke keuring, (o.a. PAGO)

05 Chauffeurskeuring

06 Rijbewijskeuring

07 Binnen-/zeevaartkeuring

08 Duikkeuring

09 Offshorekeuring

10 Ademluchtkeuring

11 Asbestkeuring

12 Bodemsaneringskeuring

13 Stralingskeuring

14 Brandweerkeuring

15 Bloedonderzoek

16 Vaccinatie

17 Werken op hoogte

18 Beroepskeuring

99 Overig

**Peventieve dienst toevoeging O an..70**

*xml tag:* PevDienstToev

Aanvulling op Preventieve dienst, code

CONTACTPERSOON 0..9, O

*werkgever - werknemer - dienstverband - preventieve dienst -
CONTACTPERSOON*

*xml tag:* Cntprsn

**<u>Identificerende gegevens</u>**

**Identificatie Werknemer O an..40**

*xml tag:* IdWrknmr

**Personeelsnummer O an..35**

*xml tag:* Persnr

De code waarmee de natuurlijk persoon in de loonadministratie van de
inhoudingsplichtige bekend is.

**<u>Naamgegevens</u>**

**Achternaam/Achternamen R an..200**

*xml tag:* Achternaam

Achternaam/achternamen inclusief voorvoegsel(s).

Mensen die getrouwd zijn of een geregistreerd partnerschap zijn
aangegaan, kunnen in het dagelijks leven de achternaam van hun partner
combineren met hun eigen achternaam. Aan een gecombineerde achternaam
alléén is niet te zien of het om een man of een vrouw gaat, en ook niet
welke van de twee achternamen de geboortenaam is en welke de
'aangetrouwde'. Alle combinaties zijn namelijk denkbaar. Stel dat de
heer of mevrouw Oudewater getrouwd is met de heer of mevrouw Simons, dan
kunnen zij elk in het dagelijks leven naar eigen inzicht kiezen uit een
van de volgende namen:

\- Simons

\- Oudewater

\- Simons-Oudewater

\- Oudewater-Simons

Bron: Genootschap Onze Taal

**Voorletters O a..6**

*xml tag:* Voorl

De verzameling letters die wordt gevormd door de eerste letter van alle
in volgorde voorkomende voornamen.

Bestaan uit hoofdletters, zijn aaneengesloten en bevatten geen punten.
Alleen alfabetische tekens zijn toegestaan.

Bron: Loonaangifte.

**Roepnaam O a..35**

*xml tag:* Roepnaam

Voornaam waarmee iemand wordt aangesproken.

**<u>Overige gegevens</u>**

**Geslachtsaanduiding, code O an1**

*xml tag:* GslchtCd

De sekse van een persoon, zoals bij de geboorte formeel vastgesteld of
nadien formeel gewijzigd.

Bron: NEN 1888: 2002 - Geslacht

*code list:* Geslacht (all selected)

M Man

O Onbekend/niet gespecificeerd

V Vrouw

**Rol contactpersoon, code R an2**

*xml tag:* RolCntprsnCd

*code list:* Rol contactpersoon (all selected)

01 Leidinggevende

02 Casemanager

03 Medewerker P&O

04 Vervangend leidinggevende

05 Algemeen contactpersoon

COMMUNICATIE 1..9, R

*werkgever - werknemer - dienstverband - preventieve dienst -
contactpersoon - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**<u>Soort communicatie</u>**

**Soort communicatie, code R an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

06 Zakelijk e-mail adres

08 Zakelijk vaste telefoon

10 Zakelijk mobiele telefoon

**<u>Nummer</u>**

**Nummer/adres communicatie R an..512**

*xml tag:* NrCom

ARBEIDSRELATIE 0..1, O

*werkgever - werknemer - dienstverband - ARBEIDSRELATIE*

*xml tag:* Arbeidsrelatie

De betrekking tussen werkgever en werknemer die ontstaat bij loonarbeid
na afsluiting van een arbeidsovereenkomst.

Dit wordt ook wel aanstelling genoemd.

**<u>Identificerende gegevens arbeidsrelatie</u>**

**Identificatie arbeidsrelatie R an..40**

*xml tag:* IdArbeidsrelatie

**Personeelsnummer O an..35**

*xml tag:* PersNr

De code waarmee de natuurlijk persoon in de administratie van de
inhoudingsplichtige bekend is.

Bron: Loonaangifte.

**<u>Data</u>**

**Ingangsdatum R an10**

*xml tag:* Ingdat

**<u>Uren per week</u>**

**Aantal contracturen per week R n..5,2**

*xml tag:* AantCtrcturenPWk

De formele arbeidsduur per week, zoals die is opgenomen in het contract
bij arbeidsverhouding/aanstelling.
