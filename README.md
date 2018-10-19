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

## Instalacja środowiska na MacOS

* https://github.com/radgost/handbook/edit/master/instalacja.md

## Narzędzia / programy

* https://www.sublimetext.com/3
* https://desktop.github.com/
* http://www.psequel.com/ do Postgres
* https://www.sequelpro.com/ do MySQL
* http://pow.cx/

fix do pow.cx (aby pokazywał poprawnie błędy w aplikacji zamiast "End of file reached"): 
```
curl -L https://gist.githubusercontent.com/RobinDaugherty/2731f20d303e6506d451384df2189210/raw/b52e6231170b3dce39633db29634dc892751910f/pow_better_errors_fix.patch | patch ~/Library/Application\ Support/Pow/Versions/0.6.0/node_modules/nack/lib/nack/server.rb 
```

### Edytor kodu

Używamy edytora Sublime 3. Skróty, które warto znać:
* wyszukiwanie pliku po nazwie: CMD + T
* wyszukiwanie metody w pliku: CMD + R
* przechodzenie do linii : CMD + R
* wyszukiwanie w całym projekcie : SHIFT + CMD + F
* uruchanianie pluginów: CMD + SHIFT + P (lub instalacja nowych - trzeba wpisać "install...")

### Bazy danych

## Formatowanie kodu 

```
*.rb - 2 spacje
*.erb - 2 spacje (tak większość bibliotek js jest pisana i nie warto mieć innej konwencji)
```
~~*.erb - 1 tab (czesem trudno sie połapać w tagach html i dlatego jest tab i dla erb powinien być 4 znakowy - konfiguracja w Sublime)~~

## Styl pisania w Ruby
https://github.com/airbnb/ruby (gdyby zniknęło to jest fork https://github.com/radgost/ruby)

# Inspiracje
* http://nvie.com/posts/a-successful-git-branching-model
* https://github.com/radgost/37signals-handbook
