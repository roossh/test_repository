## R: Osa 1

<p>Huom! Käy lukemassa ensin osa 0, joka sisältää ohjeita RStudion käyttöön. Tässä osassa oletetaan, että tiedät, miten valitsemaasi alustaa käytetään ja keskitytäänkin enemmän jo itse R-ohjelmiston perusteisiin.</p>
<p>Sivulla on paljon asiaa, joten CTRL+F (Windows/Linux) tai CMD+F (Mac) voi osoittautua varsin hyödylliseksi.</p>

### Tavoitteet

* R-ohjelmiston käyttö laskimena
* Yleistä syntaksista
* Datatyypit
  * Numeeriset arvot
  * Merkkijonot
  * Loogiset arvot
  * NA
* Muuttujat
  * Muuttujan käsite
  * Muuttujan luominen
  * Muuttujan kutsuminen
  * Muuttujan arvon muuttaminen
  * Muuttujan poistaminen
* Vektorit
  * Vektorin luominen
  * Arvojen haku vektorista
  * Vektorin arvon muuttaminen
  * Laskutoimitukset vektoreilla
* Ehtolauseet
  * Ehtolauseen rakentaminen
  * Ehtolauseiden yhdistäminen
  * Arvojen hakeminen vektorista ehtolauseella
  
## R-ohjelmisto laskimena

<p>Kuten monia muitakin skriptauskieliä, R:ää voi yksinkertaisimmillaan käyttää <b>laskimena</b>. Tämä käytännössä tarkoittaa sitä, että voit ajaa joko konsolissa tai skriptistäsi suoraan laskutoimituksia.</p>

```R
> 1+1
[1] 2
```
> _Huomaa, että sinun **ei tarvitse** kirjoittaa > -merkkiä, vaan tämä on aina R-konsolissa kuvaamassa uutta riviä!_

#### Operaattorit

 <p><i>Operaattoreilla</i> tarkoitetaan merkkejä, jotka suorittavat jotain erityistä tehtävää. Yleisimmät käytetyt operaattorit merkkeineen on esitetty alla.</p>

Operaattori | Merkitys | Esimerkki
------------ | ------------- | -------------
 <code>+</code> | Summa | 2+3
 <code>-</code> | Erotus | 3-4
 <code>*</code> | Tulo | 4*5
 <code>/</code> | Osamäärä | 16/4
 <code>**</code> tai <code>^</code> | Potenssi | 10**2
 
 <p>Laskutoimitukset tapahtuvat käytännössä niin, että kirjoitat joko tekstieditoriin (suositeltavaa) tai konsoliin laskutoimituksen, jonka haluat laskea ja ajat rivin.</p>
 
 <p>Useita laskutoimituksia on mahdollista yhdistellä, mutta tällöin ole tarkkana sulkujen kanssa!</p>
 
 ```R
> (1+2)/3
[1] 1
> 1+2/3
[1] 1.666667
```

<p>Huomaa myös, että desimaalit merkitään pisteellä eikä suomalaisittain pilkulla.</p>

#### Syntaksi

<p><i>Syntaksi</i> kuvaa tapaa kirjoittaa koodia. Kuten oikeissa kielissä, myös ohjelmointikielissä tulee noudattaa sääntöjä. Koska R on matalantason kieli, niin tämän syntaksi on hieman joustavampaa kuin eräiden korkean tason kielten kanssa (Java, JavaScript, C++...). Tämä tarkoittaa käytännössä sitä, että R:n perusteet on nopeammin opittavissa, mutta myös sitä, että tietyissä asioissa R on hitaampaa (tosin sitä on nopeampi kirjoittaa) ja R rajoittuu aika pitkälti tilastoanalyysiin ja datavisualisointiin siinä missä kielillä kuten Java voidaan rakentaa hyvinkin kattavia ohjelmistoja. Biologille kuitenkin juuri R on erittäin hyödyllinen työkalu ja esimerkiksi Javaa harvemmin käytetään biologipiireissä.</p>

<p>R-ohjelmisto toimii niin, että luettaessa skriptiä se lukee sitä ylhäältä alas: tämän vuoksi on enemmän kuin suositeltavaa, että kirjoitat koodia aina tekstieditoriisi niin, että luot muuttujat aina ennen kuin niitä käytetään ja pidät koodirivit loogisessa järjestyksessä.</p>
