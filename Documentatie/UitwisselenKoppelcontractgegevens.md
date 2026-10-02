**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Basis Arbodienst Verzekeraar*

Functional message: ***Uitwisselen koppel/contractgegevens 2026***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

6 juli 2026

Summary

Bericht algemeen 1..1, V

Verzekeraar/Volmacht 1..1, V

Arbodienst 1..1, V

Werkgever 1..\*, V

1 Personeelssterkte 0..999, F

1 Straatadres Nederland 0..9, F

1 Straatadres Buitenland 0..\*, F

1 Administratieve Eenheid 0..1, F

2 Sector Risicogroep 0..1, F

1 Organisatie eenheid 0..999, F

2 Personeelssterkte 0..\*, F

1 Arbocontract 0..9, F

2 Intermediair 0..1, F

3 Communicatie 0..9, F

2 Dienstverlening 0..9, F

1 Verzekering/Dekking 0..99, F

1 Machtigingen uitwisseling verzuim 0..1, F

1 Communicatie 0..9, F

1 Contactpersoon 0..\*, F

2 Communicatie 0..\*, F

BERICHT ALGEMEEN 1..1, V

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code V an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00700 Uitwisselen koppel/contractgegevens

**Versienummer bericht, code V an..5**

*xml tag:* VnrBrCd

*code list:* Versienummer bericht (subset selected)

00006 Versienummer 6

**<u>Functie bericht</u>**

**Functie bericht, code V an2**

*xml tag:* FunctieBrCd

*code list:* SIVI (subset selected)

01 Koppelgegevens verzekeraar --\> arbodienst

02 Koppelgegevens arbodienst --\> verzekeraar

03 Contractdata werkgever - verzekeraar

04 Contractdata werkgever - arbodienst

**<u>Aanmaakdatum</u>**

**Aanmaakdatum bericht V an10**

*xml tag:* AandatBr

**Aanmaaktijd bericht V an8**

*xml tag:* AantijdBr

**<u>Inzender</u>**

**Identificatie inzender V an..40**

*xml tag:* IdInzndr

Bilateraal afgesproken codering betreffende de inzender van het bericht.

**Gebruikt softwarepakket V an..35**

*xml tag:* GebrSwPakket

Beschrijving van het softwarepakket dat de aanleveraar heeft gebruikt
voor de vervaardiging van het bericht.

**<u>Ontvanger</u>**

**Identificatie ontvanger V an..40**

*xml tag:* IdOntvngr

Bilateraal afgesproken codering betreffende de ontvanger
(eindbestemming) van het bericht.

**<u>Berichtreferentie</u>**

**Berichtreferentienummer V an..512**

*xml tag:* Berrefnr

**Berichtreferentienummer ingezonden bericht F an..512**

*xml tag:* BerrefnrIngzndnBer

Het referentienummer van het bericht waar het onderhavige bericht een
reactie op is.

**<u>Testindicatie</u>**

**Test J/N V a1**

*xml tag:* TestJN

Geeft aan of het een testbericht betreft.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

**<u>Ontvangstbevestiging</u>**

**Ontvangstbevestiging gewenst J/N V a1**

*xml tag:* OntvngstbevJN

Geeft aan of de inzender van het bericht een ontvangstbevestiging wenst.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

**<u>Contractgegevens gewenst</u>**

**Contractgegevens gewenst J/N V a1**

*xml tag:* CntrctGegGewenstJN

Aanduiding van de zender van het bericht of het gewenst is dat de
ontvanger de contractgegevens retourneert.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

VERZEKERAAR/VOLMACHT 1..1, V

*VERZEKERAAR/VOLMACHT*

*xml tag:* VrzkrVolmacht

**<u>Handelsnaam</u>**

**Handelsnaam organisatie V an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

**<u>Identificerende gegevens</u>**

**Identificatie verzekeraar/volmacht, code V an..4**

*xml tag:* IdVrzkrVolmachtCd

