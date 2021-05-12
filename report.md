#Harjoitus 6

## a) Kokeile saltia windowsissa

Käytin windows minionin luomiseen apuna rikurikurikun [tehtäväraporttia](https://github.com/rikurikurikuriku/Palvelinten-hallinta/wiki/H5-Aikajana#b-windows-pakettivarasto-ja-vs)

Aloitin tehtävän tekemisen lataamalla salt minionin [salt stackin nettisivulta](https://repo.saltstack.com/#windows)
Installerissa laitetaan masterin IP-osoite ja nimi.

![kuva1](/images/kuva1.png) ![kuva2](/images/kuva2.png)

Kävin masterissa katsomassa, että onko sinne tullut yhtään hyväksymättömiä avaimia.

![kuva3](images/kuva3.png)

Hyväksyin juuri luodun windows avaimen. 

Päivitetään winrepo

![kuva4](images/kuva4.png)

Kokeilin asentaa rikurikurikun ohjeessa olevan vlc media playerin hänen käyttämällään komennolla sudo salt 'windows' pkg.install vlc

![kuva6](images/kuva6.png)

Asennus ja sovellus toimi moitteitta.

kokeilin vielä asentaa jotain uutta Joten päätin asentaa firefoxin windowsille. Löysin komennon firefoxin asennukselle rikurikurikun raportissa olevan [Linkin takaa.](https://docs.saltproject.io/en/latest/topics/windows/windows-package-manager.html)

  salt 'windows' pkg.install firefox_x64
  
![kuva7](images/kuva7.png)

![kuva5](images/kuva5.png)

## Lähteet

https://repo.saltstack.com/#windows

https://docs.saltproject.io/en/latest/topics/windows/windows-package-manager.html

https://github.com/rikurikurikuriku/Palvelinten-hallinta/wiki/H5-Aikajana#b-windows-pakettivarasto-ja-vs
