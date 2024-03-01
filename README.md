T: sieć to nie tylko internet, czyli poznajemy topologię sieci komputerowych.
https://pasja-informatyki.pl/sieci-komputerowe/topologie-sieci/

Wyróżniamy topologie fizyczne i logiczne sieci. Topologia fizyczna określa, w jaki sposób urządzenia i hosty
są ze sobą połączone. Topologia logiczna określa sposób przesyłania danych między urządzeniami sieciowymi i hostami.

Wyróżniamy następujące topologie fizyczne:
- topologia magistrali (ang. Bus) 
Topologia magistrali charakteryzuje się tym, że wszystkie urządzenia podłącza się do wspólnego medium transmisyjnego.
Powszechnie stosowanym w tej topologii medium transmisyjnym był kabel koncentryczny.
zalety: - niewielki koszt wdrożenia (brak urządzeń dostępowych)
wady: - mała przepustowość
- podatność na awarie sieci (przerwanie magistrali powoduje brak dostępu do internetu)
 
- topologia 
W topologii pierścienia każde urządzenie podłączone jest z dwoma sąsiadami, tworząc zamknięty krąg. Podobnie jak w przypadku topologii magistrali, przy budowie nie stosuję się dużej ilości okablowania oraz dodatkowych urządzeń.
Zalety: stosowanie małej ilości okablowania, niewielki koszt wdrożenia
Wady: podatność na awarię (przerwanie medium transmisyjnego lub awaria hosta spowoduje brak dostępu do internetu)
 
- topologia gwiazdy
 
W topologii gwiazdy urządzenia podłączone są do centralnego punktu, stanowiącego punkt dostępu do sieci. Dawniej punkt ten stanowiły koncentratory (ang. hub), obecnie natomiast stosuje się przełączniki (ang. switch). Router albo switch.
Zalety: prosta w zaprojektowaniu, łatwa administracja siecią, odporna na awarie
Wady: koszt rozbudowy sieci(wymagane dodatkowe urządzenia), ilość hostów z dostępem do internetu przewodowo zależna od urządzeń sieciowych
- topologia gwiazdy rozszerzonej
Zalety: możliwość łączenia ze sobą mniejszych sieci, ograniczenie liczby kabli między głównym przełącznikiem a znacznie oddalonymi grupami komputerów i urządzeń.
Wada: konieczność rozbudowy infrastruktury o dodatkowe urządzenia, zwiększenie poboru energii przez infrastrukturę, konieczność przygotowania odpowiednich miejsc na dodatkowe przełączniki
- P2P
 



)TOPOLOGIE LOGICZNE
- topologia punkt-punkt 
 W topologii typu punkt-punkt dane przesyłane są od jednego urządzenia do drugiego
Bezpośrednio np. komputer z przeącznikiem, lub pośrednio np. dwa routery
Topologię punkt-punkt wykorzystuje się w topologii fizycznej gwiazdy.

- Topologia przekazywania żetonu(token passing)
W topologii przekazywanaia żetonu dane przekazywane są kolejno do urządzeń połączonych w sieć. Urządzenie, które otrzyma porcję danych, analizuje czy są one kierowane do niego czy też nie. Jeśli dane nie są do niego adresowane, przekazuje je dalej, do sąsiedniego urządzenia. W taki sposób, dane przyesyłane są przez wszystkie urządzenia występujące pomiędzy urządzeniami źródłowym a docelowym
Topologia logiczna wielodostępowa
- umożliwia komunikacje urządzeń w sieci poprzez jedno fizyczne medium transmisyjne. Wykorzystywana jest w topologii fizycznej magistrali

01.03.2024
Temat: Model sieciowy ISO/OSI
(Open Systems Interconnection Reference Model)
Model ten został stworzony w celu normalizacji zasad komunikacji sieci.
Model ten został przygotowany z myślą o tworzeniu tak zwanego systemu otwartego, który nie będzie należał do żadnej zamkniętej sieci.
Model ten jest modelem podglądowym(teoretycznym) i został podzielony na 7 warstw::
7. Warstwa aplikacji – umożliwia komunikację z użytkownikiem(strony www), poczta elektroniczna
6.Warstwa prezentacji – zajmuje się konwersją danych i definiowaniem formatu; odpowiada również za odpowiednie kodowanie danych(szyfrowanie) na urządzeniu źródłowym i ich odkodowanie na urządzeniu docelowym
5.Warstwa sesji – zarządza sesjami użytkowników korzystających np.. ze stron WWW czy komunikacji video.
4.Warstwa transportowa – głównym zadaniem jest sprawna obsługa komunikacji pomiędzy urządzeniami. W warstwie tej dane dzielone są na mniejsze części(segmentowanie), następnie opatrywane są dodatkowymi informacjami, m.in. nadawane są numery porządkowe które pozwalają na przydzielenie do właściwej aplikacji
3. Warstwa sieci- segmenty danych są wzbogacane o nagłówki sieci zawierające adres IP źródła i celu. W ten sposób tworzy się pakiety danych głównym zadaniem warstwy sieciowej jest wybieranie najlepszej drogi od nadawcy do odbiorcy dla stworzonych w niej pakietów
2. Warstwa łącza danych –
1.warstwa fizyczna - 