Hiervoor wordt de POR-code gebruikt. Op dit moment wordt de POR-code
branchebreed gebruikt voor het uniek identificeren van bijna 700
verzekeraars/volmachten. Zie www.sivi.org.

*code list:* POR maatschappij aanduiding (all selected)

*The codes of this codelist are documented in a separate document*

ARBODIENST 1..1, V

*ARBODIENST*

*xml tag:* Arbdnst

**<u>Handelsnaam</u>**

**Handelsnaam organisatie F an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

**<u>Arbo-dienst</u>**

**Arbodienst, code V an3**

*xml tag:* ArbdnstCd

De lijst met codes van gecertificeerde Arbodiensten is gepubliceerd op
de website van SIVI. Zie www.sivi.org.

*code list:* Code Arbodienst (all selected)

*The codes of this codelist are documented in a separate document*

WERKGEVER 1..\*, V

*WERKGEVER*

*xml tag:* Wrkgvr

Bij het beschrijven van de kenmerken van de Werkgever wordt in een
aantal gevallen de term Inhoudingsplichtige gebruikt.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code V an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Handelsnaam</u>**

**Handelsnaam organisatie V an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

**<u>Kamer van Koophandel</u>**

**Inschrijvingsnummer Kamer van Koophandel F n..8**

*xml tag:* InschrijvingsnrKvK

Een identificerend nummer dat de Kamer van Koophandel toekent aan
ondernemingen zoals vermeld in de Handelsregisterwet.

Bron: SUWI Gegevens Register

**Vestigingsnummer F n..12**

*xml tag:* VestigingsnrHandelsregister

Een identificerend nummer voor een vestiging in het Handelsregister.

Norminstantie: Handelsregister

**<u>Identificatie bij de arbodienst</u>**

**Identificatie werkgever bij arbodienst F an..40**

*xml tag:* IdWrkgvrArbdnst

De identificatiecode die de arbodienst heeft aangeleverd aan de
werkgever waardoor de werkgever wordt onderscheden van andere werkgevers
in de administratie van de arbodienst.

**Aansluitnummer gegevensuitwisseling Arbodienst F an..70**

*xml tag:* AansltnrGeguitwlngArbdnst

Het aansluitnummer voor de gegevensuitwisseling dat de arbodienst heeft
aangeleverd aan de werkgever waardoor de werkgever wordt onderscheden
van andere werkgevers in de administratie van de arbodienst.

**Reden geen gegevensuitwisseling, code F an..2**

*xml tag:* RdnGnGgvnsuitw

*code list:* Reden geen gegevensuitwisseling, code (all selected)

01 WerkgevrID onjuist

02 Werkgever onbekend

03 Werkgevergegevens komen niet overeen

04 Koppelcode onbekend

**<u>Identificatie bij verzekeraar</u>**

**Identificatie werkgever bij verzekeraar F an..40**

*xml tag:* IDWrkgvrVerzekeraar

**<u>Identificatie bij UWV</u>**

**Identificatie werkgever bij UWV F an..40**

*xml tag:* IdWrkgvrUWV

De identificatie die het UWV heeft aangeleverd aan de werkgever

waardoor de werkgever wordt onderscheiden van andere werkgevers in de
administratie van het UWV.

**<u>Loonbelasting / loonheffingen</u>**

**Loonheffingennummer F an..12**

*xml tag:* Lhnr

Een door de Belastingdienst toegekende identificatie voor de
administratieve eenheid waaronder de werkgever bekend is en
loonheffingen afdraagt.

**<u>Eigenrisicodragerschap</u>**

**Identificatie verzekeraar ERD WGA, code F an..4**

*xml tag:* IdVrzkrWGACd

Hiervoor wordt de POR-code gebruikt. Zie www.sivi.org.

*code list:* POR maatschappij aanduiding (all selected)

*The codes of this codelist are documented in a separate document*

**Identificatie verzekeraar ERD ZW, code F an..4**

*xml tag:* IdVrzkrERDZWCd

