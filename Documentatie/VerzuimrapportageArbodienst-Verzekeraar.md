**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel 0.2*

Transaction type: *Basistransactie Verzuim*

Functional message: ***Verzuimrapportage Arbodienst -\> Verzekeraar
2019***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

1 april 2019

Summary

Bericht algemeen 1..1, R

Werkgever 1..\*, R

1 Werknemer 1..\*, R

2 Partner 0..1, O

2 Straatadres Nederland 0..9, O

2 Straatadres Buitenland 0..9, O

2 Dienstverband 1..99, R

3 Verzuim 1..99, R

4 Werkhervattingsadvies 0..99, O

5 Werkhervattingsperiode 1..99, R

4 Actie 0..99, O

BERICHT ALGEMEEN 1..1, R

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code R an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00702 Verzuimmelding Arbodienst --\> Verzekeraar

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

**<u>Verslagperiode</u>**

**Ingangsdatum Verslagperiode O an10**

*xml tag:* IngdatVerslagperiode

**Einddatum verslagperiode O an10**

*xml tag:* EnddatVerslagperiode

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

**Loonheffingennummer O an..12**

*xml tag:* Lhnr

Een door de Belastingdienst toegekende identificatie voor de
administratieve eenheid waaronder de werkgever bekend is en
loonheffingen afdraagt.

WERKNEMER 1..\*, R

*werkgever - WERKNEMER*

*xml tag:* Wrknmr

Een werknemer is de natuurlijke persoon met wie een inkomstenverhouding
binnen de loonadministratie bestaat.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (subset selected)

04 Ter identificatie en/ of ter informatie

**Ingangsdatum mutatie O an10**

*xml tag:* IngdatMut

**<u>Identificerende gegevens</u>**

**Burgerservicenummer R n..9**

*xml tag:* SofiNr

Een door de Gemeente aan een natuurlijk persoon toegekend uniek
administratief nummer, ook wel BSN genoemd.

Indien de inhoudingsplichtige niet beschikt of kan beschikken over het
BSN dan moet in ieder geval het Personeelsnummer doorgegeven worden.

Bron: Loonaangifte.

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

**Overlijdensdatum O an10**

*xml tag:* Overldat

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

*code list:* Geslacht (subset selected)

M Man

V Vrouw

**<u>Identificatie</u>**

**Identificatie werknemer O an..40**

*xml tag:* IdWrknmr

Een unieke identificatie van de werknemer bij de werkgever. Een eenmaal
uitgegeven identificatie wordt niet hergebruikt.

**Identificatie werknemer oud O an..40**

*xml tag:* IdWrknmrOud

**Identificatie werknemer arbodienst O an..40**

*xml tag:* IdWrknmrArbdnst

**Identificatie werknemer verzekeraar O an..40**

*xml tag:* IdWrknmrVzkr

PARTNER 0..1, O

*werkgever - werknemer - PARTNER*

*xml tag:* Prtnr

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (all selected)

01 Nieuw

02 Gewijzigd

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

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

*code list:* Soort adres (all selected)

01 Woonadres, verblijfadres of vestigingsadres

02 Postadres cq correspondentie adres

03 Factuuradres

04 Tijdelijk adres

05 OR adres

06 Verpleegadres

**Soort verpleegadres, code O an2**

*xml tag:* SrtVrplgadrsCd

*code list:* Soort verpleegadres (all selected)

01 Ander huisadres

Bijvoorbeeld familie of vakantieadres.

02 Verpleeginstelling

Ziekenhuis, verpleeghuis, etc.

03 Camping

99 Onbekend

**Naam verpleegadres O an..70**

*xml tag:* NmVrpladrs

Bijvoorbeeld de naam van een verpleeginrichting.

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

*code list:* Soort adres (all selected)

01 Woonadres, verblijfadres of vestigingsadres

02 Postadres cq correspondentie adres

03 Factuuradres

04 Tijdelijk adres

05 OR adres

06 Verpleegadres

**Soort verpleegadres, code O an2**

*xml tag:* SrtVrplgadrsCd

*code list:* Soort verpleegadres (all selected)

01 Ander huisadres

Bijvoorbeeld familie of vakantieadres.

02 Verpleeginstelling

Ziekenhuis, verpleeghuis, etc.

03 Camping

99 Onbekend

