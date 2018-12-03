# NVDB

Nasjonal vegdatabank (NVDB) er et datasystem som inneholder informasjon om det norske vegnettet og er Statens vegvesens hovedkilde for informasjon om vegen og objekter på og langs vegen. NVDB skal til enhver tid inneholde reell og relevant informasjon med forutsigbar kvalitet. 

Vegnettet er representert geometrisk og topologisk for alle landets bilveger med lengde over 50 meter, samt en stor andel av gang/sykkelveger. NVDB er primærkilde for et nasjonalt digitalt navigerbart vegnett. 

## Innhold i NVDB

Det finnes i overkant av 400 ulike typer av fagdata - vegobjekttyper - knyttet til vegnettet. Eksempler på vegobjekttyper i NVDB er:

* Inventarregister over utstyr som befinner seg på, i, under og langs vegen: Rekkverk, Skilt, Stikkrenner, Vegdekke, Vegoppmerking, Elektrisk anlegg, ... 
* Administrativ informasjon: Fartsgrenser, Bruksklasser, ...
* Hendelser: Trafikkulykker, Skred, ...
* Målinger/Måleserier: Nedbøyingsmålinger, Friksjonsmålinger, ...
* Statistikk: Trafikkmengde, Jevnhet, Spor, Vegbredde, ...
* Beregninger: Kurvatur, Vegbredde, ...

## Stedfesting
NVDB inneholder stedfestet informasjon. Alle vegobjekter i NVDB må være stedfestet til vegnettet. Vegnettet er bygget opp av veglenker og noder. I NVDB er det denne nettverksstrukturen som er grunnlaget for all stedfesting av fagobjekter. Veglenkene har også nøyaktig kurvegeometri som beskriver deres posisjon i verden. 

Vegobjektene kan også ha egengeometri som angir objektets nøyaktige posisjon. I tilfeller der et vegobjekt ikke har egen, innmålt geometri (f.eks. Fartsgrenser, bruksklasser m.fl.), så kan det avledes en geometrisk plassering for vegobjektet basert på objektets stedfesting i vegnettet. 

I tillegg er det lagt et metrert lineært referansesystem oppå selve vegnettet - det Nasjonale Vegreferansesystemet. Vegreferansen utgjør en brukervennlig betegnelse på et punkt i vegnettet og blir brukt ved oppslag mot NVDB, ved rapportering og i enkelte tilfeller ved registreringer ute på vegen. Vegreferansen er som alle andre vegobjekttyper stedfestet på vegnettet. Selve vegreferanseobjektene har ikke egengeometri, men deres plassering i verden kan avledes av geometrien til veglenkene de er stedfestet på.

Eksempel: https://www.vegvesen.no/nvdb/api/v2/vegobjekter/5/862633699

## Datakatalogen

Alle vegobjekttyper i NVDB er definert i Datakatalogen. Datakatalogen definerer hvilke fagdata det er mulig å legge inn i NVDB, den kan sees på som et detaljert innholdsregister for NVDB. Datakatalogen definerer alle vegobjekttyper detaljert, med sine egenskaper og styringsparametre, samt relasjoner til andre vegobjekter. 

* https://www.vegvesen.no/fag/teknologi/nasjonal+vegdatabank/datakatalogen
* https://datakatalogen.vegdata.no/

## Vegkart

Innsynsløsning for NVDB. Start her for rask oversikt over innhold og snarveger til APIet

* http://www.vegkart.no


## API

* https://www.vegvesen.no/nvdb/api/v2
* http://api.vegdata.no/ 

### API - Eksempelklienter

* JAVA: https://github.com/nvdb-vegdata/nvdb-api-client
* PYTHON: https://github.com/LtGlahn/nvdbapi-V2
* PYTHON: https://github.com/Acurus/pnvdb