Hiervoor wordt de POR-code gebruikt. Zie www.sivi.org.

*code list:* POR maatschappij aanduiding (all selected)

*The codes of this codelist are documented in a separate document*

**<u>Collectieve zorgverzekering</u>**

**Identificatie verzekeraar collectieve zorg, code F an..4**

*xml tag:* IdVrzkrCollectieveZorgCd

Hiervoor wordt de POR-code gebruikt. Zie www.sivi.org.

*code list:* POR maatschappij aanduiding (all selected)

*The codes of this codelist are documented in a separate document*

**<u>Sector waarin werkgever opereert</u>**

**Sector volgens SBI F n..5**

*xml tag:* SectorVolgensSBI

De sector waarin de werkgever opereert volgens de Standaard
Bedrijfsindeling (SBI) het Centraal Bureau voor de Statistiek van
Nederland.

PERSONEELSSTERKTE 0..999, F

*werkgever - PERSONEELSSTERKTE*

*xml tag:* Personeelssterkte

Gegevens met betrekking tot het aantal werknemers.

**<u>Datum waarop de Personeelssterkte is vastgesteld</u>**

**Peildatum personeelssterkte V an10**

*xml tag:* PeildatPersoneelssterkte

De datum waarop de personeelssterkte - in termen van aantallen
werknemers en FTE - is vastgesteld.

**Vorige peildatum personeelssterkte F an10**

*xml tag:* VorigePeildatPersoneelssterkte

**<u>Gegevens over de personeelssterkte</u>**

**Aantal werknemers V n..7**

*xml tag:* AantWrknmrs

**Aantal werknemers in dienst sinds vorige peildatum F n..7**

*xml tag:* AantWrknmrsInDienstSindsVorigePeildat

**Aantal werknemers uit dienst sinds vorige peildatum F n..7**

*xml tag:* AantWrknmrsUitDienstSindsVorigePeildat

**Aantal nulurencontracten F n..7**

*xml tag:* AantalNulurencntrcten

**Aantal FTE F n..7**

*xml tag:* AantFTE

**Aantal vrouwelijke werknemers F n..5**

*xml tag:* AantVrouwelijkeWrknmrs

Het aantal vrouwelijke werknemers dat werkt bij de werkgever.

**Aantal vrouwelijke FTE F n..5**

*xml tag:* AantVrouwelijkeFTE

Het aantal vrouwelijke FTE dat werkt bij de werkgever.

**Aantal mannelijke werknemers F n..5**

*xml tag:* AantMannelijkeWrknmrs

Het aantal mannelijke werknemers dat werkt bij de werkgever.

**Aantal mannelijke FTE F n..5**

*xml tag:* AantMannelijkeFTE

Het aantal mannelijke FTE dat werkt bij de werkgever.

**Aantal uren FTE F n..3**

*xml tag:* AantUrenFTE

Aantal uren dat 1 FTE wordt geacht te werken in een werkweek.

STRAATADRES NEDERLAND 0..9, F

*werkgever - STRAATADRES NEDERLAND*

*xml tag:* StrAdrNl

Een adres in Nederland dat wordt bepaald aan de hand van straatnaam en
huisnummer.

**<u>Soort adres</u>**

**Soort adres, code F an2**

*xml tag:* SrtAdrsCd

*code list:* Soort adres (subset selected)

01 Woonadres, verblijfadres of vestigingsadres

02 Postadres cq correspondentie adres

03 Factuuradres

05 OR adres

**<u>Periode geldig</u>**

**Ingangsdatum F an10**

*xml tag:* Ingdat

**Einddatum F an10**

*xml tag:* Enddat

De datum van de laatste dag waarop de gegevens geldig zijn.

**<u>Generiek voor adres</u>**

**Postcode V an6**

*xml tag:* Pc

De officiële Nederlandse codering, bestaande uit een numerieke
woonplaatscode een alfabetische lettercode.

Norminstantie: NEN 5825 (Postcode)

**Woonplaatsnaam F an..24**

