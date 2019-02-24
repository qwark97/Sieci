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


![763542de-69d5-4aae-a51a-c07c955552b5 png](https://user-images.githubusercontent.com/37438072/53300117-16eb6280-3843-11e9-9313-0d9f470a72e3.jpg)




| Komenda | Znaczenie  
| ------------- |:-------------:| 
| ifup <nazwa>  |  Do wlaczenia karty | 
| nmcli device show | Nazwa karty |

