# Oppimispäiväkirja: Git projektissa

__Mitä hyötyä voisi olla versionhallinnasta, jos kehität projektia yksin?__

Versionhallinnan avulla voin palata aiempaan toimivaan versioon, jos jokin muutos rikkoo ohjelman. Historiasta näkee, mitä on muutettu ja milloin, ja talletusviestit toimivat samalla muistiinpanoina. Ominaisuushaaroissa voi kokeilla uusia asioita turvallisesti ilman, että toimiva versio vaarantuu. Lisäksi GitHub toimii varmuuskopiona, ja koodin saa helposti käyttöön myös toiselle koneelle.

__Mitä hyötyä voisi olla versionhallinnasta, jos projektissa on useita kehittäjiä?__

Useat kehittäjät voivat työskennellä samaan aikaan omissa haaroissaan ilman, että he ylikirjoittavat toistensa töitä. Muutokset yhdistetään hallitusti, ja konfliktit huomataan ennen kuin ne päätyvät päähaaraan. Historiasta näkee, kuka on tehnyt minkäkin muutoksen ja miksi. Yhdistämispyynnöillä (pull request) muut voivat tarkastaa koodin ennen yhdistämistä, mikä parantaa laatua.

__Miten järjestäisit projektitiimin versionhallinnan 3-4 hengen ohjelmistoprojektikurssilla? Laadi tiimiläisille lyhyt ohje, miten projektissa toimitaan.__

Tiimin ohje:

1. Projektilla on yksi yhteinen GitHub-repositorio, ja kaikki kloonaavat sen omalle koneelleen.
2. `master`-haarassa on aina toimiva, testattu versio. Siihen ei talleteta suoraan.
3. `develop`-haarassa kootaan valmiit ominaisuudet yhteen.
4. Jokainen tekee oman työnsä ominaisuushaarassa (esim. `feature/kirjautuminen`), joka luodaan `develop`-haarasta.
5. Talletukset ovat pieniä, ja viesti kertoo selkeästi, mitä muutettiin.
6. Kun ominaisuus on valmis, siitä tehdään pull request haaraan `develop`. Vähintään yksi toinen tiimiläinen tarkastaa sen ennen hyväksymistä.
7. Ennen töiden aloittamista ja ennen pushia haetaan muiden muutokset komennolla `git pull`.
8. Hyväksytyn pull requestin jälkeen ominaisuushaara poistetaan.
9. Sprintin lopussa testattu `develop` yhdistetään haaraan `master`, ja versiolle lisätään tunniste (tag).

__Kommenttini opintojaksosta, esim. sisällöstä, materiaalista, työmäärästä, hyödyllisyydestä, työmäärästä. Mitä toivoisit olevan enemmän, mitä vähemmän?__

Opintojakso oli hyödyllinen, ja Gitin perusasiat tulivat tutuiksi harjoitusten kautta. Harjoitukset etenivät sopivassa järjestyksessä, ja oppimispäiväkirja auttoi kertaamaan komentoja. Työmäärä oli kohtuullinen. Harjoitus 6 oli selvästi vaikein, ja siihen olisin kaivannut tarkempia ohjeita, esimerkiksi tiimikaverin muutosten hakemisesta. Toivoisin enemmän harjoituksia merge-konflikteista ja niiden ratkaisemisesta, koska ne ovat käytännön työssä yleisiä.