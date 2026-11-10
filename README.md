# PP2 Tracker iPhonelle (testiversio)

PP2 Tracker on iPhone-apuohjelma **Pro Pilkki 2** -peliin. Se katsoo pelin ruutua puhelimen
näytön tallennuksella, tunnistaa nostetut kalat (laji ja paino), tunnistaa kisatyypin ja laskee
kisan pisteet pelin sääntöjen mukaan. Tulokset näkyvät sovelluksessa ja halutessasi pienessä
kelluvassa ikkunassa pelin päällä.

> **Tärkeää:** tämä on epävirallinen harrastusprojekti eikä liity Pro Pilkki 2:n tekijöihin.
> Ohjelma on testiversio, ja siinä voi olla virheitä. Kaikki toimii vain puhelimen sisällä:
> mitään ei lähetetä internetiin.

## Miksi asennus on näin vaivalloinen? (ei App Storessa)

Ohjelma **ei ole App Storessa**, eikä sitä sinne ole tulossakaan. Apple vaatii App Storeen ja
Applen TestFlight-testaukseen maksullisen kehittäjätilin (99 dollaria vuodessa). En ole valmis
maksamaan sitä harrastusprojektin takia.

Siksi ohjelma asennetaan itse omalla ilmaisella Apple ID:llä (ns. sideloading). Sen rajoitukset:

- Asennus **vanhenee 7 päivässä**. Silloin ohjelma lakkaa avautumasta, ja sen voi asentaa uudelleen
  samalla IPA-tiedostolla. Asennus ei poista tietojasi. (Uusinnan voi tehdä automaattiseksi, ks. kohta 8.)
- Tarvitset **Windows-tietokoneen** (tai Macin), USB-kaapelin ja ilmaisen Apple ID:n.
- Jokaisen testaajan omat rajat: enintään 3 sivulatattua sovellusta kerrallaan ja 10 uutta
  sovellustunnusta viikossa. Tämä ohjelma käyttää niistä kaksi.

## Mitä tarvitset

- iPhone, jossa iOS 16 tai uudempi (testattu iPhone 13:lla, iOS 26)
- Windows-tietokone ja USB-kaapeli (Mac käy myös, ohjeet alla)
- Apple ID (ilmainen riittää). Suosittelen tekemään erillisen Apple ID:n tätä varten, jos et halua
  käyttää omaa tunnustasi.
- Pro Pilkki 2 asennettuna puhelimeen

## 1. Lataa ohjelma

Lataa uusin **PP2Tracker.ipa** tämän repon [Releases-sivulta](../../releases/latest).
Älä pura tiedostoa: se asennetaan sellaisenaan.

## 2. Asenna tietokoneelle tarvittavat ohjelmat (Windows)

1. Asenna **Apple Devices** -sovellus Microsoft Storesta (tai iTunes Applen sivuilta). Se asentaa
   ajurit, joilla tietokone näkee iPhonen.
2. Asenna **Sideloadly** osoitteesta <https://sideloadly.io> (Windows-versio).

(Macilla voit käyttää Sideloadlyn Mac-versiota tai AltStorea samalla tavalla. Ohjeet ovat
muuten samat.)

## 3. Laita puhelimessa Kehittäjätila päälle

1. Asetukset → **Tietosuoja ja turvallisuus** → **Kehittäjätila** → päälle.
2. Puhelin käynnistyy uudelleen. Vahvista kehittäjätila kysyttäessä ja anna lukituskoodi.

Jos Kehittäjätila-kohtaa ei näy, se ilmestyy vasta, kun puhelin on kytketty tietokoneeseen ja
Sideloadly on yrittänyt asennusta kerran. Yritä silloin vaiheen 4 asennusta ensin, avaa sitten
Kehittäjätila ja yritä uudelleen.

## 4. Asenna ohjelma puhelimeen

1. Avaa puhelimen lukitus ja kytke se USB-kaapelilla tietokoneeseen.
2. Valitse puhelimessa **Luota tähän tietokoneeseen** ja anna lukituskoodi.
3. Avaa Sideloadly. Ylhäällä pitäisi näkyä oma iPhonesi. Jos ei näy, avaa puhelimen lukitus,
   irrota ja kytke kaapeli uudelleen ja varmista, että Apple Devices -sovellus on asennettu.
4. Vedä **PP2Tracker.ipa** Sideloadlyn ikkunaan.
5. Kirjoita **Apple ID** -kenttään Apple ID:si sähköposti.
6. Paina **Start**. Anna Apple ID:n salasana kysyttäessä (se menee Applelle, ei minulle
   eikä kenellekään muulle). Jos käytössäsi on kaksivaiheinen tunnistus, kirjoita puhelimeen tuleva koodi.
