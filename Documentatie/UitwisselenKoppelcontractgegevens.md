**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Basis Arbodienst Verzekeraar*

Functional message: ***Uitwisselen koppel/contractgegevens 2020***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

1 juli 2020

Summary

Bericht algemeen 1..1, R

Verzekeraar/Volmacht 1..1, R

Arbodienst 1..1, R

Werkgever 1..\*, R

1 Personeelssterkte 0..999, O

1 Straatadres Nederland 0..9, O

1 Postbusadres Nederland 0..9, O

1 Straatadres Buitenland 0..\*, O

1 Postbusadres Buitenland 0..\*, O

1 Administratieve Eenheid 0..1, O

1 Organisatie eenheid 0..999, O

2 Personeelssterkte 0..\*, O

1 Arbocontract 0..9, O

2 Intermediair 0..1, O

3 Straatadres Nederland 0..\*, O

3 Communicatie 0..9, O

2 Dienstverlening 0..9, O

1 Verzekering/Dekking 0..99, O

2 Afspraken Uitwisseling Verzuimdata 0..9, O

1 Afspraken Uitwisseling Verzuimdata 0..9, O

1 Communicatie 0..9, O

1 Contactpersoon 0..\*, O

2 Communicatie 0..\*, O

BERICHT ALGEMEEN 1..1, R

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code R an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00700 Uitwisselen koppel/contractgegevens

**Versienummer bericht, code R an..5**

*xml tag:* VnrBrCd

*code list:* Versienummer bericht (subset selected)

00002 Versienummer 2

**<u>Functie bericht</u>**

**Functie bericht, code R an2**

*xml tag:* FunctieBrCd

*code list:* SIVI (all selected)

01 Koppelgegevens verzekeraar --\> arbodienst

02 Koppelgegevens arbodienst --\> verzekeraar

03 Contractdata werkgever - verzekeraar

04 Contractdata werkgever - arbodienst

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

**Berichtreferentienummer ingezonden bericht O an..512**

*xml tag:* BerrefnrIngzndnBer

Het referentienummer van het bericht waar het onderhavige bericht een
reactie op is.

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

**<u>Contractgegevens gewenst</u>**

**Contractgegevens gewenst J/N R a1**

*xml tag:* CntrctGegGewenstJN

Aanduiding van de zender van het bericht of het gewenst is dat de
ontvanger de contractgegevens retourneert.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

VERZEKERAAR/VOLMACHT 1..1, R

*VERZEKERAAR/VOLMACHT*

*xml tag:* VrzkrVolmacht

**<u>Handelsnaam</u>**

**Handelsnaam organisatie R an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

**<u>Identificerende gegevens</u>**

**Identificatie verzekeraar/volmacht, code R an..4**

*xml tag:* IdVrzkrVolmachtCd

Hiervoor wordt de POR-code gebruikt. Op dit moment wordt de POR-code
branchebreed gebruikt voor het uniek identificeren van bijna 700
verzekeraars/volmachten. Zie www.sivi.org.

*code list:* POR maatschappij aanduiding (all selected)

*The codes of this codelist are documented in a separate document*

ARBODIENST 1..1, R

*ARBODIENST*

*xml tag:* Arbdnst

**<u>Handelsnaam</u>**

**Handelsnaam organisatie O an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

**<u>Arbo-dienst</u>**

**Arbodienst, code R an3**

*xml tag:* ArbdnstCd

De lijst met codes van gecertificeerde Arbodiensten is gepubliceerd op
de website van SIVI. Zie www.sivi.org.

*code list:* Code Arbodienst (all selected)

*The codes of this codelist are documented in a separate document*

WERKGEVER 1..\*, R

*WERKGEVER*

*xml tag:* Wrkgvr

Bij het beschrijven van de kenmerken van de Werkgever wordt in een
aantal gevallen de term Inhoudingsplichtige gebruikt.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

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

**Identificatie werkgever bij Arbo-dienst O an..40**

*xml tag:* IdWrkgvrArbdnst

De identificatiecode die de arbodienst heeft aangeleverd aan de
werkgever waardoor de werkgever wordt onderscheden van andere werkgevers
in de administratie van de arbodienst.

**Aansluitnummer gegevensuitwisseling Arbodienst O an..70**

*xml tag:* AansltnrGeguitwlngArbdnst

Het aansluitnummer voor de gegevensuitwisseling dat de arbodienst heeft
aangeleverd aan de werkgever waardoor de werkgever wordt onderscheden
van andere werkgevers in de administratie van de arbodienst.

