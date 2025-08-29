---
nav_order: 5
sort: 5
---

# Lähtötiedot

## Aineistojen ylläpito

HSL ylläpitää lähtötietoaineistoja MAL-suunnittelun ja joukkoliikennesuunnittelun tueksi.
Aineistojen nimissä on yleensä jokin vuosiskenaario, mutta ennusteet eivät koskaan kuvaa tarkkaa vuotta, vaan tiettyä hankkeiden,
maankäyttöjen ja muiden lähtötietojen yhdistelmää.

Tässä on kuvattu yleisesti HSL:n ylläpitämiä lähtötietoaineistoja ja niiden rakennetta.
Ohjeita aineistojen lataamiseen ja käyttöön löydät "[Mallijärjestelmän käyttö](mallitoiden_yleisohje.md)"-sivulta.

## Ennusteskenaarioiden syöttötiedot (maankäyttö, kustannukset ym)

**Lähtötietoja tuotetaan MAL-suunnittelun yhteydessä n. neljän vuoden välein seuraaville skenaarioille:**
* Nykytilan kuvaus
* MAL-suunnitelman tavoitevuoden skenaario
* MAL-suunnitelman pitkän aikavälin tavoiteskenaario
* Välivuosiskenaario

Aineistojen sisältöjä on kuvattu tarkemmin aineiston jakokansiossa, johon saat käyttöoikeuden täyttämällä hakemuslomakkeen EXT-helmet-Teams-ryhmässä.
Tiedostopolun juuren on dokumentit sisältävät aineistojen yleiskuvauksen,
ja tarkempia tietoja löytyy kunkin tiedoston sisältä kommmentteina.

