**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel ~~~~*

Transaction type: *Basis Arbodienst Verzekeraar ~~~~*

Functional message: ***Rapportage Arbodienst -\> Verzekeraar* *~~2021~~*
*2022***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

~~25 juni 2021~~

1 juli 2022

Summary

Bericht algemeen 1..1, R

Verzekeraar/Volmacht 0..1, O

Arbodienst 0..1, O

Verslagperiode 1..999, R

1 Rapportage 1..1, R

BERICHT ALGEMEEN 1..1, R

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code R an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00703 Managementrapportage

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

**<u>Testindicatie</u>**

**Test J/N R a1**

*xml tag:* TestJN

Geeft aan of het een testbericht betreft.

*code list:* Logische eenheid (all selected)

J Ja

N Nee

O Onbekend

**<u>Ontvangstbevestiging</u>**

**Ontvangstbevestiging gewenst J/N R a1**

*xml tag:* OntvngstbevJN

Geeft aan of de inzender van het bericht een ontvangstbevestiging wenst.

*code list:* Logische eenheid (all selected)

J Ja

N Nee

O Onbekend

VERZEKERAAR/VOLMACHT 0..1, O

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

ARBODIENST 0..1, O

*ARBODIENST*

*xml tag:* Arbdnst

**<u>Handelsnaam</u>**

**Handelsnaam organisatie R an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

**<u>Arbo-dienst</u>**

**Arbodienst, code O an3**

*xml tag:* ArbdnstCd

De lijst met codes van gecertificeerde Arbodiensten is gepubliceerd op
de website van SIVI. Zie www.sivi.org.

*code list:* Code Arbodienst (all selected)

*The codes of this codelist are documented in a separate document*

VERSLAGPERIODE 1..999, R

*VERSLAGPERIODE*

*xml tag:* Verslagperiode

**Ingangsdatum R an10**

*xml tag:* Ingdat

**Einddatum R an10**

*xml tag:* Enddat

De datum van de laatste dag waarop de gegevens geldig zijn.

RAPPORTAGE 1..1, R

*verslagperiode - RAPPORTAGE*

*xml tag:* Rapportage

**<u>Algemeen</u>**

**Aantal klanten R n..7**

*xml tag:* AantalKlanten

**Aantal werknemers O n..7**

*xml tag:* AantalMeldingen

**<u>Aantal meldingen</u>**

**Aantal verzuimmeldingen O n..7**

*xml tag:* AantalVerzuimmeldingen

**Aantal verzuimdagen O n..7**

*xml tag:* AantalVerzuimdagen

**Verzuimpercentage O n..6,2**

*xml tag:* Verzuimpercentage

**Verzuimfrequentie O n..7**

*xml tag:* Verzuimfrequentie

**Aantal deelherstelmeldingen O n..7**

*xml tag:* AantalDeelherstelmeldingen

**Percentage deelherstelmeldingen O n..6,2**

*xml tag:* PercentageDeelherstelmeldingen

**Aantal herstelmeldingen O n..7**

*xml tag:* AantalHerstelmeldingen

**Percentage herstelmeldingen O n..6,2**

*xml tag:* PercentageHerstelmeldingen

**Aantal meldingen regres O n..7**

*xml tag:* AantalMeldingenRegres

**<u>Verzuimduur</u>**

**Gemiddelde verzuimduur (gesloten dossiers) O n..7**

*xml tag:* GemiddeldeVerzuimduur

**Ziekteverzuimpercentage 1-7 dgn O n..6,2**

*xml tag:* ZiekteverzuimpercentageKort

**Ziekteverzuimpercentage 8-42 dgn O n..6,2**

*xml tag:* ZiekteverzuimpercentageMiddellang

**Ziekteverzuimpercentage 43-365 dgn O n..6,2**

*xml tag:* ZiekteverzuimpercentageLang

**Ziekteverzuimpercentage \>365 dgn O n..6,2**

*xml tag:* ZiekteverzuimpercentageExtraLang

**Aantal meldingen verzuim 1-7 werkdagen O n..7**