**<u>Identificatie bij verzekeraar</u>**

**Identificatie werkgever bij verzekeraar O an..40**

*xml tag:* IDWrkgvrVerzekeraar

**<u>Identificatie bij UWV</u>**

**Identificatie werkgever bij UWV O an..40**

*xml tag:* IdWrkgvrUWV

De identificatie die het UWV heeft aangeleverd aan de werkgever

waardoor de werkgever wordt onderscheiden van andere werkgevers in de
administratie van het UWV.

**<u>Loonbelasting / loonheffingen</u>**

**Loonheffingennummer O an..12**

*xml tag:* Lhnr

Een door de Belastingdienst toegekende identificatie voor de
administratieve eenheid waaronder de werkgever bekend is en
loonheffingen afdraagt.

**<u>Codering organisatie-eenheid</u>**

**Organisatie-eenheid, code R an..70**

*xml tag:* OrgeenhCd

Bilateraal afgesproken codering van de organisatie-eenheid.

**<u>Eigenrisicodragerschap</u>**

**Identificatie verzekeraar ERD WGA, code O an..4**

*xml tag:* IdVrzkrWGACd

Hiervoor wordt de POR-code gebruikt. Zie www.sivi.org.

*code list:* POR maatschappij aanduiding (all selected)

*The codes of this codelist are documented in a separate document*

**Identificatie verzekeraar ERD ZW, code O an..4**

*xml tag:* IdVrzkrERDZWCd

Hiervoor wordt de POR-code gebruikt. Zie www.sivi.org.

*code list:* POR maatschappij aanduiding (all selected)

*The codes of this codelist are documented in a separate document*

**<u>Collectieve zorgverzekering</u>**

**Identificatie verzekeraar collectieve zorg, code O an..4**

*xml tag:* IdVrzkrCollectieveZorgCd

Hiervoor wordt de POR-code gebruikt. Zie www.sivi.org.

*code list:* POR maatschappij aanduiding (all selected)

*The codes of this codelist are documented in a separate document*

**<u>Sector waarin werkgever opereert</u>**

**Sector volgens SBI O n..5**

*xml tag:* SectorVolgensSBI

De sector waarin de werkgever opereert volgens de Standaard
Bedrijfsindeling (SBI) het Centraal Bureau voor de Statistiek van
Nederland.

PERSONEELSSTERKTE 0..999, O

*werkgever - PERSONEELSSTERKTE*

*xml tag:* Personeelssterkte

Gegevens met betrekking tot het aantal werknemers.

**<u>Datum waarop de Personeelssterkte is vastgesteld</u>**

**Peildatum personeelssterkte R an10**

*xml tag:* PeildatPersoneelssterkte

De datum waarop de personeelssterkte - in termen van aantallen
werknemers en FTE - is vastgesteld.

**Vorige peildatum personeelssterkte O an10**

*xml tag:* VorigePeildatPersoneelssterkte

**<u>Gegevens over de personeelssterkte</u>**

**Aantal werknemers R n..7**

*xml tag:* AantWrknmrs

**Aantal werknemers in dienst sinds vorige peildatum O n..7**

*xml tag:* AantWrknmrsInDienstSindsVorigePeildat

**Aantal werknemers uit dienst sinds vorige peildatum O n..7**

*xml tag:* AantWrknmrsUitDienstSindsVorigePeildat

**Aantal nulurencontracten O n..7**

*xml tag:* AantalNulurencntrcten

**Aantal FTE O n..7**

*xml tag:* AantFTE

**Aantal vrouwelijke werknemers O n..5**

*xml tag:* AantVrouwelijkeWrknmrs

Het aantal vrouwelijke werknemers dat werkt bij de werkgever.

**Aantal vrouwelijke FTE O n..5**

*xml tag:* AantVrouwelijkeFTE

Het aantal vrouwelijke FTE dat werkt bij de werkgever.

**Aantal mannelijke werknemers O n..5**

*xml tag:* AantMannelijkeWrknmrs

Het aantal mannelijke werknemers dat werkt bij de werkgever.

**Aantal mannelijke FTE O n..5**

*xml tag:* AantMannelijkeFTE

Het aantal mannelijke FTE dat werkt bij de werkgever.

**Aantal uren FTE O n..3**

*xml tag:* AantUrenFTE

Aantal uren dat 1 FTE wordt geacht te werken in een werkweek.

STRAATADRES NEDERLAND 0..9, O

