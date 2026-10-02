# Oppimispäiväkirja: Paikallinen git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?__

Tehtävä oli mielestäni helppo, sillä olen käyttänyt näitä komentoja jo muillakin kursseilla

## Osiossa käyttämäni Git-komennot

| Komento | Kuvaus |
| --------| ------ |
| git clone https://github.com/mruonavaara/git-oppimispaivakirja | git clone lataa GitHubissa olevan repositoryn omalle tietokoneelle. Se luo samalla uuden kansion, johon repositorion tiedostot tallennetaan |
| cd git-oppimispaivakirja| cd-komennolla siirrytään terminaalissa toiseen kansioon|
| git switch paivakirja1 | git switch-komennola vaihdetaan Git haaraa |
| git init | Alustaa kansioon uuden Git-repositorion |
| git status | Näyttää repositorion tilan ja muuttuneet tiedostot |
| git add test.txt | Lisää tiedoston muutokset seuraavaan talletukseen |
| git add . | Lisää kaikki muutokset kerralla seuraavaan talletukseen |
| git commit -m "test.txt luotu" | Tallettaa muutokset versiohistoriaan viestin kanssa |
| git mv hello.html index.html | Nimeää tiedoston uudelleen |
| git rm test.txt | Poistaa tiedoston ja merkitsee poiston talletettavaksi |
| git log | Näyttää talletushistorian |
| git log --stat | Näyttää historian ja talletuksissa muuttuneet tiedostot |
| git log --oneline | Näyttää historian tiiviisti, yksi talletus per rivi |
| git log --oneline -3 | Näyttää vain kolme viimeisintä talletusta |
| git log --oneline --graph --all | Näyttää kaikkien haarojen historian graafina |
| git tag harjoitus2 | Lisää viimeisimpään talletukseen tunnisteen |
| git tag | Listaa kaikki tunnisteet |
| git restore --staged muutos.txt | Peruu tiedoston git add -komennon |
| git restore --staged . | Peruu kaikkien tiedostojen git add -komennon |
| git restore index.html | Palauttaa tiedoston viimeksi talletettuun tilaan |
| rm muutos.txt | PowerShellin komento, joka poistaa tiedoston |
| git revert 0778b7ecbecf1ba5ae765e1888aebef63261a4be | Kumoaa talletuksen tekemällä uuden talletuksen |
| git branch | Listaa haarat ja näyttää aktiivisen haaran |
| git switch -c tyylit | Luo uuden haaran ja siirtyy siihen |
| git switch master | Vaihtaa takaisin master-haaraan |
| git merge --no-ff tyylit | Yhdistää haaran nykyiseen haaraan ja luo oman merge-talletuksen |