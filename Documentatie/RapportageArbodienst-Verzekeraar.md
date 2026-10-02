**Functional message: Hierarchic**

Business chain: *Verzuim Datamodel*

Transaction type: *Basis Arbodienst Verzekeraar*

Functional message: ***Rapportage Arbodienst -\> Verzekeraar 2024***

Actor group: *Arbodiensten Verzekeraars*

XML Tag Set: *Standard XML*

**Copyright SIVI**

3 juli 2024

Summary

Bericht algemeen 1..1, V

Verzekeraar/Volmacht 0..1, F

Arbodienst 0..1, F

Verslagperiode 1..999, V

1 Rapportage 1..1, V

BERICHT ALGEMEEN 1..1, V

*BERICHT ALGEMEEN*

*xml tag:* BrAlg

**<u>Soort bericht + versienummer</u>**

**Bericht, code V an..5**

*xml tag:* BrCd

*code list:* Berichtcode (subset selected)

00703 Managementrapportage

**Versienummer bericht, code V an..5**

*xml tag:* VnrBrCd

*code list:* Versienummer bericht (subset selected)

00002 Versienummer 2

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

*code list:* Logische eenheid (all selected)

J Ja

N Nee

O Onbekend

**<u>Ontvangstbevestiging</u>**

**Ontvangstbevestiging gewenst J/N V a1**

*xml tag:* OntvngstbevJN

Geeft aan of de inzender van het bericht een ontvangstbevestiging wenst.

*code list:* Logische eenheid (all selected)

J Ja

N Nee

O Onbekend

VERZEKERAAR/VOLMACHT 0..1, F

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

ARBODIENST 0..1, F

*ARBODIENST*

*xml tag:* Arbdnst

**<u>Handelsnaam</u>**

**Handelsnaam organisatie V an..100**

*xml tag:* HndlsnmOrg

De naam waaronder een organisatie aan het maatschappelijk verkeer
deelneemt.

Norminstantie: SUWI

**<u>Arbo-dienst</u>**

**Arbodienst, code F an3**

*xml tag:* ArbdnstCd

De lijst met codes van gecertificeerde Arbodiensten is gepubliceerd op
de website van SIVI. Zie www.sivi.org.

*code list:* Code Arbodienst (all selected)

*The codes of this codelist are documented in a separate document*

VERSLAGPERIODE 1..999, V

*VERSLAGPERIODE*

*xml tag:* Verslagperiode

**Ingangsdatum V an10**

*xml tag:* Ingdat

**Einddatum V an10**

*xml tag:* Enddat

De datum van de laatste dag waarop de gegevens geldig zijn.

RAPPORTAGE 1..1, V

*verslagperiode - RAPPORTAGE*

*xml tag:* Rapportage

**<u>Algemeen</u>**

**Aantal klanten V n..7**

*xml tag:* AantalKlanten

**Aantal werknemers F n..7**

*xml tag:* AantalMeldingen

**<u>Aantal meldingen</u>**

**Aantal verzuimmeldingen F n..7**

*xml tag:* AantalVerzuimmeldingen

**Aantal verzuimdagen F n..7**

*xml tag:* AantalVerzuimdagen

**Verzuimpercentage F n..6,2**

*xml tag:* Verzuimpercentage

**Verzuimfrequentie F n..7**

*xml tag:* Verzuimfrequentie

**Aantal deelherstelmeldingen F n..7**

*xml tag:* AantalDeelherstelmeldingen

**Percentage deelherstelmeldingen F n..6,2**

*xml tag:* PercentageDeelherstelmeldingen

**Aantal herstelmeldingen F n..7**

*xml tag:* AantalHerstelmeldingen

**Percentage herstelmeldingen F n..6,2**

*xml tag:* PercentageHerstelmeldingen

**Aantal meldingen regres F n..7**

*xml tag:* AantalMeldingenRegres

**<u>Verzuimduur</u>**

**Gemiddelde verzuimduur (gesloten dossiers) F n..7**

*xml tag:* GemiddeldeVerzuimduur

**Ziekteverzuimpercentage 1-7 dgn F n..6,2**

*xml tag:* ZiekteverzuimpercentageKort

**Ziekteverzuimpercentage 8-42 dgn F n..6,2**

*xml tag:* ZiekteverzuimpercentageMiddellang

**Ziekteverzuimpercentage 43-365 dgn F n..6,2**

