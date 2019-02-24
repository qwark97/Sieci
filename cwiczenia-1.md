System operacyjny w środowisku sieciowym
=========================================

Charakterystyka systemu operacyjnego
------------------------------------

| Charakterystyka | wartość           | komentarzu |
| ------------- |:-------------:| -----:|
| nazwa      | linux | centos 7 |
| program (parametry sieci)      | nie wiem |  |


Konfiguracja połączenia sieciowego
----------------------------------

| Parametr | wartość           | komentarzu |
| ------------- |:-------------:| -----:|
| Adres IP      | 10.0.2.15 | przydzielony przez DHCP |
| Maska podsieci      | 24 |  |
| Brama      | 10.0.2.2 |  |
| DNS 1      | 10.10.0.8 |  |
| DNS 2      | 10.10.0.4 |  |

Schemat sieci
-------------

aby załączyć obrazek 

![39607](https://user-images.githubusercontent.com/37438072/53299752-1cdf4480-383f-11e9-8ab4-f59d61ecec51.jpg)



| Komenda | Znaczenie  
| ------------- |:-------------:| 
| ifup <nazwa>  |  Do wlaczenia karty | 
| nmcli device show | Nazwa karty |

