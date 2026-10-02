**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Basistransactie Verzuim*

Functional message: ***Verzuimrapportage Arbodienst -\> Verzekeraar
2024***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

3 juli 2024

Summary

Bericht algemeen 1..1, V

Werkgever 1..\*, V

1 Werknemer 1..\*, V

2 Dienstverband 1..99, V

3 Verzuim 1..99, V

4 Werkhervattingsadvies 0..99, F

5 Werkhervattingsperiode 1..99, V

4 Actie 0..99, F

BERICHT ALGEMEEN 1..1, V

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code V an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00704 Verzuimrapportage Arbodienst --\> Verzekeraar

**Versienummer bericht, code V an..5**

*xml tag:* VnrBrCd

*code list:* Versienummer bericht (subset selected)

00003 Versienummer 3

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

**<u>Verslagperiode</u>**

**Ingangsdatum Verslagperiode F an10**

*xml tag:* IngdatVerslagperiode

**Einddatum verslagperiode F an10**

*xml tag:* EnddatVerslagperiode

WERKGEVER 1..\*, V

*WERKGEVER*

*xml tag:* Wrkgvr

Bij het beschrijven van de kenmerken van de Werkgever wordt in een
aantal gevallen de term Inhoudingsplichtige gebruikt.

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

**Identificatie werkgever bij arbodienst V an..40**

*xml tag:* IdWrkgvrArbdnst

De identificatiecode die de arbodienst heeft aangeleverd aan de
werkgever waardoor de werkgever wordt onderscheden van andere werkgevers
in de administratie van de arbodienst.

**Aansluitnummer gegevensuitwisseling Arbodienst V an..70**

*xml tag:* AansltnrGeguitwlngArbdnst

Het aansluitnummer voor de gegevensuitwisseling dat de arbodienst heeft
aangeleverd aan de werkgever waardoor de werkgever wordt onderscheden
van andere werkgevers in de administratie van de arbodienst.

**<u>Identificatie bij verzekeraar</u>**

**Identificatie werkgever bij verzekeraar F an..40**

*xml tag:* IDWrkgvrVerzekeraar

**<u>Loonbelasting / loonheffingen</u>**

**Loonheffingennummer F an..12**

*xml tag:* Lhnr

Een door de Belastingdienst toegekende identificatie voor de
administratieve eenheid waaronder de werkgever bekend is en
loonheffingen afdraagt.

WERKNEMER 1..\*, V

*werkgever - WERKNEMER*

*xml tag:* Wrknmr

Een werknemer is de natuurlijke persoon met wie een inkomstenverhouding
binnen de loonadministratie bestaat.

**<u>Identificatie</u>**

**Identificatie werknemer V an..40**

*xml tag:* IdWrknmr

Een unieke identificatie van de werknemer bij de werkgever. Een eenmaal
uitgegeven identificatie wordt niet hergebruikt.

**Identificatie werknemer arbodienst F an..40**

*xml tag:* IdWrknmrArbdnst

**Identificatie werknemer verzekeraar F an..40**

*xml tag:* IdWrknmrVzkr

DIENSTVERBAND 1..99, V

*werkgever - werknemer - DIENSTVERBAND*

*xml tag:* Dnstvbnd

**<u>Identificatie</u>**

**Identificatie dienstverband V an..40**

*xml tag:* IdDnstvbnd

Unieke code voor het dienstverband van de werknemer.

**<u>Personeelsnummer behorende bij het dienstverband</u>**

**Personeelsnummer F an..35**

*xml tag:* PersNr

De code waarmee de natuurlijk persoon in de administratie van de
inhoudingsplichtige bekend is.

Bron: Loonaangifte.

VERZUIM 1..99, V

*werkgever - werknemer - dienstverband - VERZUIM*

*xml tag:* Vrzm

**<u>Identificatie</u>**

**Verzuimgeval identificatie V an..40**

*xml tag:* VrzmgvlId

Unieke identificatie van het verzuimgeval voor één dienstverband. Als
een werknemer verzuim heeft op meerdere dienstverbanden, geldt per
dienstverband een unieke "Verzuimgeval identificatie".

Uniek per werkgever ook in de tijd.

**<u>Data</u>**

**Datum eerste verzuimdag V an10**

*xml tag:* DatEerstVrzmdg

De eerste dag waarop iemand zou moeten werken maar verzuimt, of
verminderd inzetbaar is, wegens ziekte of een ongeval. Is er sprake van
ziekte of een ongeval tijdens zwangerschaps- en bevallingsverlof en
waarvoor men nog verzuimt na beëindiging van dat verlof, dan is de
aanvangsdatum de dag waarop men zou moeten werken na beëindiging van de
zwangerschaps- en bevallingsuitkering. Tijdens regulier verlof wordt het
ziekteverzuim ook meegeteld.

Datum mag niet in de toekomst liggen.

Bron:

Berekening van ziekteverzuim

NVS Standaard voor verzuimregistratie

Nationale Verzuimstatistiek

November 2004

**<u>Gegevens over verzuim</u>**

**Datum einde verzuimbegeleiding F an10**

*xml tag:* DatEndVrzmBeg

**Reden einde verzuimbegeleiding,code F an2**

*xml tag:* RdnEndVrzmBegeleidingCd

*code list:* Reden einde verzuimbeleiding (all selected)

01 Hersteld

02 Overleden

03 Uit dienst

04 Overgang naar WAZO

05 Einde Arbocontract

06 Overdracht naar UWV

99 Onbekend

WERKHERVATTINGSADVIES 0..99, F

*werkgever - werknemer - dienstverband - verzuim -
WERKHERVATTINGSADVIES*

*xml tag:* WrkHrvAdv

Het werkhervattingsadvies zoals afgegeven door een Arbo-arts.

**<u>Wijze waarop de gegevens verwerkt moeten worden</u>**

**Verwerking, code V an2**

*xml tag:* VrwrkCd

*code list:* Verwerkingscode (subset selected)

01 Nieuw

03 Vervallen

04 Ter identificatie en/ of ter informatie

05 Correctie

**Identificatie werkhervattingsadvies bij Arbodienst V an..40**

*xml tag:* IdWrkHrvAdv

De identificatiecode die de arbodienst heeft aangeleverd waardoor dit
advies wordt onderscheden van andere adviezen in de administratie van de
arbodienst.

**Datum werkhervattingsadvies V an10**

*xml tag:* DatWerkhervattingsadvies

WERKHERVATTINGSPERIODE 1..99, V

*werkgever - werknemer - dienstverband - verzuim -
werkhervattingsadvies - WERKHERVATTINGSPERIODE*

*xml tag:* WrkHrvPer

Periode waar het werkhervattingsadvies betrekking op heeft.

**<u>Periode geldig</u>**

**Ingangsdatum V an10**

*xml tag:* Ingdat

**Einddatum F an10**

*xml tag:* Enddat

De datum van de laatste dag waarop de gegevens geldig zijn.

**<u>Gegevens advies</u>**

**Percentage ziek conform werkhervattingsadvies V n..6,2**

*xml tag:* PercZiekConformWerkhervattingsadvies

ACTIE 0..99, F

*werkgever - werknemer - dienstverband - verzuim - ACTIE*

*xml tag:* Actie

**<u>Identificatie actie</u>**

**Datum Poortwachtactie V an10**

*xml tag:* DatPoortwActie

**Poortwachteractie, code V an2**

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
