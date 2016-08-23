## Installasjon av BizTalk Server


### Developer SDK & Templates

BizTalk 2013 krever Visual Studio 2012 for å installere sitt SDK.  En løsning for å installare den med VS2015+ er beskrevet på http://stackoverflow.com/questions/31337396/biztalk-2013-r2-installation


### Configuration

Ved konfigurasjon av installasjonen ga "Groups" og "Enterprise Single Sign On" forskjellige klager om servernavnet til en lokal SQL 2014 instanse.  "Avansert konfigurasjon" og en blanding av servernavn (maskinnavn og localhost), var løsningen.
