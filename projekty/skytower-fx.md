# SkyTower-FX AI

> Bot automatyzujący handel pod publikacje makroekonomiczne, z egzekucją przez MetaTrader 5.

**Technologie:** Python · MetaTrader 5 API · ForexFactory i TradingView (kalendarz) · opcjonalnie GPT-4o · Telegram

## Architektura
| Moduł | Rola |
|---|---|
| Kalendarz makro | Feed ForexFactory i zapasowe źródło TradingView, filtrowanie według reguł strategii |
| Backtester | Testowanie strategii na historycznych publikacjach i świecach M1 |
| Silnik decyzji | BUY / SELL / NO_TRADE: GPT-4o albo lokalna heurystyka |
| Ryzyko | Wielkość pozycji z procentu kapitału, limity dzienne, SL/TP, trailing stop |
| Egzekucja | Zlecenia rynkowe i oczekujące, paper trading na żywych cenach |
| Dziennik | CSV każdej transakcji i statystyki skuteczności |
| Watchdog | Alert na Telegramie, gdy bot przestaje odpowiadać |

## Podejście
Projekt zakłada uczciwą ocenę: najpierw minimum 4–8 tygodni na koncie demo, a dopiero potem decyzje. Nie obiecuje zysków.