*xml tag:* Wnpl

De door de gemeente vastgestelde naam van een woonplaats.

Norm(instantie): NEN 5825 (Woonplaatsnaam)

**<u>Specifiek voor straatadres Nederland</u>**

**Straatnaam\_ F an..80**

*xml tag:* StraatLang

De officiële door de gemeente vastgestelde naam van een straat.

Als de officiële straatnaam echter langer is dan 24 posities dan mag

deze ingekort volgens de specificaties van de BOCO-norm.

Norm(instantie)

NEN 5825 (Straatnaam)

**Huisnummer V n..5**

*xml tag:* Huisnr

De numerieke aanduiding zoals deze door de gemeente aan het object is
toegekend.

Norminstantie: NEN 5825 (Huisnummer)

**Huisnummertoevoeging F an..4**

*xml tag:* HuisToev

De alfanumerieke aanduiding achter huisnummer, zoals toegekend door de
gemeente.

Norminstantie: NEN 5825 (Huisnummertoevoeging)

STRAATADRES BUITENLAND 0..\*, F

*werkgever - STRAATADRES BUITENLAND*

*xml tag:* StrAdrBl

Een adres in het buitenland dat wordt bepaald aan de hand van straatnaam
en huisnummer.

**<u>Soort adres</u>**

**Soort adres, code F an2**

*xml tag:* SrtAdrsCd

*code list:* Soort adres (subset selected)

01 Woonadres, verblijfadres of vestigingsadres

02 Postadres cq correspondentie adres

03 Factuuradres

05 OR adres

**<u>Periode geldig</u>**

**Ingangsdatum F an10**

*xml tag:* Ingdat

**Einddatum F an10**

*xml tag:* Enddat

De datum van de laatste dag waarop de gegevens geldig zijn.

**<u>Generiek voor adres buitenland</u>**

**Locatieomschrijving buitenland F an..35**

*xml tag:* LocomsBtl

Een nadere aanduiding bij een buitenlands adres.

Bron: SUWI

**Postcode buitenland F an..9**

*xml tag:* PcBtl

Een door de buitenlandse postdienst vastgestelde codering voor een adres
in het buitenland.

Bron: SUWI

**Woonplaatsnaam buitenland V an..24**

*xml tag:* WnplBtl

De naam van een woonplaats in het buitenland.

Bron: SUWI

**Regionaam buitenland F an..24**

*xml tag:* RegBtl

De naam van een gebiedsdeel binnen een land.

Bron: SUWI

**Land, code V a2**

*xml tag:* LandCd

De code van een huidig land of gebiedsdeel conform ISO 3166.

Norminstantie: ISO 3166 (Entity, Alpha-2 code)

*code list:* ISO landcode (all selected)

*The codes of this codelist are documented in a separate document*

**Landnaam F an..40**

*xml tag:* Landnm

De naam van een land of een gebiedsdeel.

Bron: SUWI

**<u>Specifiek voor straatadres buitenland</u>**

**Straatnaam\_ F an..80**

*xml tag:* StraatLang

**Huisnummer buitenland V an..9**

*xml tag:* HuisnrBtl

**Huisnummer toevoeging buitenland F an..70**

*xml tag:* HuisnrToevBtl

ADMINISTRATIEVE EENHEID 0..1, F

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

**Naam inhoudingsplichtige V an..200**

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

**Loonheffingennummer F an..12**

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

SECTOR RISICOGROEP 0..1, F

*werkgever - administratieve eenheid - SECTOR RISICOGROEP*

*xml tag:* SectorRisicogroep

Een su-indeling voor administratieve eenheden binnen een sector SV
waarvoor een eigen premie geldt.

**Code sector OSV V n3**

*xml tag:* CdSectorOsv

De code die het bedrijfs- en beroepsleven indeelt in sectoren, waarbij
elke sector één of meer takken van bedrijf of beroep of gedeelte daarvan
omvat.

*code list:* Code sector OSV (all selected)

