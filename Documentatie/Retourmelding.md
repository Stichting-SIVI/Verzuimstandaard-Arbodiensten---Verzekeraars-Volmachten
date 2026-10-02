**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Basistransactie Verzuim*

Functional message: ***Retourmelding 2026***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

24 juni 2026

Summary

Bericht algemeen 1..1, V

Foutmelding 0..\*, F

BERICHT ALGEMEEN 1..1, V

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code V an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

99999 Retourmelding

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

**<u>Retourmelding</u>**

**Soort retourmelding, code V an2**

*xml tag:* SrtRetmldngCd

*code list:* Soort Retourmelding (subset selected)

02 Bericht kan verwerkt worden

03 Bericht kan niet verwerkt worden

FOUTMELDING 0..\*, F

*FOUTMELDING*

*xml tag:* Foutmldng

**Soort fout, code V an2**

*xml tag:* SrtFoutCd

*code list:* Soort fout (subset selected)

01 Berichttype mag niet verstuurd worden door inzender

06 Ongeldige waarden in een of meer elementen

99 Overig

**Toelichting F an..512**

*xml tag:* Toelchtng
