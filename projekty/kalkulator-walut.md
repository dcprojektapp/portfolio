# Kalkulator Walut

> Kursy walut i surowców z oficjalnego API NBP, przelicznik i wykresy historyczne, bez zbędnych reklam.

**Status:** opublikowana · [Google Play](https://play.google.com/store/apps/details?id=com.dawidchaber.kalkulatorwalut) · App Store
**Technologie:** Flutter · flutter_bloc (Cubit) · Clean Architecture · API NBP · testy jednostkowe

## Funkcje
- Aktualne kursy wszystkich walut dostępnych w NBP
- Dowolna waluta bazowa i natychmiastowe przeliczanie
- Wykresy historyczne kursów
- Ulubione waluty pod ręką

## Dla kogo
Podróżni, osoby kupujące online w obcych walutach, inwestorzy, przedsiębiorcy i uczniowie uczący się ekonomii.

## Architektura
Warstwy UI → Cubit → Repository → Data Source z jasnym podziałem odpowiedzialności. Repozytorium zawiera gotowe metadane do App Store i Google Play oraz przewodnik publikacji.