*xml tag:* ZiekteverzuimpercentageLang

**Ziekteverzuimpercentage \>365 dgn F n..6,2**

*xml tag:* ZiekteverzuimpercentageExtraLang

**Aantal meldingen verzuim 1-7 werkdagen F n..7**

*xml tag:* AantalMeldingenVerzuimKort

**Aantal meldingen verzuim 8-42 werkdagen F n..7**

*xml tag:* AantalMeldingenVerzuimMiddellang

**Aantal meldingen verzuim 43-365 werkdagen F n..7**

*xml tag:* AantalMeldingenVerzuimLang

**Aantal meldingen verzuim \> 365 dagen F n..7**

*xml tag:* AantalMeldingenVerzuimExtraLang

**Aantal ziekdagen 1-7 werkdagen F n..7**

*xml tag:* AantalZiekdagenKort

**Aantal ziekdagen 8-42 werkdagen F n..7**

*xml tag:* AantalZiekdagenMiddellang

**Aantal ziekdagen 43-365 werkdagen F n..7**

*xml tag:* AantalZiekdagenLang

**Aantal ziekdagen \> 365 werkdagen F n..7**

*xml tag:* AantalZiekdagenExtraLang

**<u>Proces poortwachterproof</u>**

**Aantal probleemanalyses opgesteld F n..7**

*xml tag:* AantalProbleemanalysesOpgesteld

**Percentage probleemanalyses op tijd F n..6,2**

*xml tag:* PercentageProbleemanalysesOpTijd

**Aantal plannen van aanpak opgesteld F n..7**

*xml tag:* AantalPlannenVanAanpakOpgesteld

**Percentage plannen van aanpak op tijd F n..6,2**

*xml tag:* PercentagePlannenVanAanpakOpTijd

**Aantal 42 weeksmeldingen gedaan F n..7**

*xml tag:* AantalTweeenveertigWeeksmeldingenGedaan

**Percentage 42 weeksmeldingen op tijd F n..6,2**

*xml tag:* PercentageTweeenveertigWeeksmeldingenOpTijd

**Aantal eindejaarsevaluaties gedaan F n..7**

*xml tag:* AantalEindejaarsevaluatiesGedaan

**Percentage eindejaarsevaluaties op tijd F n..6,2**

*xml tag:* PercentageEindejaarsevaluatiesOpTijd

**Aantal re-integratieverslagen opgesteld F n..7**

*xml tag:* AantalReintegratieverslagenOpgesteld

**Percentage re-integratieverslagen op tijd F n..7**

*xml tag:* PercentageReintegratieverslagenOpTijd

**Aantal poortwachtersancties F n..7**

*xml tag:* AantalPoortwachtersancties

**<u>Interventies</u>**

**Aantal geadviseerde interventies F n..7**

*xml tag:* AantalGeadviseerdeInterventies

**Aantal geaccordeerde interventies F n..7**

*xml tag:* AantalGeaccordeerdeInterventies

**Aantal interventies met bijdrage Verzekeraar F n..7**

*xml tag:* AantalInterventiesMetBijdrageVerzekeraar

**Kosten interventies voor Verzekeraar F n..9,2**

*xml tag:* KostenInterventiesVootVerzekeraar

**<u>Soorten geaccordeerde interventies</u>**

**Aantal tweede spoor F n..7**

*xml tag:* AantalTweedeSpoor

**Aantal psychische interventies F n..7**

*xml tag:* AantalPsychischeInterventies

**Aantal fysieke interventies F n..7**

*xml tag:* AantalFysiekeInterventies

**Aantal multidisciplinaire interventies F n..7**

*xml tag:* AantalMultidisciplinaireInterventies

**Aantal wachtlijstbemiddelingen F n..7**

*xml tag:* AantalWachtlijstbemiddelingen

**Aantal overige internventies F n..7**

*xml tag:* AantalOverigeInterventies

**<u>Klanttevredenheid</u>**

**Werkgevertevredenheid van 0 - 10 F n..3**

*xml tag:* Werkgevertevredenheid

**Aantal gemelde klachten F n..7**

*xml tag:* AantalGemeldeKlachten

**Aantal terechte klachten F n..7**

*xml tag:* AantalTerechteKlachten

**Percentage terechte klachten F n..6,2**

*xml tag:* PercentageTerechteKlachten