001 Agrarisch bedrijf

002 Tabaksverwerkende industrie

003 Bouwbedrijf

004 Baggerbedrijf

005 Houten emballage-industrie, etc.

006 Timmerindustrie

007 Meubel- en orgelbouwindustrie

008 Groothandel in hout, etc.

009 Grafische industrie

010 Metaalindustrie

011 Elektrotechnische industrie

012 Metaal- en technische bedrijfstakken

013 Bakkerijen

014 Suikerverwerkende industrie

015 Slagersbedrijven

016 Slagers overig

017 Detailhandel en ambachten

018 Reiniging

019 Grootwinkelbedrijf

020 Havenbedrijven

021 Havenclassificeerders

022 Binnenscheepvaart

023 Visserij

024 Koopvaardij

025 Vervoer KLM

026 Vervoer NS

027 Vervoer Posterijen

028 Taxivervoer

029 Openbaar vervoer

030 Besloten busvervoer

031 Overig personenvervoer te land en in de lucht

032 Overig goederenvervoer te land en in de lucht

033 Horeca algemeen

034 Horeca catering

035 Gezondheiid, geestelijke en maatschappelijke belangen

038 Banken

039 Verzekeringswezen

040 Uitgeverij

041 Groothandel I

042 Groothandel II

043 Zakelijke dienstverlening I

044 Zakelijke dienstverlening II

045 Zakelijke dienstverlening III

046 Zuivelindustrie

047 Textielindustrie

048 Steen-, cement-, glas-, en keramische industrie

049 Chemische industrie

050 Voedingsindustrie

051 Algemene industrie

052 Uitzendbedrijven

053 Bewakingsondernemingen

054 Culturele instellingen

055 Overige takken van bedrijf en beroep

056 Schildersbedrijf

057 Stukadoorsbedrijf

058 Dakdekkerbedrijf

059 Mortelbedrijf

060 Steenhouwersbedrijf

061 Overheid, onderwijs en wetenschappen

062 Overheid, rijk, politie en rechterlijke macht

063 Overheid, defensie

064 Overheid, provincies, gemeenten en waterschappen

065 Overheid, openbare nutsbedrijven

066 Overheid, overige instellingen

067 Werk en (re)integratie

068 Railbouw

069 Telecommunicatie

998 Sector niet van toepassing

**Code risicopremiegroep F n2**

*xml tag:* CdRisicopremiegroep

De code die de rsicopremiegroep binnen de sector aangeeft.

*code list:* Code risicogroep (all selected)

00 Niet van toepassing

01 Premiegroep kortingsklasse

02 Premiegroep middenklasse

03 Premiegroep opslagklasse

04 Premiegroep kortingsklasse

05 Premiegroep middenklasse

06 Premiegroep opslagklasse

07 Premiegroep detachering

08 Premiegroep intermediaire diensten

09 Uitzendbedrijven I B + II B

10 Uitzendbedrijven I A

11 Uitzendbedrijven II A

ORGANISATIE EENHEID 0..999, F

*werkgever - ORGANISATIE EENHEID*

*xml tag:* OrgEenh

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code V an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**Ingangsdatum mutatie F an10**

*xml tag:* IngdatMut

**<u>Naam / referentie</u>**

**Naam organisatie-eenheid V an..70**

*xml tag:* NmOrgeenh

**Organisatie-eenheid, code V an..70**

*xml tag:* OrgeenhCd

Bilateraal afgesproken codering van de organisatie-eenheid.

**Onderdeel van organisatieeenheid, code V an..70**

*xml tag:* OndOrgeenhCd

Iedere organisatie-eenheid kan weer onderdeel zijn van een andere
organisatie-eenheid.

PERSONEELSSTERKTE 0..\*, F

*werkgever - organisatie eenheid - PERSONEELSSTERKTE*

*xml tag:* Personeelssterkte

Gegevens met betrekking tot het aantal werknemers.

**<u>Datum waarop de Personeelssterkte is vastgesteld</u>**

