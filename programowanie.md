# Programowanie

## Funkcje / klasy

Cześć kodu z danej funkcji/metody wydzielamy do osobnej funkcji tylko gdy:
* aktualna funkcja jest bardzo duża i chcemy zwiększyć czytelność rozbijając ją na mniejsze
* część kodu (nowa funkcja) będzie wywoływana wiele razy

Kod jednej funkcji/metody wydzielamy do osobnego pliku/klasy tylko gdy:
* funkcja jest bardzo duża, powinna mieć wiele podfunkcji (prywatnych) dla czytelności i całość ma skomplikowaną i dużą logikę

Styl kodowania
* jeśli chcemy zmienić jakiś zastany w projekcie styl (podstyl) kodowania to musimy to omówić, aby cały zespół na to się zgodził i przyją ten nowy (lepszy) styl

## Język polski

Komentarze do kodu i PR piszemy w języku polskim. Nazwy zmiennych i metod/funkcji po angielsku.

## Proces tworzenie kodu i PR (Pull-Requestów)

Przed rozpoczęciem pracy nad zadaniem:
* skonsultuj z DevLeadem to jak dane zadanie będzie wykonane (ta osoba będzie sprawdzała / mergowała PR i wiedzieć czego on dotyczy)
* stwórze Branch, gdzie będziesz dodawał/dodawała zmiany w kodzie
* stwórze PR, który zostanie sprawdzony i zmergowany 

Przed stworzeniem PR upewnij się że:
* nazwa PR jest w języku polskim i jasno opisuje czego PR dotyczny
* jest wpisane info o zadaniu którego dotyczy ten PR (opis lub link do zadania)
* dodałeś/aś testy-automatyczne do każdej metody która była dodana/modyfikowana w danym PR (i testy przechodzą)


## Edytor kodu - Sublime

Używamy edytora Sublime.
Nasza konfiguracja: https://github.com/radgost/handbook/blob/master/sublime.md

## Formatowanie kodu 

```
*.rb - 2 spacje
*.erb - 2 spacje (tak większość bibliotek js jest pisana i nie warto mieć innej konwencji)
```

## Styl pisania w Ruby

* staramy się nie używać "unless", a już na pewno nie używamy nigdy z || i &&
* nie używamy "and", "or" - zamiast tego zawsze: || i &&

https://github.com/airbnb/ruby (gdyby zniknęło to jest fork https://github.com/radgost/ruby)


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




## Inspiracja
* http://nvie.com/posts/a-successful-git-branching-model

