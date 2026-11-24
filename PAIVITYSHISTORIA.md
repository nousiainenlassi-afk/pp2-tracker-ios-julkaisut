# Päivityshistoria

Uusin versio on ylhäällä. Asennusohjeet ovat [etusivulla](README.md). Päivitys asennetaan
samalla tavalla kuin ensiasennus: asenna uusi IPA vanhan päälle samalla Apple ID:llä, niin
tietoja ei menetä. Lopeta ensin näytön tallennus ja aloita se päivityksen jälkeen uudelleen.

## 0.10 (24.11.2026)

- **Lajin korjaus:** jos sama kala luetaan ensin väärällä lajilla ja hetken päästä oikein,
  se lasketaan yhtenä kalana (ennen se saattoi laskeutua kahdesti).
- **Ä-kirjaimen lukuvirheet:** esim. puronieriä ja harmaanieriä tunnistetaan, vaikka ä luettaisiin väärin.
- **Siika:** "SUKA"-lukuvirhe tulkitaan siiaksi eikä sulkavaksi.

## 0.9 (10.11.2026) – ensimmäinen julkinen testiversio

- Kalat (laji ja paino) luetaan pelin ruudulta ja lasketaan kisan sääntöjen mukaan.
- 30 kisatyyppiä tunnistetaan automaattisesti, ja kisatyypin voi valita myös käsin.
- Järvi tunnistetaan latausruudusta ja tulosnäytöstä, ja sen voi valita käsin.
- Laskuri nollautuu uuden kisan alussa.
- Tuntemattoman lajin kala lasketaan pelin aikana lajilla "tuntematon", jotta kokonaispaino täsmää.
- Osittain näkyvä paino (viesti vielä liukumassa paneeliin) hylätään.
- Pieni kelluva ikkuna: pisteet, kappaleet ja viimeisin kala.
- Lokin kopiointi ja jakaminen vikaraporttia varten.
