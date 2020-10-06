# host_2

B. Aplikacja kliencka:
- Uruchamiana jest z dwoma parametrami: nazwa_uzytkownika i sciezka do lokalnego folderu
- Klient po uruchomieniu rejestruje sie na serwerze (podajac swoja nazwe_uzytkownika)
- Kazdy klient ma swoj lokalny folder z plikami
- Aplikacja obserwuje lokalny folder i reaguje na zmiany. Jak pojawia sie tam nowe pliki, to wysyla je na serwer
- Jak pojawi sie nowy plik dla danego uzytkownika, to jest on pobierany do lokalnego folderu
- Aplikacja po uruchomieniu odpytuje serwer o nowe pliki i je sciaga
- Aplikacja kliencka ma interfejs graficzny (np. Java FX) pokazujacy w czasie rzeczywistym czym sie w danej chwili zajmuje klient ("Pobieram...", "Wysylam ...", "Sprawdzam ....") oraz wyswietlajacy liste aktualnych plikow w lokalnym folderze. Panel graficzny ma umozliwic takze udostepnienie danego pliku innemu uzytkownikowi. Liste dostepnych uzytkownikow nalezy pobrac z serwera (lista ta ma sie dynamicznie odswiezac wraz z nowymi uzytkownikami/po wyrejestrowaniu uzytkownikow na serwerze.
- klient po zamknieciu informuje serwer ze sie zamyka i serwer usuwa go z listy uzytkownikow dostepnych.
