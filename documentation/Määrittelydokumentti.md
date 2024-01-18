# Määrittelydokumentti

### Kuvaus ja motivaatio
Yritetään vastata kysymykseen, "Kuinka monta viiden pituista joukkoa viiden pituisia sanoja, joissa on yhteensä 25 eri kirjainta on sanalistassa?". Aluksi ainakin näillä määritteillä ja englannin kielellä, mutta myöhemmin ohjelman pitäisi myös toimia eripituisilla joukoilla, sanoilla ja eri kielillä. 


Halusin ratkaista juuri tämän ongelman, sillä olin vähän aikaa sitten katsonut [tämän Matt Parkerin videon](https://youtu.be/_-AfhLQfb6w), jossa esiintyi sama kysymys, sekä [tämän jatko osan](https://youtu.be/c33AZBnRHks) jossa koodia nopeutettiin eri optimisaatioilla ja mielestäni koodin nopeutustavat olivat hyvin kiinnostavia ja halusin itse kokeilla niiden toteuttamista ja vertailua.

### Kielet
Käytän projektin tekemiseen suurimmaksi osaksi Python3:sta, mutta minulla on myös pieni määrä Java kokemusta, joten kykenen hädässä myös vertaisarvioimaan Java:lla tehtyjä projektejä.

### Algoritmit ja tietorakenteet
Tulen lähestymään kysymystä monella eri tavalla.
- Tiedän kuvastamani sanajoukkoja verkkoina.
- Kuvata sanoja jonoina bittejä.
- Käyttämäni [Knuth's Algorithm X](https://en.wikipedia.org/wiki/Knuth%27s_Algorithm_X)
- Muita itsetehtyjä algoritmejä eri optimisaatioilla, kuten karsinalla
- Erilaisia kombinaatioita näistä maksiminopeutta tavoitellessa.

### Ohjelman toiminta ja aikavaatimukset

Aluksi ohjelma saa syötteenä listan sanoja, testaukseen käytän [tätä listaa](https://github.com/dwyl/english-words), joka sisältää ~479 000 englanninkielistä sanaa. Tämän jälkeen ohjelman tulee rajata sanat n pituisiin sanoihin (n=5 alussa). 

Tämän jälkeen ohjelman pitää vain käsitellä kaikki sanajoukot ja palauttaa vastaus. On kuitenkin helposti huomattavissa, että 479 000 sanan käsittelyssä menee useita viikkoja, sillä jokainen kirjain pitää tarkastaa, ilman monia eri optimisaatioita ja algoritmejä, joihin projekti tulee suurimmaksi osaksi keskittymään.

Tämän toteuttaminen pienillä optimisaatioilla kuten anagrammien poistamisella, Matt Parkerilla menin koodin suoritukseen pythonilla noin 32 päivää, joten tämä on pohjataso. Tämän hetkinen nopein suoritus ongelmaan on 0.5 ms C kielellä, joka löytyy [täältä](https://github.com/stew675/standup5x5/).

En vielä ole varma omasta tavoitteesta, mutta uskon noin minuutin tai kahden olevan saatavissa.


### Lähteet
- Matt Parkerin videot https://www.youtube.com/watch?v=_-AfhLQfb6w ja https://www.youtube.com/watch?v=c33AZBnRHks
- Englanninkielen sanalista https://github.com/dwyl/english-words
- Ongelmaratkaisuennätykset https://docs.google.com/spreadsheets/d/11sUBkPSEhbGx2K8ah6WbGV62P8ii5l5vVeMpkzk17PI/edit#gid=0

 
Opinto-ohjelma: TKT

Dokumentaatiokieli: Suomi
