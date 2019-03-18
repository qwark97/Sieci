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

Ustawianie parametrów sieci ip
------------------------------

* stan interfejsu
    * interfejs up
    * interfejs down
* adresacja
    * dodaj adres
    * zmień adres
    * usuń adres
* routing
    * dodaj trasę default
    * dodaj trasę przez bramę
    * dodaj trasę przez interfejs
    * usuń trasę
    * zmień trasę
    * pobierz trasę dla adresu
* adresacja fizyczna
    * pokaż adresy interfejsów dostępnych w sieci
    * pokaż adresy dla konkretnego interfejsu
     

podstawowe komendy 
-------------------------
|  polecenie   | opis  |
| -------------| :-----|
| ifup <nazwa>  |  Do wlaczenia karty | 
| ifup <nazwa>  |  Do wylaczenia karty | 
| nmcli device show | Nazwa karty |


ip 
-------------------------
| subcommand    |  polecenie   | opis  |
| ------------- |:-------------| :---------------| 
|   ``addr``    |                               | infirmacje o adresacji i własnościach interfejsów |
|               |   ``ip addr``                 | informacja o wszystkich interfejsach              |
|               |   ``ip addr show dev enp0s3`` | informacja o konkretnym interfejsie               |
|   ``link``    |   ``ip link set enp0s3 down`` | wyłącza interfejs enp0s3                          |
|               |   ``ip link set enp0s3 up``   | włącza interfejs enp0s3                           |
|   ``route``   |   ``ip route show ``          | pokazuje wszystkie routy                          |
|               |   ``ip route add``            | dodaje do tablicy routing np: ``ip route add default via 10.0.10.1 dev enp0s3``|
|   ``maddr``   |   ``ip route get``            | sprawdzenie gdzie konkretny adres zostanie wysłany np: ``ip route get 8.8.8.8`` |
|   ``neigh``   |  | |
|   ``help``    |  | |

Zadanie
------------

![zadanie 3](cwiczenia3.svg)

1.1 Przygotuj konfigurację sieci zgodnie z powyższym diagramem,\n 
1.2 Przetestuj połączenie poleceniem ping\n
2.1 Zainstaluj na komputerze ``PC1`` serwer programu ``HTTP CHAT`` dostępnego pod adresem ``https://github.com/jkanclerz/http-chat``
2.2 Przetestuj komunikację wysyłając wiadomość z komputera ``PC2``, upewnij się czy jest widoczna w konsoli serwera
3.1 Dodaj do istniejącej sieci komputer ``PC3`` pod kontroloą systemu windows
3.2 Skonfiguruj ``PC3`` zgodnie z poniższym diagramem
3.3 Zweryfkuj połączenie kożystając z przeglądarki, odwiedzając graficzny interfejs ``HTTP CHAT`` pod adresem ``http://172.16.100.10:8888``
3.4 Przygotuj dokumentację pisemno obrazkową z wykonania zadania w formacie ``markdown`` zamieść ją w serwisie ``github.com`` obok obocnego tematu ``cwiczenia-3``

![zadanie 3.1](cwiczenia3.1.svg) 