Kysyntämalleja on kuvattu tarkemmin raportissa [Helsingin seudun työssäkäyntialueen liikenne-ennustejärjestelmän kysyntämallit 2020](https://staticfiles.hsl.fi/globalassets/julkaisuarkisto/2020/6_2020_helsingin_seudun_tyossakayntialueen_liikenne-ennustejarjestelman_kysyntamallit.pdf).

## Verkkokuvaukset

Vuosittain päivitetään tuore nykytilan kuvaus sekä mahdolliset muutokset tulevien vuosien kuvauksiin HSL:n ja kuntien tuottamiin suunnitelmiin perustuen.
Muutostyö käynnistyy tammikuussa Liikennöintisuunnitelman hyväksymisen jälkeen, ja viimeistellään kesällä, kun kaikki syksyn muutokset ovat varmistuneet.
Päivitetyt versiot julkaistaan syksyisin. Verkkojen vuosipäivityksiä laaditaan vuosittain kuvaamaan kunkin syksyn liikennetilannetta HSL-liikenteessä. 
Tässä yhteydessä samat muutokset kuvataan myös MAL-verkkojen päivitettäviin versioihin sekä välivuosien verkoille.
Lisäksi tulevaisuuden verkkoihin viedään tiedot esim. valmistuneiden linjastosuunnitelmien tuomista muutoksista. 

Kaukojunaliikennettä ja muiden kuin HSL-alueen bussilinjoja ei päivitetä säännöllisesti vuosipäivitysten yhteydessä.
Kaukojunaliikennettä päivitetään suurempien muutosten yhteydessä, ja viimeisin muutos on syksyltä 2023.
Muiden kuin HSL:n järjestämän linja-autoliikenteen viimeisin päivitys on vuodelta 2023.

Laajempia muutoksia tehdään MAL-suunnittelun yhteydessä n. neljän vuoden välein, ja tässä pohjana käytetään viimeisimmän vuosipäivityksen mukaisia verkkoja.

**Lähtötietoja tuotetaan seuraaville skenaarioille:**
* Nykytilan kuvaus
* MAL-suunnitelman tavoitevuoden skenaario
* MAL-suunnitelman pitkän aikavälin tavoiteskenaario
* Välivuosiskenaario

Aineistojen sisältöjä on kuvattu tarkemmin aineiston jakokansiossa, johon saat käyttöoikeuden täyttämällä hakemuslomakkeen EXT-helmet-Teams-ryhmässä.
Kullekin vuodelle on oma alikansionsa ja niistä löytyy readme-tiedostot, joissa on selostettu yleiskuvaus aineistosta.

Ilmoitathan, mikäli havaitset tarjontakuvauksissa puutteita tai korjaustarpeita.
HSL ylläpitää korjaustarvelistaa sekä tarjontamallin lähtötietojen tarkempia kuvauksia.

Verkkokuvausperiaatteita on kuvattu tarkemmin raportissa Helsingin seudun liikenteen Emme-verkon kuvaus,
joka on saatavilla mallin käyttäjien EXT-Helmet -Teams-ryhmässä.
Noudatathan näitä periaatteita verkonkuvauksia koodatessa, jotta varmistutaan tulosten oikeellisuudesta ja aineistojen yhteiskäyttöisyydestä. 

Lisätietoja mallin käyttämisestä "[Mallijärjestelmän käyttö](mallitoiden_yleisohje.md)"-sivulla.
Taustatietoa verkkokuvausten muodostamisesta ja historiasta löydät raportista [Helsingin seudun työssäkäyntialueen liikenne-ennustejärjestelmän tarjontamallit 2017](https://staticfiles.hsl.fi/globalassets/julkaisuarkisto/2019/helsingin-seudun-tyossakayntialueen-liikenne-ennustejarjestelman-tarjontamallit-6-2019.pdf).



## Ennusteskenaarioiden syöttötiedot

Kansio sisältää kullekin tarkasteluvuodelle/skenaariolle alikansion, jossa on lähtötiedot mm. maankäytön ja kustannusten osalta.
Kunkin tiedoston alussa on kuvattu mitä tiedosto sisältää ja mistä tiedot tulevat.
Kansiossa on oltava yksi kappale kustakin tiedostotyypista .cco, .edu, .ext, .lnd, .pop, .prk, .tco, .trk sekä .wrk.
Tiedostojen nimillä ei ole merkitystä, ja ne voivat poiketa toisistaan (kansiossa voi esim. olla 2023.pop ja 2023_b.wrk)

**Tiedostot**

* **car** = *valinnainen tiedosto*, johon voi syöttää aluekohtaiset pysäköintinormit (autoa/asukas) sarakkeeseen `prknorm`, esimerkiksi tällä tavalla:

|     | prknorm |
|-----|---------|
| 191 |     0.7 |
| 192 |     0.6 |
| 301 |     1.0 |

Pysäköintinormit vaikuttavat vain uusien asukkaiden autonomistukseen.

* **cco** = autoilun kilometrikustannus
* **edu** = kunkin ennustealueen oppilaspaikkamäärät peruskoulussa, toisella asteella ja korkeakouluissa
* **ext** = ulkoinen liikenne eli työsäkäyntialueen tienpäät (kasvukerroin verrattuna nykytilaan)
* **lnd** = kunkin ennustealueen rakennetun maa-alan osuus sekä erillistalojen osuus rakennuskannasta
* **pop** = kunkin ennustealueen kokonaisväkiluku sekä eri ikäryhmien osuudet
* **pnr** = liityntäpysäköintilaitosten kapasiteetti ja 12 tunnin hinta
* **prk** = kunkin ennustealueen työpaikan ja asiointimatkojen pysäköintikustannukset
* **tco** = joukkoliikenteen kuukausikustannukset eri vyöhykkeillä
* **trk** = raskaan liikenteen lähtötiedot: yhdistelmäajoneuvoilta kielletyt ennustealueet ja jätteenkäsittelylaitosten ennustealueet
* **wrk** = kunkin ennustealueen kokonaistyöpaikkamäärä sekä eri alojen työpaikkojen osuudet (palvelut, kaupat, logistiikka, teollisuus)

### Lähtödata

Kansio sisältää perusvuoden (lähtökohtaisesti 2023, mutta jotkut tiedot voivat olla vanhempia) syöttötietoja (kuvattu yllä)
ja [kysyntämatriiseja](tulokset.md#tuloskansion-matriisitiedostojen-kuvaukset).
Kysyntämatriisit menevät ensimmäiseen sijoitteluun, josta kysyntälaskenta alkaa.
Perusvuoden syöttötiedot menevät tavaraliikennemalliin ja autonomistusmalliin, jotka molemmat ovat muutosmalleja.
Perusvuoden syöttötiedoissa `car`-tiedosto on (toisin kuin ennusteskenaarion syöttötiedoissa) pakollinen:

* **car** = kunkin ennustealueen autotiheys

### Verkot

Kansio sisältää kullekin tarkasteluvuodelle/skenaariolle alikansion, jossa on liikenneverkon lähtötiedot sekä niiden selostus (readme).

**Tiedostot**

* **base_network_xxx.txt** = liikenneverkon solmut ja linkit sekä niiden attribuutit
* **transit_lines_xxx.txt** = joukkoliikennelinjaston kuvaus: mm. linjatunnus, kulkumuoto, ajoneuvotyyppi (vehicle), reitin otsikko, reitin käyttämät solmut
* **turns_xxx.txt** = kääntymiskiellot eri solmujen välillä
* **extra_links_xxx.txt** = linkkikohtainen tienkäyttömaksu eri aikajaksoilla (aht, pt, iht), pyörätieluokka eri linkeillä, linkin kaltevuus
* **extra_nodes_xxx.txt** = solmun korkeustaso
* **extra_transit_lines_xxx.txt** = joukkoliikennelinjojen vuorovälit eri aikajaksoilla (aht, pt, iht)

Skenaariot voi muodostaa kootusti Modellerissa "[Sijoittelupankin perustaminen](sijopankki.md)"-sivun ohjeiden mukaan.
Moduuli ajaa myös sisään seuraavat kaikille skenaarioille yhteiset tiedot:

* **modes_xxx.txt** auto- ja pyöräverkon kulkutavat
* **vehicles_xxx.txt** joukkoliikenteen ajoneuvotyypit

## Lähtötietojen muokkaaminen

Lähtötietoja voi muokata joko suoraan lähtötietotiedostoihin tai Emme-ohjelmiston (Modeller, Network Editor, Prompt) kautta.

Verkkokuvausperiaatteita on kuvattu tarkemmin "[EMME-verkon kuvaus](emme_verkko.md)" -sivulla.
Noudatathan näitä periaatteita verkonkuvauksia koodatessa, jotta varmistutaan tulosten oikeellisuudesta ja aineistojen yhteiskäyttöisyydestä.

## Lähtötietojen vaikutus ennustemallin eri osiin

* Autonomistus alueittain
  * Kerros- ja pientalojen osuudet
  * Matka-aikasuhteet
* Matkamäärä alueittain
  * Asukasmäärä ikäryhmittäin
  * Autonomistus
* Kulkutavan valinta
  * Alueparien väliset matka-ajat autolla ja joukkoliikenteellä
  * Alueparien väliset etäisyydet polkupyörällä ja autolla
  * Alueparien väliset matkakustannukset: joukkoliikennelipun hinta, autoiun muuttuvat kustannukset (polttoaine, renkaat) ja mahdollinen ruuhkamaksu/tietulli
  * Autonomistus alueittain
* Matkakohteiden valinta
  * Saavutettavuus (matka-aika, etäisyys ja matkakustannus määräpaikkaan eri kulkutavoilla)
  * Työpaikkamäärä määräpaikassa
  * Oppilaspaikkojen määrä määräpaikassa
* Reitin valinta
  * Auto- ja joukkoliikennelinkin matka-aika
  * Pyörälinkin pituus
  * Autolinkin matkakustannus
