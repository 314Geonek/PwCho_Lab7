Projekt polegal na stworzeniu usugi LAMP skadajacej sie z serwerow:

PHP posiadajacego przylaczone sieci backend.

APACHE posiadajacego przylaczone sieci backend i frontend oraz wystawiony port 6666. 

MySQL posiadajacego przylaczone sieci backend. 

projekt nalezy najpierw zbuildowac poleceniem:
```
docker-compose build
```
nastepnie uruchomic poleceniem: 
```
docker-compose up
```
w momencie uruchomienia systemu na adresie localhost:6666 jestesmy w stanie zaobserwowac dzialanie skryptu index.php zlokalizowanego w folderze files. Przegladarki przy polaczeniu z tym portem blokuja polaczenie co zmusza uzytkownika do sprawdzenia poprawnosci dzialania systemu poprzez  polecenie:
```
curl localhost:6666/ 
```
po wykonaniu polecenia wyswietla nam sie wynik dialania skryptu zawartego w index.php

polecenie:
```
curl localhot:6666/index.html
 ```
wywietli nam zawartosc  pliku index.html zawartego w folderze files