**Naam verpleegadres O an..70**

*xml tag:* NmVrpladrs

Bijvoorbeeld de naam van een verpleeginrichting.

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

DIENSTVERBAND 1..99, R

*werkgever - werknemer - DIENSTVERBAND*

*xml tag:* Dnstvbnd

**<u>Identificatie</u>**

**Identificatie dienstverband R an..40**

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

VERZUIM 1..99, R

*werkgever - werknemer - dienstverband - VERZUIM*

*xml tag:* Vrzm

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (subset selected)

02 Gewijzigd

04 Ter identificatie en/ of ter informatie

05 Correctie

**<u>Identificatie</u>**

**Verzuimgeval identificatie R an..40**

*xml tag:* VrzmgvlId

Unieke identificatie van het verzuimgeval.

Uniek per werkgever ook in de tijd.

**<u>Data</u>**

**Datum eerste verzuimdag R an10**

*xml tag:* DatEerstVrzmdg

De eerste dag waarop iemand zou moeten werken maar verzuimt, of
verminderd inzetbaar is, wegens ziekte of een ongeval. Is er sprake van
ziekte of een ongeval tijdens zwangerschaps- en bevallingsverlof en
waarvoor men nog verzuimt na beëindiging van dat verlof, dan is de
aanvangsdatum de dag waarop men zou moeten werken na beëindiging van de
zwangerschaps- en bevallingsuitkering. Tijdens regulier verlof wordt het
ziekteverzuim ook meegeteld.

Bron:

Berekening van ziekteverzuim

NVS Standaard voor verzuimregistratie

Nationale Verzuimstatistiek

November 2004

**<u>Gegevens over verzuim</u>**

**Datum einde verzuimbegeleiding O an10**

*xml tag:* DatEndVrzmBeg

**Reden einde verzuimbegeleiding,code O an2**

*xml tag:* RdnEndVrzmBegeleidingCd

*code list:* Reden einde verzuimbeleiding (all selected)

01 Hersteld

02 Overleden

03 Uit dienst

04 Overgang naar WAZO

05 Einde Arbocontract

06 Overdracht naar UWV

99 Onbekend

WERKHERVATTINGSADVIES 0..99, O

*werkgever - werknemer - dienstverband - verzuim -
WERKHERVATTINGSADVIES*

*xml tag:* WrkHrvAdv

Het werkhervattingsadvies zoals afgegeven door een Arbo-arts.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code R an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (subset selected)

01 Nieuw

03 Vervallen

05 Correctie

**Identificatie werkhervattingsadvies bij Arbodienst R an..40**

*xml tag:* IdWrkHrvAdv

De identificatiecode die de arbodienst heeft aangeleverd waardoor dit
advies wordt onderscheden van andere adviezen in de administratie van de
arbodienst.

**Datum werkhervattingsadvies R an10**

*xml tag:* DatWerkhervattingsadvies

WERKHERVATTINGSPERIODE 1..99, R

*werkgever - werknemer - dienstverband - verzuim -
werkhervattingsadvies - WERKHERVATTINGSPERIODE*

*xml tag:* WrkHrvPer

Periode waar het werkhervattingsadvies betrekking op heeft.

**<u>Periode geldig</u>**

**Ingangsdatum R an10**

*xml tag:* Ingdat

**Einddatum O an10**

*xml tag:* Enddat

**<u>Gegevens advies</u>**

**Percentage ziek conform werkhervattingsadvies R n..6,2**

*xml tag:* PercZiekConformWerkhervattingsadvies

ACTIE 0..99, O

*werkgever - werknemer - dienstverband - verzuim - ACTIE*

*xml tag:* Actie

**<u>Identificatie actie</u>**

**Datum Poortwachtactie R an10**

*xml tag:* DatPoortwActie

**Poortwachteractie, code R an2**

*xml tag:* PoortwachteractieCd

*code list:* Poortwachter actie (all selected)

01 Melden verzuim bij arbodienst

02 Gehoor geven aan oproepen bedrijfsarts

03 Opstellen plan van aanpak

04 Uitvoeren acties plan van aanpak

05 Opvolgen aanwijzingen bedrijfsarts (interventies)

06 Opvolgen aanwijzingen bedrijfsarts (deel)herstel

07 Plan van aanpak

08 Probleemanalyse

09 Eerstejaars evaluatie
