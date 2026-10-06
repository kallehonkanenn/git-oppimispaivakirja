# Oppimispäiväkirja: Hajautettu git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet, jotka vaikuttivat tehtävän suorittamiseen?__

Osion tehtävät olivat melko helppoja, kun ohjeita noudatti kohta kohdalta. Vaikeinta oli ymmärtää, miten paikallinen repositorio ja GitHub-repositorio eroavat toisistaan ja miksi muutokset täytyy erikseen viedä ja hakea. Ymmärsin tämän parhaiten, kun tein muutoksen GitHubin web-käyttöliittymässä ja katsoin, miten git status muuttui ennen git fetch -komentoa ja sen jälkeen.

## Osiossa käyttämäni Git-komennot

| Komento | Kuvaus |
| --------| ------ |
| git remote add origin https://github.com/kallehonkanenn/hello.git | Lisää GitHub-repositorion etärepositorioksi nimellä origin |
| git remote -v | Näyttää etärepositoriot ja niiden osoitteet |
| git push -u origin master | Vie master-haaran GitHubiin ja muistaa sen jatkossa |
| git switch -c new-feat | Luo uuden haaran ja siirtyy siihen |
| git add feat.txt | Lisää tiedoston seuraavaan talletukseen |
| git commit -m "Lisätty feat.txt" | Tallettaa muutokset versiohistoriaan |
| git status | Näyttää repositorion tilan |
| git branch | Listaa paikalliset haarat |
| git push -u origin new-feat | Vie uuden haaran GitHubiin |
| git fetch | Hakee muutokset GitHubista yhdistämättä niitä |
| git switch origin/new-feat | Siirtyy katsomaan etähaaran tilaa |
| git switch new-feat | Vaihtaa takaisin paikalliseen new-feat-haaraan |
| git merge origin/new-feat | Yhdistää etähaaran muutokset paikalliseen haaraan |
| git switch master | Vaihtaa master-haaraan |
| git merge new-feat | Yhdistää new-feat-haaran master-haaraan |
| git push | Vie nykyisen haaran talletukset GitHubiin |
| git tag harjoitus5 | Lisää viimeisimpään talletukseen tunnisteen |