**Peildatum personeelssterkte V an10**

*xml tag:* PeildatPersoneelssterkte

De datum waarop de personeelssterkte - in termen van aantallen
werknemers en FTE - is vastgesteld.

**Vorige peildatum personeelssterkte F an10**

*xml tag:* VorigePeildatPersoneelssterkte

**<u>Gegevens over de personeelssterkte</u>**

**Aantal werknemers V n..7**

*xml tag:* AantWrknmrs

**Aantal werknemers in dienst sinds vorige peildatum F n..7**

*xml tag:* AantWrknmrsInDienstSindsVorigePeildat

**Aantal werknemers uit dienst sinds vorige peildatum F n..7**

*xml tag:* AantWrknmrsUitDienstSindsVorigePeildat

**Aantal nulurencontracten F n..7**

*xml tag:* AantalNulurencntrcten

**Aantal FTE F n..7**

*xml tag:* AantFTE

**Aantal vrouwelijke werknemers F n..5**

*xml tag:* AantVrouwelijkeWrknmrs

Het aantal vrouwelijke werknemers dat werkt bij de werkgever.

**Aantal vrouwelijke FTE F n..5**

*xml tag:* AantVrouwelijkeFTE

Het aantal vrouwelijke FTE dat werkt bij de werkgever.

**Aantal mannelijke werknemers F n..5**

*xml tag:* AantMannelijkeWrknmrs

Het aantal mannelijke werknemers dat werkt bij de werkgever.

**Aantal mannelijke FTE F n..5**

*xml tag:* AantMannelijkeFTE

Het aantal mannelijke FTE dat werkt bij de werkgever.

**Aantal uren FTE F n..3**

*xml tag:* AantUrenFTE

Aantal uren dat 1 FTE wordt geacht te werken in een werkweek.

ARBOCONTRACT 0..9, F

*werkgever - ARBOCONTRACT*

*xml tag:* ArboCntrct

Het contract dat de werkgever met de arbodienst heeft gesloten.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code V an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Identificatie contract</u>**

**Contractnummer V an..40**

*xml tag:* Cntrnr

**<u>Data</u>**

**Ingangsdatum V an10**

*xml tag:* Ingdat

**Ingangsdatum mutatie F an10**

*xml tag:* IngdatMut

**Einddatum F an10**

*xml tag:* Enddat

De datum van de laatste dag waarop de gegevens geldig zijn.

**<u>Status</u>**

**Status contract, code V an2**

*xml tag:* StatusCntrctCd

*code list:* Status contract (all selected)

01 Lopend

02 Beëindigd

**Type arbocontract, code V an..2**

*xml tag:* TypArbContCod

*code list:* Type arbocontract (all selected)

01 Combicontract

02 Monocontract via verzekeraar

03 Monocontract via arbodienst

INTERMEDIAIR 0..1, F

*werkgever - arbocontract - INTERMEDIAIR*

*xml tag:* Intermediair

**Handelsnaam organisatie V an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

COMMUNICATIE 0..9, F

*werkgever - arbocontract - intermediair - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**Soort communicatie, code V an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

06 Zakelijk e-mail adres

08 Zakelijk vaste telefoon

10 Zakelijk mobiele telefoon

**Nummer/adres communicatie V an..512**

*xml tag:* NrCom

Het veld bevat een geldige duiding van de soort communicatie, zoals
e-mailadres of telefoonummer. In het geval van een telefoonnummer is het
formaat in het bericht volgens ITU-T E.164: +31201234567

DIENSTVERLENING 0..9, F

*werkgever - arbocontract - DIENSTVERLENING*

*xml tag:* Dnstvrlnng

Geeft aan welke dienstverlening wordt afgenomen.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code V an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Identificerende gegevens</u>**

**Identificatie dienstverlening V an..40**

*xml tag:* DnstvrlnngId

**<u>Gegevens dienstverlening</u>**

**Type arbopakket, code F an..70**