*xml tag:* AantalMeldingenVerzuimKort

**Aantal meldingen verzuim 8-42 werkdagen O n..7**

*xml tag:* AantalMeldingenVerzuimMiddellang

**Aantal meldingen verzuim 43-365 werkdagen O n..7**

*xml tag:* AantalMeldingenVerzuimLang

**Aantal meldingen verzuim \> 365 dagen O n..7**

*xml tag:* AantalMeldingenVerzuimExtraLang

**Aantal ziekdagen 1-7 werkdagen O n..7**

*xml tag:* AantalZiekdagenKort

**Aantal ziekdagen 8-42 werkdagen O n..7**

*xml tag:* AantalZiekdagenMiddellang

**Aantal ziekdagen 43-365 werkdagen O n..7**

*xml tag:* AantalZiekdagenLang

**Aantal ziekdagen \> 365 werkdagen O n..7**

*xml tag:* AantalZiekdagenExtraLang

**<u>Proces poortwachterproof</u>**

**Aantal probleemanalyses opgesteld O n..7**

*xml tag:* AantalProbleemanalysesOpgesteld

**Percentage probleemanalyses op tijd O n..6,2**

*xml tag:* PercentageProbleemanalysesOpTijd

**Aantal plannen van aanpak opgesteld O n..7**

*xml tag:* AantalPlannenVanAanpakOpgesteld

**Percentage plannen van aanpak op tijd O n..6,2**

*xml tag:* PercentagePlannenVanAanpakOpTijd

**Aantal 42 weeksmeldingen gedaan O n..7**

*xml tag:* AantalTweeenveertigWeeksmeldingenGedaan

**Percentage 42 weeksmeldingen op tijd O n..6,2**

*xml tag:* PercentageTweeenveertigWeeksmeldingenOpTijd

**Aantal eindejaarsevaluaties gedaan O n..7**

*xml tag:* AantalEindejaarsevaluatiesGedaan

**Percentage eindejaarsevaluaties op tijd O n..6,2**

*xml tag:* PercentageEindejaarsevaluatiesOpTijd

**Aantal re-integratieverslagen opgesteld O n..7**

*xml tag:* AantalReintegratieverslagenOpgesteld

**Percentage re-integratieverslagen op tijd O n..7**

*xml tag:* PercentageReintegratieverslagenOpTijd

**Aantal poortwachtersancties O n..7**

*xml tag:* AantalPoortwachtersancties

**<u>Interventies</u>**

**Aantal geadviseerde interventies O n..7**

*xml tag:* AantalGeadviseerdeInterventies

**Aantal geaccordeerde interventies O n..7**

*xml tag:* AantalGeaccordeerdeInterventies

**Aantal interventies met bijdrage Verzekeraar O n..7**

*xml tag:* AantalInterventiesMetBijdrageVerzekeraar

**Kosten interventies voor Verzekeraar O n..9,2**

*xml tag:* KostenInterventiesVootVerzekeraar

**<u>Soorten geaccordeerde interventies</u>**

**Aantal tweede spoor O n..7**

*xml tag:* AantalTweedeSpoor

**Aantal psychische interventies O n..7**

*xml tag:* AantalPsychischeInterventies

**Aantal fysieke interventies O n..7**

*xml tag:* AantalFysiekeInterventies

**Aantal multidisciplinaire interventies O n..7**

*xml tag:* AantalMultidisciplinaireInterventies

**Aantal wachtlijstbemiddelingen O n..7**

*xml tag:* AantalWachtlijstbemiddelingen

**Aantal overige internventies O n..7**

*xml tag:* AantalOverigeInterventies

**<u>Klanttevredenheid</u>**

**Werkgevertevredenheid van 0 - 10 O n..3**

*xml tag:* Werkgevertevredenheid

**Aantal gemelde klachten O n..7**

*xml tag:* AantalGemeldeKlachten

**Aantal terechte klachten O n..7**

*xml tag:* AantalTerechteKlachten

**Percentage terechte klachten O n..6,2**

*xml tag:* PercentageTerechteKlachten