*werkgever - STRAATADRES NEDERLAND*

*xml tag:* StrAdrNl

Een adres in Nederland dat wordt bepaald aan de hand van straatnaam en
huisnummer.

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

**Woonplaatsnaam O an..24**

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

POSTBUSADRES NEDERLAND 0..9, O

*werkgever - POSTBUSADRES NEDERLAND*

*xml tag:* PbadrsNl

De gegevens van een postbusadres in Nederland.

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

**Woonplaatsnaam O an..24**

*xml tag:* Wnpl

De door de gemeente vastgestelde naam van een woonplaats.

Norm(instantie): NEN 5825 (Woonplaatsnaam)

**<u>Specifiek voor postbusadres</u>**

**Postbusnummer R n..5**

*xml tag:* Pbnr

De numerieke aanduiding zoals deze door de Nederlandse TPG Post is
vastgesteld voor postbusadressen.

Norminstantie: NEN 5825 (Postbusnummer)

STRAATADRES BUITENLAND 0..\*, O

*werkgever - STRAATADRES BUITENLAND*

*xml tag:* StrAdrBl

Een adres in het buitenland dat wordt bepaald aan de hand van straatnaam
en huisnummer.

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

**Huisnummer toevoeging buitenland O an..70**

*xml tag:* HuisnrToevBtl

POSTBUSADRES BUITENLAND 0..\*, O

*werkgever - POSTBUSADRES BUITENLAND*

*xml tag:*

Gegevens van een postbusadres in het buitenland.

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

**<u>Specifieke gegevens postbusadres buitenland</u>**

**Postbusnummer buitenland R an..7**

*xml tag:*

ADMINISTRATIEVE EENHEID 0..1, O

*werkgever - ADMINISTRATIEVE EENHEID*

*xml tag:* AdministratieveEenheid

Een door de Belastingdienst en UWV erkende organisatorische eenheid, die
door een inhoudingsplichtige wordt gevoerd ter naleving van diens
wettelijke verplichtingen met betrekking tot de loonheffingen. Een
inhoudingsplichtige kan meer dan één administratieve eenheid voeren. De
administratieve eenheden van een inhoudingsplichtige worden van elkaar
onderscheiden door hun subnummers.

Hoofdregel is dat voor een administratieve eenheid één aangiftetijdvak
en één op basis van de Wet Financiering Sociale Verzekeringen (WFSV)
onderkende sector (een deelverzameling van één of meer takken van
bedrijf of beroep of gedeelten daarvan) geldt.

In de volgende situaties is het echter mogelijk dat in de loop van het
kalenderjaar de sectorcode wijzigt, zonder dat er een nieuwe
administratieve eenheid ontstaat (het bestaande loonheffingennummer
blijft dus in stand):

\- De Belastingdienst heeft een onjuiste sectorcode toegekend (al dan
niet op grond van onjuiste informatie). Deze situatie moet altijd worden
hersteld.

\- De activiteiten van de onderneming zijn in de loop van het
kalenderjaar dusdanig gewijzigd dat de maatschappelijke functie is
gewijzigd, waardoor de sector wijzigt. De oude sectorcode geldt voor
aangiftetijdvakken tot de datum van sectorwijziging. Voor

aangiftetijdvakken vanaf die datum geldt de nieuwe sectorcode.

**<u>Naam gegevens</u>**

**Naam inhoudingsplichtige R an..200**

*xml tag:* NmIp

In de aangifte Loonheffingen moet de inhoudingsplichtige de naam
vermelden zoals die

door de Belastingdienst aan hem is medegedeeld in de aangiftebrief
waarin de aangifte en betaaldata bekend zijn gemaakt.

Deze naam wordt als volgt bepaald:

Natuurlijke personen: samengestelde naam; voorletters, voorvoegsels en
familienaam conform naamgebruik. Bijv. G W ROOSINK-DEGOEIJEN.

Niet natuurlijke personen: (juridische) naam; in principe de naam zoals
die in de (oprichtings)akte is vastgelegd, als er geen (oprichtings)akte
is (bijv. bij maatschap) dan de naam zoals die in de jaarstukken en
dergelijke is aangegeven.

Naam inhoudingsplichtige moet behoren bij het aangegeven
loonheffingennummer.

**<u>Overige gegevens</u>**

**Loonheffingennummer O an..12**

*xml tag:* LhNr

Een door de Belastingdienst toegekende identificatie waaronder de
administratieve eenheid bekend is bij UWV/Belastingdienst.