*xml tag:* TypeArbopakketCd

**Type arbopakket, omschrijving F an..70**

*xml tag:* TypeArbopakketOms

**Reden einde dienstverlening, code F an..2**

*xml tag:* RdnEindDnstvrl

*code list:* Reden einde dienstverlening (all selected)

01 Overvoer

02 Vervanging contract

03 Dienstverlening komt te vervallen

04 Dienstverlening omgezet naar monocontract

**<u>Data</u>**

**Ingangsdatum V an10**

*xml tag:* Ingdat

**Ingangsdatum mutatie F an10**

*xml tag:* IngdatMut

**Einddatum F an10**

*xml tag:* Enddat

De datum van de laatste dag waarop de gegevens geldig zijn.

VERZEKERING/DEKKING 0..99, F

*werkgever - VERZEKERING/DEKKING*

*xml tag:* Verzekering

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code V an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Identificatie contract</u>**

**Contractnummer F an..40**

*xml tag:* Cntrnr

**Contractnummer pakket F an..40**

*xml tag:* CntrnrPakket

Identificerende kenmerk van de pakketverzekering waarvan het contract
deel uitmaakt.

**<u>Data</u>**

**Ingangsdatum F an10**

*xml tag:* Ingdat

**Ingangsdatum mutatie F an10**

*xml tag:* IngdatMut

**Einddatum F an10**

*xml tag:* Enddat

De datum van de laatste dag waarop de gegevens geldig zijn.

**Contract periode F an..2**

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

**Status contract, code V an2**

*xml tag:* StatusCntrctCd

*code list:* Status contract (all selected)

01 Lopend

02 Beëindigd

**Reden beëindiging contract, code F an2**

*xml tag:* RdnBeeindCntrct

*code list:* Reden beëindiging contract (all selected)

01 Geen werknemers meer

02 Bedrijfsbeëindiging

03 Beëindiging per contractdatum

04 Failliet

05 Opgezegd door verzekeraar

06 Verkeerd opgemaakt contract

07 Overvoer

08 Vervanging contract

99 Onbekend

**<u>Soort verzekeringen</u>**

**Soort verzekering, gecodeerd V an2**

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

**Wachttijd in werkdagen F n..3**

*xml tag:* WachttijdInDgn

Wachttijd eigen risico in werkdagen.

**<u>Soort verzekering</u>**

**Loonsoort F an..2**

*xml tag:* LoonsrtCd

*code list:* Loonsoort (all selected)

01 Bruto loon

02 SV loon

03 Loon voor loonheffing

04 Uniform loon

**Maximum verzekerd jaarloon F n..9,2**

*xml tag:* MaxJrLoonVrzkrd

**Dekkingspercentage jaar 1 F n..6,2**

*xml tag:* PrcDkkngJr1

**Dekkingspercentage jaar 2 F n..6,2**

*xml tag:* PrcDkkngJr2

**<u>Werkgeverslasten</u>**

**Percentage werkgeverslasten F n..6,2**

*xml tag:* PercWrkgvrslasten

Percentage meeverzekerde werkgeverslasten.

**<u>Kenmerk</u>**

**Productkenmerk F an..70**

*xml tag:* Productkenmerk

Maatschappijspecifiek kenmerk om verzekering/dekking te typeren.

**<u>Inloop/uitloop</u>**

**Inloop J/N V a1**

*xml tag:* InloopJN

Een indicatie dat inloop van toepassing is. Hierbij zijn de
interventiekosten gedekt, ook als de ingangsdatum van verzuim van vóór
het verzuimcontract is.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

**Uitloop J/N V a1**

*xml tag:* UitloopJN

Indicatie dat uitloop van toepassing is. Hierbij zijn de
interventiekosten gedekt, ook als verzuim doorloopt na beëindiging van
het contract.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

MACHTIGINGEN UITWISSELING VERZUIM 0..1, F

*werkgever - MACHTIGINGEN UITWISSELING VERZUIM*

*xml tag:* MchtVrzm

