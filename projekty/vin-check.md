# VIN Check

> Darmowy dekoder VIN dla aut sprowadzanych z USA.

**Technologie:** czyste PHP 8.2, bez żadnych zależności (bez Composera, bez kroku budowania) · API NHTSA · testy

## Co zawiera raport
| Sekcja | Źródło |
|---|---|
| Dane fabryczne: marka, model, rocznik, silnik, fabryka, wyposażenie bezpieczeństwa | NHTSA vPIC |
| Akcje serwisowe (recalle) | NHTSA Recalls |
| Oceny testów zderzeniowych NCAP | NHTSA Safety Ratings |
| Zgłoszenia usterek, statystyki kolizji i pożarów | NHTSA Complaints |
| Linki do samodzielnego sprawdzenia | NICB, NMVTIS |

## Decyzje projektowe
- Nie istnieje darmowe API odpowiadające na pytanie „czy auto było rozbite”, więc projekt nie udaje, że to sprawdza.
- Zamiast obchodzić zabezpieczenia NICB (captcha, regulamin), raport daje VIN do skopiowania i linki do źródeł.
- Wdrożenie polega na skopiowaniu katalogu na FTP.