Het loonheffingennummer bestaat uit een fiscaal nummer gevolgd door de
hoofdletter L en een subnummer. De waarden 01 t/m 99 zijn toegestaan
voor het subnummer.

Het fiscaal nummer moet u met 9 cijfers (zonder punten) aanleveren.
Fiscale nummers die uit minder dan 9 cijfers bestaan vult u aan met
voorloopnullen. Het fiscaal nummer 1212126 levert u aan als 001212126.

Van de eerste drie cijfers moet er minimaal één niet een nul zijn.

Het fiscaal nummer moet aan de volgende elfproef voldoen:

1\) beschouw de cijfers op de posities van het nummer van links naar
rechts als a0, a1, a2, a3, a4, a5, a6, a7 en a8

2\) het nummer voldoet aan de elfproef indien a8 gelijk is aan de
restwaarde van de volgende berekening: (9\*a0 + 8\*a1 + 7\*a2 + 6\*a3 +
5\*a4 + 4\*a5 + 3\*a6 + 2\*a7) / 11

Het fiscaal nummer moet bestaan en in gebruik zijn.

Het Loonheffingennummer moet bestaan en in gebruik zijn.

Voor softwarepakketten is het niet mogelijk om softwarematig te
controleren of het loonheffingennummer bestaat en in gebruik is.

ORGANISATIE EENHEID 0..999, O

*werkgever - ORGANISATIE EENHEID*

*xml tag:* OrgEenh

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**Ingangsdatum mutatie O an10**

*xml tag:* IngdatMut

**<u>Naam / referentie</u>**

**Naam organisatie-eenheid R an..70**

*xml tag:* NmOrgeenh

**Organisatie-eenheid, code R an..70**

*xml tag:* OrgeenhCd

Bilateraal afgesproken codering van de organisatie-eenheid.

**Onderdeel van organisatieeenheid, code R an..70**

*xml tag:* OndOrgeenhCd

Iedere organisatie-eenheid kan weer onderdeel zijn van een andere
organisatie-eenheid.

PERSONEELSSTERKTE 0..\*, O

*werkgever - organisatie eenheid - PERSONEELSSTERKTE*

*xml tag:* Personeelssterkte

Gegevens met betrekking tot het aantal werknemers.

**<u>Datum waarop de Personeelssterkte is vastgesteld</u>**

**Peildatum personeelssterkte R an10**

*xml tag:* PeildatPersoneelssterkte

De datum waarop de personeelssterkte - in termen van aantallen
werknemers en FTE - is vastgesteld.

**Vorige peildatum personeelssterkte O an10**

*xml tag:* VorigePeildatPersoneelssterkte

**<u>Gegevens over de personeelssterkte</u>**

**Aantal werknemers R n..7**

*xml tag:* AantWrknmrs

**Aantal werknemers in dienst sinds vorige peildatum O n..7**

*xml tag:* AantWrknmrsInDienstSindsVorigePeildat

**Aantal werknemers uit dienst sinds vorige peildatum O n..7**

*xml tag:* AantWrknmrsUitDienstSindsVorigePeildat

**Aantal nulurencontracten O n..7**

*xml tag:* AantalNulurencntrcten

**Aantal FTE O n..7**

*xml tag:* AantFTE

**Aantal vrouwelijke werknemers O n..5**

*xml tag:* AantVrouwelijkeWrknmrs

Het aantal vrouwelijke werknemers dat werkt bij de werkgever.

**Aantal vrouwelijke FTE O n..5**

*xml tag:* AantVrouwelijkeFTE

Het aantal vrouwelijke FTE dat werkt bij de werkgever.

**Aantal mannelijke werknemers O n..5**

*xml tag:* AantMannelijkeWrknmrs

Het aantal mannelijke werknemers dat werkt bij de werkgever.

**Aantal mannelijke FTE O n..5**

*xml tag:* AantMannelijkeFTE

Het aantal mannelijke FTE dat werkt bij de werkgever.

**Aantal uren FTE O n..3**

*xml tag:* AantUrenFTE

Aantal uren dat 1 FTE wordt geacht te werken in een werkweek.

ARBOCONTRACT 0..9, O

*werkgever - ARBOCONTRACT*

*xml tag:* ArboCntrct

Het contract dat de werkgever met de arbodienst heeft gesloten.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Identificatie contract</u>**

**Contractnummer R an..40**

*xml tag:* Cntrnr

**<u>Data</u>**

**Ingangsdatum R an10**

*xml tag:* Ingdat