7. Odota, että alareunassa lukee **Done**. Puhelimeen ilmestyy PP2 Tracker -kuvake.
   Sininen täppä kuvakkeen vieressä tarkoittaa vain, että sovellusta ei ole vielä avattu.

Jos Sideloadly antaa virheen **"Password protected" / "Pairing failed"**, puhelimen
lukitus on päällä: avaa lukitus ja yritä uudelleen.

## 5. Luota kehittäjään puhelimessa

Ennen ensimmäistä avausta:

1. Asetukset → Yleiset → **VPN ja laitehallinta**.
2. Valitse kohdassa *Kehittäjäsovellus* oma Apple ID:si ja paina **Luota**.

Nyt ohjelman voi avata.

## 6. Käyttö pelin aikana

1. Avaa **PP2 Tracker**. Paina **Salli ilmoitukset** ja hyväksy, jos sovellus pyytää.
2. Käynnistä näytön tallennus: paina sovelluksessa tallennusnappia, valitse listasta
   **PP2 Tracker** ja paina **Aloita lähetys**. Odota kolmen sekunnin lasku.
   Tallennus näkyy puhelimen yläreunassa punaisena merkkinä.
3. Avaa **Pro Pilkki 2** ja pelaa kisaa normaalisti. Peli on pidettävä vaakatasossa.
4. Ohjelma lukee kalaviestit ruudusta ja laskee kalat. Kisatyyppi tunnistetaan pelin ruudusta
   automaattisesti. Järvi tunnistetaan latausruudusta ja tulosnäytöstä, mutta järven
   tunnistus on lisätieto eikä vaikuta laskentaan.
5. **Katso tulokset** kahdella tavalla:
   - Avaa PP2 Tracker ja paina **Näytä tulokset**. Samalla sivulla voit valita kisatyypin ja
     järven käsin, jos automaattinen tunnistus on väärin. Käsin valittu voittaa automatiikan.
   - Paina sivulla **Pieni ikkuna**. Pelin päälle tulee pieni kelluva ikkuna, jossa näkyvät pisteet,
     kappaleet ja paino sekä viimeisin kala. Ikkunan voi vetää puhelimen reunaan piiloon ja
     takaisin näkyviin. iOS päättää ikkunan koon, ja sen voi nipistää suuremmaksi tai pienemmäksi.
6. Uusi kisa nollaa laskurin automaattisesti (latausruutu, kisatyypin vaihtuminen tai kellon
   hyppy). Voit nollata myös käsin sivulta.
7. Kun lopetat, paina yläreunan punaista merkkiä ja valitse **Lopeta**.

Vinkki: kisan tulokset säilyvät sivulla, vaikka tallennus katkeaisi.

## 7. Jos jokin ei toimi

- **Kalat jäävät laskematta tai laskuri on väärässä:** paina sivulta **Jaa loki** (tai **Kopioi
  loki**) ja lähetä loki minulle. Kerro myös, mitä pelissä oikeasti tapahtui (ja liitä pelin lista
  "Kaikki kalat painojärjestyksessä"). Näin virheen löytää nopeimmin.
- **Pieni ikkuna ei käynnisty:** paina nappia uudelleen. Ikkuna ei toimi, jos sivu ei ole auki
  tallennuksen aikana.
- **Sovellus ei avaudu enää (7 päivää kulunut):** asenna se uudelleen vaiheesta 4. Mitään ei menetä.
- **Tallennus katkeaa itsestään:** käynnistä tallennus uudelleen.
- **Sideloadly ei löydä puhelinta:** lukitus auki, kaapeli uudelleen, Apple Devices asennettuna.
  Kokeile eri USB-porttia ja datakaapelia (pelkkä latauskaapeli ei riitä).

## 8. Haluatko, ettei asennusta tarvitse tehdä joka viikko?

Ilmaisella Apple ID:llä sovellus on uusittava 7 päivän välein. Ilmaisia tapoja automatisoida se:

- **Sideloadlyn automaattinen uusinta:** tietokoneen on oltava päällä ja samassa wifi-verkossa
  kuin puhelin. Ota wifi-synkronointi päälle Apple Devices -sovelluksessa.
- **SideStore:** uusii sovellukset puhelimella ilman tietokonetta (vaatii ensiasennuksen
  tietokoneelta). Katso <https://docs.sidestore.io>.

Nämä ovat kolmansien osapuolien työkaluja, ja niiden toimivuus riippuu iOS-versiosta.

## Tietosuoja

Ohjelma lukee vain pelin ruudun puhelimen sisällä eikä lähetä mitään verkkoon. Tulossivu on
puhelimen sisäinen osoite (127.0.0.1). Apple ID:täsi käytetään vain asennuksessa (Sideloadly ja
Apple), ei tässä ohjelmassa.
