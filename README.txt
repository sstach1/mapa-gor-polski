MAPA GÓR POLSKICH – v16
=======================

STRUKTURA
---------
index.html  – wygląd i mechanizm mapy
dane.js     – baza pasm, kategorii i miejsc
zdjecia/    – katalog na własne zdjęcia

URUCHAMIANIE
------------
1. Rozpakuj cały folder w jednym miejscu.
2. Otwórz index.html w przeglądarce.
3. Do publicznego udostępnienia wgraj CAŁY folder na hosting
   (np. GitHub Pages, Netlify albo własny hosting).

DODAWANIE WŁASNEGO ZDJĘCIA
--------------------------
Przykład:
1. Skopiuj zdjęcie do:
   zdjecia/karkonosze/sniezka.jpg

2. W pliku dane.js przy danym miejscu zmień:
   photo: "https://commons.wikimedia.org/..."
na:
   photo: "zdjecia/karkonosze/sniezka.jpg"

3. Przy zdjęciu własnym możesz usunąć pola:
   photoPage
   photoCredit
   photoLicense
lub wpisać np.:
   photoCredit: "zdjęcie własne"

WAŻNE
-----
Nie zmieniaj nazw plików index.html i dane.js bez równoczesnej zmiany odwołań.
W przyszłości możemy dodać prosty formularz/panel do edycji miejsc bez ręcznej pracy w kodzie.

PANEL EDYCJI – WERSJA v17 POPRAWIONA
------------------------------------
Panel jest ładowany dopiero po uruchomieniu mapy i nie blokuje wyświetlania
dotychczasowej bazy danych.

Jeżeli edytujesz dane:
1. kliknij „Zapisz lokalnie”,
2. po zakończeniu kliknij „Eksportuj dane.js”,
3. zastąp nim dotychczasowy plik dane.js.


POPUPY – v18
------------
Okno opisu miejsca można przeciągać myszką lub palcem.
Dodatkowo ma ono ograniczoną wysokość i własne przewijanie, aby nie wychodziło
poza ekran na mniejszych monitorach i telefonach.

GÓRY IZERSKIE – v19
-------------------
Uzupełniono wszystkie 8 kategorii: szczyty, wodospady, punkty widokowe,
atrakcje, formacje skalne, schroniska, zabytki i mniej znane miejsca.
Tam, gdzie źródła nie pozwalały rzetelnie potwierdzić parkingu/czasu dojścia,
pola pozostawiono puste zamiast wpisywać dane orientacyjne jako pewne.

v20 – ROZSZERZONY STANDARD
--------------------------
Ujednolicono dotychczas wypełnione pasma do rozszerzonego schematu kart.
Każde miejsce ma przygotowane pola: why, curiosity, tags, difficulty, family,
dog, fee, parking, parkingLat/Lon, walkTime, distance, gain oraz pola zdjęcia.
Pola praktyczne pozostają puste, jeśli nie zostały rzetelnie potwierdzone.
Dla najważniejszych miejsc uzupełniono zweryfikowane informacje praktyczne.

v21 – DOPRACOWANIE DOTYCHCZASOWEJ BAZY
--------------------------------------
Po ponownym przeliczeniu baza obejmuje 221 obiektów w dotychczas
opracowanych pasmach (wcześniejsze podsumowanie omyłkowo nie doliczyło Gór Złotych).

Każdy obiekt ma teraz spójny rozszerzony standard karty:
- nazwa, wysokość, GPS, opis
- Dlaczego warto?
- tagi
- trudność
- rodziny
- pies
- opłaty
- parking/start i jego GPS tam, gdzie został rzetelnie ustalony
- czas, dystans i przewyższenie tam, gdzie są jednoznaczne dla wskazanego wariantu
- ciekawostka, gdy jest zweryfikowana
- zdjęcie i dane licencyjne, jeśli posiadamy pewne zdjęcie Wikimedia Commons
- źródła regionalne / oficjalne
- wyraźna informacja, gdy parametry trasy zależą od wybranego wariantu

Nie wpisywano fikcyjnych współrzędnych parkingów ani pozornie dokładnych czasów
dla miejsc, które mają wiele równorzędnych wariantów dojścia.

v22 – PRZYCISK „WYBIERZ WŁASNE ZDJĘCIE”
---------------------------------------
W panelu edycji dodano przycisk „📷 Wybierz własne zdjęcie”.

Po wybraniu zdjęcia panel:
- pokazuje je od razu w podglądzie,
- automatycznie tworzy bezpieczną nazwę pliku (małe litery, bez polskich znaków),
- automatycznie wpisuje ścieżkę np. zdjecia/karkonosze/sniezka.jpg,
- pokazuje, do którego folderu projektu trzeba skopiować plik.

WAŻNE:
Plik dane.js NIE zmienia się sam na dysku. „Zapisz lokalnie” zapisuje zmiany
w pamięci przeglądarki. Gdy skończysz edycję, użyj „Eksportuj dane.js” i zastąp
nim dane.js w projekcie. Na hostingu będzie tak samo: wysyłasz nowy dane.js oraz
nowe zdjęcia do odpowiednich folderów.

v23 – GÓRY KACZAWSKIE
---------------------
Uzupełniono wszystkie 8 kategorii Gór Kaczawskich.
Linki w sekcji „Źródła” mają teraz formę wyraźnych zielonych przycisków
z białym tekstem, aby były dobrze widoczne.