**Ingangsdatum mutatie O an10**

*xml tag:* IngdatMut

**Einddatum O an10**

*xml tag:* Enddat

**<u>Status</u>**

**Status contract, code R an2**

*xml tag:* StatusCntrctCd

*code list:* Status contract (all selected)

01 Lopend

02 Beëindigd

INTERMEDIAIR 0..1, O

*werkgever - arbocontract - INTERMEDIAIR*

*xml tag:* Intermediair

**Handelsnaam organisatie R an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

STRAATADRES NEDERLAND 0..\*, O

*werkgever - arbocontract - intermediair - STRAATADRES NEDERLAND*

*xml tag:* StrAdrNl

Een adres in Nederland dat wordt bepaald aan de hand van straatnaam en
huisnummer.

**Postcode R an6**

*xml tag:* Pc

De officiële Nederlandse codering, bestaande uit een numerieke
woonplaatscode een alfabetische lettercode.

Norminstantie: NEN 5825 (Postcode)

**Woonplaatsnaam R an..24**

*xml tag:* Wnpl

De door de gemeente vastgestelde naam van een woonplaats.

Norm(instantie): NEN 5825 (Woonplaatsnaam)

**Straatnaam\_ R an..80**

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

COMMUNICATIE 0..9, O

*werkgever - arbocontract - intermediair - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**Soort communicatie, code R an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

06 Zakelijk e-mail adres

08 Zakelijk vaste telefoon

10 Zakelijk mobiele telefoon

**Nummer/adres communicatie R an..512**

*xml tag:* NrCom

DIENSTVERLENING 0..9, O

*werkgever - arbocontract - DIENSTVERLENING*

*xml tag:* Dnstvrlnng

Geeft aan welke dienstverlening wordt afgenomen.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Identificerende gegevens</u>**

**Identificatie dienstverlening R an..40**

*xml tag:* DnstvrlnngId

**<u>Gegevens dienstverlening</u>**

**Type arbopakket, code O an..70**

*xml tag:* TypeArbopakketCd

**Type arbopakket, omschrijving O an..70**

*xml tag:* TypeArbopakketOms

**<u>Data</u>**

**Ingangsdatum R an10**

*xml tag:* Ingdat

**Ingangsdatum mutatie O an10**

*xml tag:* IngdatMut

**Einddatum O an10**

*xml tag:* Enddat

VERZEKERING/DEKKING 0..99, O

*werkgever - VERZEKERING/DEKKING*

*xml tag:* Verzekering

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Identificatie contract</u>**

**Contractnummer O an..40**

*xml tag:* Cntrnr

**Contractnummer pakket O an..40**

*xml tag:* CntrnrPakket

Identificerende kenmerk van de pakketverzekering waarvan het contract
deel uitmaakt.

**<u>Data</u>**

**Ingangsdatum O an10**

*xml tag:* Ingdat

**Ingangsdatum mutatie O an10**

*xml tag:* IngdatMut

**Einddatum O an10**

*xml tag:* Enddat

**Contract periode O an..2**

*xml tag:* CntrctPerCd

Duur van een contract vanaf het moment dat het contract ingaat, of
verlengd wordt.

*code list:* Contractperiode (all selected)

01 Week

02 4 weken

03 Maand

04 Kwartaal

05 Half jaar

06 Jaar

**<u>Status</u>**

**Status contract, code R an2**

*xml tag:* StatusCntrctCd

*code list:* Status contract (all selected)

01 Lopend

02 Beëindigd

**Reden beëindiging contract, code O an2**

*xml tag:* RdnBeeindCntrct

*code list:* Reden beëindiging contract (all selected)

01 Geen werknemers meer

02 Bedrijfsbeëindiging

03 Beëindiging per contractdatum

04 Failliet

05 Opgezegd door verzekeraar

06 Verkeerd opgemaakt contract

99 Onbekend

**<u>Soort verzekeringen</u>**

**Soort verzekering, gecodeerd R an2**

*xml tag:* SrtVerzekeringCd

*code list:* Soort verzekering (all selected)

01 Loondoorbetaling bij ziekte

02 WGA-eigen risicodrager

03 ZW eigen risicodrager

04 Dienstverlening

05 WIA-excedent

06 Vaste WIA-aanvulling

07 WGA-hiaat verzekering (basisvariant)

08 WGA-hiaatverzekering (uitgebreide variant)

09 WIA bodem

10 Overig

**<u>Wachttijd gegevens</u>**

