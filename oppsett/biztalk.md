## Installasjon av BizTalk Server


### Miljø


BizTalk 2013 var bygget for SQL Server 2008, og er kanskje oppdatert til SQL Server 2012, men er ikke "fremover kompatible" nødvendigviss.  Installasjon på SQL Server 2014 var litt vanskelig.

SQL Server 2008 Management Tools (Basic & Complete) er et krav for å få Data Transformation Services på maskinen, som er igjen et krav til BAM Tools installasjon.


### Developer SDK & Templates

BizTalk 2013 krever Visual Studio 2012 for å installere sitt SDK.  En løsning for å installare den med VS2015+ er beskrevet på http://stackoverflow.com/questions/31337396/biztalk-2013-r2-installation


### Configuration

Ved konfigurasjon av installasjonen ga "Groups" og "Enterprise Single Sign On" forskjellige klager om servernavnet til en lokal SQL 2014 instanse.  "Avansert konfigurasjon" og en blanding av servernavn (maskinnavn og localhost), var løsningen.


#### Konfigurasjonsrekkefølgen

I BizTalk sin hovedinstaller kan man forsøke å konfigurere løsningen.  Rekkefølgen av komponentene påvirker installasjonslogikk.  Fikk feil på Group konfigurasjon med Regel motoren alerede installert.  Installere komponentene i rekkefølgen de presenteres.


### Bruker Roller

Flere forskjellige bruker kontorer trenges for BizTalk oppsettet.  Tjeneste kontoer for meldingsplatformen og regel motoroen.