Machtigingsafspraken die nodig zijn bij het koppelen van monocontracten.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code V an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (subset selected)

01 Nieuw

02 Gewijzigd

04 Ter identificatie en/ of ter informatie

**<u>Data</u>**

**Ingangsdatum V an10**

*xml tag:* Ingdat

**Einddatum F an10**

*xml tag:* Enddat

**<u>Machtigingsgegevens</u>**

**Koppelcode V an..70**

*xml tag:* KpplCd

Identificatie van de klant voor gegevensuitwisseling. Klant haalt deze
code bij de ontvangende partij.

**Reden einde machtiging, code F an2**

*xml tag:* RdnEndMCd

Code die de reden aangeeft voor het beëindigen van de machtiging voor
het koppelen op basis van monocontracten.

*code list:* Reden einde machtiging, code (all selected)

01 Verzekering uitgebreid met arbodienstverlening

02 Beëindiging verzuimverzekering

03 Beëindiging arbodienstverlening vanuit arbodienst

04 Verzoek werkgever

COMMUNICATIE 0..9, F

*werkgever - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**<u>Soort communicatie</u>**

**Soort communicatie, code V an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

01 Vaste telefoon

02 Mobiele telefoon

04 E-mail adres

**<u>Nummer</u>**

**Nummer/adres communicatie V an..512**

*xml tag:* NrCom

Het veld bevat een geldige duiding van de soort communicatie, zoals
e-mailadres of telefoonummer. In het geval van een telefoonnummer is het
formaat in het bericht volgens ITU-T E.164: +31201234567

CONTACTPERSOON 0..\*, F

*werkgever - CONTACTPERSOON*

*xml tag:* Cntprsn

**<u>Identificerende gegevens</u>**

**Personeelsnummer F an..35**

*xml tag:* Persnr

De code waarmee de natuurlijk persoon in de loonadministratie van de
inhoudingsplichtige bekend is.

**<u>Naamgegevens</u>**

**Achternaam/Achternamen V an..200**

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

**Voorletters V a..6**

*xml tag:* Voorl

De verzameling letters die wordt gevormd door de eerste letter van alle
in volgorde voorkomende voornamen.

Bestaan uit hoofdletters, zijn aaneengesloten en bevatten geen punten.
Alleen alfabetische tekens zijn toegestaan.

Bron: Loonaangifte.

**Roepnaam F a..35**

*xml tag:* Roepnaam

Voornaam waarmee iemand wordt aangesproken.

**<u>Overige gegevens</u>**

**Geslachtsaanduiding, code V an1**

*xml tag:* GslchtCd

De sekse van een persoon, zoals bij de geboorte formeel vastgesteld of
nadien formeel gewijzigd.

Bron: NEN 1888: 2002 - Geslacht

*code list:* Geslacht (all selected)

M Man

O Onbekend/niet gespecificeerd

V Vrouw

**Rol contactpersoon, code F an2**

*xml tag:* RolCntprsnCd

*code list:* Rol contactpersoon (subset selected)

02 Casemanager

03 Medewerker P&O

05 Algemeen contactpersoon

COMMUNICATIE 0..\*, F

*werkgever - contactpersoon - COMMUNICATIE*

*xml tag:* Com

Communicatie is de verzameling van gegevens die het partijen mogelijk
maakt met hulpmiddelen met elkaar te communiceren.

**<u>Soort communicatie</u>**

**Soort communicatie, code V an2**

*xml tag:* SrtComCd

*code list:* Communicatiesoort (subset selected)

06 Zakelijk e-mail adres

08 Zakelijk vaste telefoon

10 Zakelijk mobiele telefoon

**<u>Nummer</u>**

**Nummer/adres communicatie V an..512**

*xml tag:* NrCom

Het veld bevat een geldige duiding van de soort communicatie, zoals
e-mailadres of telefoonummer. In het geval van een telefoonnummer is het
formaat in het bericht volgens ITU-T E.164: +31201234567
