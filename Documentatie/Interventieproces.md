**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Basistransactie Verzuim*

Functional message: ***Interventieproces 2025***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

4 juli 2025

Summary

Bericht algemeen 1..1, V

Werkgever 1..\*, V

1 Werknemer 1..\*, V

2 Dienstverband 1..99, V

3 Arbeidsrelatie 0..1, F

3 Verzuim 1..99, V

BERICHT ALGEMEEN 1..1, V

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code V an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00801 Interventieproces

**Versienummer bericht, code V an..5**

*xml tag:* VnrBrCd

*code list:* Versienummer bericht (subset selected)

00001 Versienummer 1

**Functie bericht, code V an2**

*xml tag:* FunctieBrCd

*code list:* SIVI (subset selected)

05 Indicatie interventie arbodienst --\> verzekeraar

06 Interventiegegevens verzekeraar --\> arbodienst

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

**<u>Eigenrisicodragerschap</u>**

**Indicatie eigenrisicodrager voor de WGA F a1**

*xml tag:* IndERDWGA

Aanduiding of de Inhoudingsplichtige eigenrisicodrager (ERD) is voor de
WGA.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

**Indicatie eigenrisicodrager voor de ZW F a1**

*xml tag:* IndERDZW

Aanduiding of de Inhoudingsplichtige eigenrisicodrager (ERD) is voor de
ZW.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

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

**<u>Berekende kolommen</u>**

**Loon LB/PH F n..9,2**

*xml tag:* LnLbPh

Het loon waarover de loonbelasting/premie volksverzekeringen wordt
berekend.

Geheel conform kolom 14 van de loonstaat.

Bron: Loonaangifte.

**Loon SV F n..9,2**

*xml tag:* LnSV

Het loon voor de werknemersverzekeringen.

Geheel conform kolom 8 van de loonstaat. Dit is het loon zonder rekening
te houden met maximumpremieloon en franchise. Vul 0 in als de werknemer
niet verzekerd is voor de werknemersverzekeringen.

Bron: Loonaangifte.

ARBEIDSRELATIE 0..1, F

*werkgever - werknemer - dienstverband - ARBEIDSRELATIE*

*xml tag:* Arbeidsrelatie

De betrekking tussen werkgever en werknemer die ontstaat bij loonarbeid
na afsluiting van een arbeidsovereenkomst.

Dit wordt ook wel aanstelling genoemd.

**<u>Identificerende gegevens arbeidsrelatie</u>**

**Identificatie arbeidsrelatie V an..40**

*xml tag:* IdArbeidsrelatie

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

**<u>Inloop/uitloop</u>**

**Inloop J/N F a1**

*xml tag:* InloopJN

Een indicatie dat inloop van toepassing is. Hierbij zijn de
interventiekosten gedekt, ook als de ingangsdatum van verzuim van vóór
het verzuimcontract is.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

**Uitloop J/N F a1**

*xml tag:* UitloopJN

Indicatie dat uitloop van toepassing is. Hierbij zijn de
interventiekosten gedekt, ook als verzuim doorloopt na beëindiging van
het contract.

*code list:* Logische eenheid (subset selected)

J Ja

N Nee

**<u>Interventie</u>**

**Interventie J/N V a1**

*xml tag:* InterventieJN

Indicatie dat een interventietraject loopt. De betrokken arbodienst
heeft hierbij actuele gegevens nodig voor de kosten-batenanalyse.
