**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Basistransactie Verzuim*

Functional message: ***Retourmelding 2022***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

1 juli 2022

Summary

Bericht algemeen 1..1, R

Foutmelding 0..\*, O

BERICHT ALGEMEEN 1..1, R

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code R an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

99999 Retourmelding

**Versienummer bericht, code R an..5**

*xml tag:* VnrBrCd

*code list:* Versienummer bericht (subset selected)

00002 Versienummer 2

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

**Berichtreferentienummer ingezonden bericht R an..512**

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

**<u>Retourmelding</u>**

**Soort retourmelding, code R an2**

*xml tag:* SrtRetmldngCd

*code list:* Soort Retourmelding (all selected)

01 Bericht is ontvangen

02 Bericht kan verwerkt worden

03 Bericht kan niet verwerkt worden

04 Bericht is verwerkt

FOUTMELDING 0..\*, O

*FOUTMELDING*

*xml tag:* Foutmldng

**Soort fout, code R an2**

*xml tag:* SrtFoutCd

*code list:* Soort fout (all selected)

01 Berichttype mag niet verstuurd worden door inzender

02 Niet herkenbaar bericht

03 Fout in de tekenset

04 Fout in de opbouw van het bericht

05 Een of meer verplichte gegevens ontbreken

06 Ongeldige waarden in een of meer elementen

99 Overig

**Toelichting O an..512**

*xml tag:* Toelchtng
