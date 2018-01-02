# Radgost Handbook

## Brancze

* "master" - na nim jest kod, który jest też na produkcji
* "develop" - kod developowany, który trafia na mastera i później na produkcję
* "test" - każdy PR do develop jest tam od razu mergowany (automatycznie?) i na serwerze testowym można przetestować aktualne funkcjonalności (TODO)

## Statusy PR

* "do poprawy" (jasno czerwone) - wymagane poprawki - opisane w komentarzach
* "konflikty" (jasno czerwone) - konflikty do poprawy
* "poprawione" (zółte) - poprawki poprawione - można sprawdzić i ew. mergować
* "skomplikowane" (fioletowe) - sprawdzający nie chce tego mergować - do obgadania
* "na przyszłość" (jasny fiolet) - odłożone na przyszłość
* "wgrane /u" (zielone) - na serwerze
* "bardzo ważne" (czerwone) - dodaje twórca PR gdy chce aby bardzo szybko został on zmergowany i wgrany
* "do wgrania w nocy" (niebieskie) - dodaje twórca PR gdy np. jest migracja na bazie obciązająca serwer i lepiej wgrać ją w nocy
* "w trakcie testów" (jasno niebieskie) - PR nieskończony, trwają testy lub ktoś go sprawdza

Komentarze do kodu i PR piszemy w języku polskim

## Edytor kodu 

Używamy edytora Sublime 3. Skróty, które warto znać:
* wyszukiwanie pliku po nazwie: CMD + T
* wyszukiwanie metody w pliku: CMD + R
* przechodzenie do linii : CMD + R
* przechodzenie w całym projekcie : SHIFT + CMD + F

## Formatowanie kodu 

```
*.rb - 2 spacje
*.erb - 1 tab (czesem trudno sie połapać w tagach html i dlatego jest tab i dla erb powinien być 4 znakowy - konfiguracja w Sublime)
```

## Styl pisania w Ruby
https://github.com/airbnb/ruby (gdyby zniknęło to jest fork https://github.com/radgost/ruby)

# Inspiracje
* http://nvie.com/posts/a-successful-git-branching-model
* https://github.com/radgost/37signals-handbook
