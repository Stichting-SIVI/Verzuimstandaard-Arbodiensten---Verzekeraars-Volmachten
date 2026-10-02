**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Verwerking*

Functional message: ***Verwerkingsmelding arbo-verz 2025***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

4 juli 2025

Summary

Bericht algemeen 1..1, V

Verwerkingsmelding 1..\*, V

1 Vrije Tekst 0..1, F

BERICHT ALGEMEEN 1..1, V

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code V an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00901 Verwerkingsmelding arbo - verz

**Versienummer bericht, code V an..5**

*xml tag:* VnrBrCd

*code list:* Versienummer bericht (subset selected)

00001 Versienummer 1

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

**Berichtreferentienummer ingezonden bericht V an..512**

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

VERWERKINGSMELDING 1..\*, V

*VERWERKINGSMELDING*

*xml tag:* VrwrkMld

**<u>Verwerkbaarheid</u>**

**Verwerkbaarheid, code V an2**

*xml tag:* VrwrkbhdCd

Een code die aangeeft of het ingezonden verzuim verwerkbaar is.

*code list:* Verwerkbaarheid (all selected)

01 Melding verwerkbaar

02 Uitval melding

03 Waarschuwing

**<u>Identificatie verzuimmelding</u>**

**Verzuimgeval identificatie V an..40**

*xml tag:* VrzmgvlId

Unieke identificatie van het verzuimgeval voor één dienstverband. Als
een werknemer verzuim heeft op meerdere dienstverbanden, geldt per
dienstverband een unieke "Verzuimgeval identificatie".

Uniek per werkgever ook in de tijd.

**Verzuimgeval volgnummer melding V n..3**

*xml tag:* VrzmgvlVnrMld

De meldingen bij het verzuimgeval worden oplopend in de tijd genummerd.

De nummers moeten wel oplopen, maar hoeven niet op te lopen vanaf 1 en
iedere keer opgehoogd te worden met de waarde 1.

**<u>Identificatie werkgever</u>**

**Aansluitnummer gegevensuitwisseling Arbodienst V an..70**

*xml tag:* AansltnrGeguitwlngArbdnst

Het aansluitnummer voor de gegevensuitwisseling dat de arbodienst heeft
aangeleverd aan de werkgever waardoor de werkgever wordt onderscheden
van andere werkgevers in de administratie van de arbodienst.

**Identificatie werkgever bij arbodienst V an..40**

*xml tag:* IdWrkgvrArbdnst

De identificatiecode die de arbodienst heeft aangeleverd aan de
werkgever waardoor de werkgever wordt onderscheden van andere werkgevers
in de administratie van de arbodienst.

**<u>Identificatie bij verzekeraar</u>**

**Identificatie werkgever bij verzekeraar V an..40**

*xml tag:* IDWrkgvrVerzekeraar

**<u>Melding</u>**

**Controle, code V an5**

*xml tag:* CtrlCd

Unieke code die de fout of waarschuwing identificeert. Het overzicht van
Verzuimcontrolecodes is gepubliceerd op de SIVI-website.

*code list:* SIVI meldingscodes (all selected)

*The codes of this codelist are documented in a separate document*

**Meldingstekst V an..512**

*xml tag:* MldngTkst

De meldingstekst die corrspondeert met de verzuimfoutcodelijst op de
SIVI-website.

VRIJE TEKST 0..1, F

*verwerkingsmelding - VRIJE TEKST*

*xml tag:* VrTkst

Vrije tekst om een nadere toelichting te geven.

**<u>Tekst</u>**

**Vrije tekst V an..512**

*xml tag:* VrijeTekst
