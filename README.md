**Eksperymentalny obraz hotspot FM Orange PI Zero v3**

**To jest projekt hobbystyczny i rozwija się w autora własnym tempie.**

Obraz przeznaczony do budowy hotspota domowego

Obraz o nazwie fmpoland-ozpi3.img.xz nagrać na kartę microSD (8 Gb lub większa) przy pomocy: https://etcher.balena.io/

Login do konsoli via ssh:

user: root

hasło: fmpoland

Zalecana zmiana hasła poleceniem: passwd

Dostęp do dashboard:

http://hotspot-fmpl.local/

lub

http://ip_adres

IP adres możesz znaleźć przy pomocy darmowego narzędzia: https://www.advanced-ip-scanner.com/pl/

Konfiguracja via Dashboard, należy wybrać z menu "Admin" i następnie:

W pierwszej kolejności sprawdź poprawne ustawienia obsługi SQL i PTT w menu

**SQL PTT"

Po sprawdzeniu / ustawieniu SQL / PTT dopiero wtedy możesz przejść do konfiguracji:

"SVXCnf" - konfiguracja konta 

"NodeInfo" - Informacje o stacji

"WEBCnf" - konfiguracja Dashboard

oraz inne opcje stosownie do potrzeb

CZYTAJ uważnie informacje umieszczone w każdym oknie z serii administracyjnych
w których są istotne informacje do dostępnych ustawień

![Admin Menu](https://github.com/radioprj/orangepiv3/blob/main/admin-menu.png)

Domyślnie obraz przygotowany do pracy z modyfikowana kartą dźwiękowa CM108: http://fm-poland.pl/budowa-hotspota/

Można wykorzystać obraz z dowolnym radiem np GMxx, BF-888, UVK5, UV5R itp podłączając go do: http://fm-poland.pl/files/ozpi3-anyradio.pdf lub 
http://fm-poland.pl/files/ozpi3-sa818.pdf (obecnie niesprawdzone działanie GPIO na OZPI3 wymaga testów, używać zalecane numery GPIO SQL: 69, PTT: 70)

Jeśli dashboard będzie dostępny z zewnątrz (zastanów sie czy jest to ci niezbędne) to aby dostać się do menu ADMIN należy w Admin -> WebCnf w opcji REMOTEIP zamiast adresu 127.0.0.1 wpisać zdalny zaufany IP adres (ZALECANE: można skorzystać z VPN Tailscale wersja personal zawiera darmową obsługę 3 userów/100 urządzeń). Można też dostać z publicznego adresu do strony dashboard po linkiem

http://ipadresdashboard/svxc/

po podaniu użytkownika i hasła gdzie można wyłączyć lub włączyć zdalnie odbiornik SVXLINK. Jak założyć użytkownika i dla niego hasło patrz opis na swoim hotspot w pliku /etc/svxlink/SVXControl.txt

![Hotspot login](https://github.com/radioprj/orangepiv3/blob/main/hotspot-login.png)



**Eksperymentalny obraz używasz na własną odpowiedzialność i autor nie ponosi odpowiedzialności za wykorzystane rozwiązanie i wynikające z niego skutki.**