**Wachttijd in werkdagen O n..3**

*xml tag:* WachttijdInDgn

Wachttijd eigen risico in werkdagen.

**<u>Soort verzekering</u>**

**Loonsoort O an..2**

*xml tag:* LoonsrtCd

*code list:* Loonsoort (all selected)

01 Bruto loon

02 SV loon

03 Loon voor loonheffing

04 Uniform loon

**Maximum verzekerd jaarloon O n..9,2**

*xml tag:* MaxJrLoonVrzkrd

**Dekkingspercentage jaar 1 O n..6,2**

*xml tag:*

**Dekkingspercentage jaar 2 O n..6,2**

*xml tag:* PrcDkkngJr2

**<u>Werkgeverslasten</u>**

**Percentage werkgeverslasten O n..6,2**

*xml tag:* PercWrkgvrslasten

Percentage meeverzekerde werkgeverslasten.

**<u>Kenmerk</u>**

**Productkenmerk O an..70**

*xml tag:* Productkenmerk

Maatschappijspecifiek kenmerk om verzekering/dekking te typeren.

**<u>Inloop/uitloop</u>**

**Inloop J/N R a1**

*xml tag:* InloopJN

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

**Uitloop J/N R a1**

*xml tag:* UitloopJN

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

AFSPRAKEN UITWISSELING VERZUIMDATA 0..9, O

*werkgever - verzekering/dekking - AFSPRAKEN UITWISSELING VERZUIMDATA*

*xml tag:* AfsprakenUitwisselingVerzuimdata

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Data</u>**

**Ingangsdatum R an10**

*xml tag:* Ingdat

**Einddatum O an10**

*xml tag:* Enddat

**<u>Uitwisseling van verzuimgegevens</u>**

**Uitwisseling verzuimmeldingen, code R an2**

*xml tag:* UitwisselingVerzuimmeldingenCd

*code list:* Uitwisseling verzuimmeldingen (all selected)

01 Verzekeraar/Volmacht -\> Arbodienst

02 Arbodienst --\> Verzekeraar/Volmacht

99 Niet van toepassing

**Frequentie, code R an2**

*xml tag:* FrequentieCd

*code list:* Frequentie (all selected)

01 Dagbasis

02 Maandbasis

03 Kwartaalbasis

04 Jaarbasis

05 Continu

AFSPRAKEN UITWISSELING VERZUIMDATA 0..9, O

*werkgever - AFSPRAKEN UITWISSELING VERZUIMDATA*

*xml tag:* AfsprakenUitwisselingVerzuimdata

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Data</u>**

**Ingangsdatum R an10**

*xml tag:* Ingdat

**Einddatum O an10**

*xml tag:* Enddat

**<u>Uitwisseling van verzuimgegevens</u>**

**Uitwisseling verzuimmeldingen, code R an2**

*xml tag:* UitwisselingVerzuimmeldingenCd

*code list:* Uitwisseling verzuimmeldingen (all selected)

01 Verzekeraar/Volmacht -\> Arbodienst

02 Arbodienst --\> Verzekeraar/Volmacht

99 Niet van toepassing

**Frequentie, code R an2**

*xml tag:* FrequentieCd

*code list:* Frequentie (all selected)

01 Dagbasis

02 Maandbasis

03 Kwartaalbasis

04 Jaarbasis

05 Continu

COMMUNICATIE 0..9, O

*werkgever - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**<u>Soort communicatie</u>**

**Soort communicatie, code R an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

01 Vaste telefoon

02 Mobiele telefoon

04 E-mail adres

**<u>Nummer</u>**

**Nummer/adres communicatie R an..512**

*xml tag:* NrCom

CONTACTPERSOON 0..\*, O

*werkgever - CONTACTPERSOON*

*xml tag:* Cntprsn

**<u>Identificerende gegevens</u>**

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

**Voorletters R a..6**

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

**Geslachtsaanduiding, code R an1**

*xml tag:* GslchtCd

De sekse van een persoon, zoals bij de geboorte formeel vastgesteld of
nadien formeel gewijzigd.

Bron: NEN 1888: 2002 - Geslacht

*code list:* Geslacht (all selected)

M Man

O Onbekend/niet gespecificeerd

V Vrouw

**Rol contactpersoon, code O an2**

*xml tag:* RolCntprsnCd

*code list:* Rol contactpersoon (subset selected)

02 Casemanager

03 Medewerker P&O

05 Algemeen contactpersoon

COMMUNICATIE 0..\*, O

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
