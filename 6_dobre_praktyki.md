# Dobre praktyki

## Commit'y

Dobrze jest przeznaczyć pierwszą linijkę wiadomości w commit'cie na tytuł, bo github w niektórych miejscach wyświetla tylko ją zamiast całości.

W commit'cie wypisujemy wszystkie zmiany, najdrobniej jak się da. To pozwala odszukać powód problemu z działaniem kodu, wykonywać merge oraz kompilować listę zmian wersji.

Najlepiej robić commit'y co 20-30 minut, im mniejsza lista zmian w commit'cie tym lepiej. Można zawsze oznaczać jakoś bardziej istotne commit'y lub używać małych branchy i często merge'ować.

## Branch'e

Każdy feature powinien być osobnym branch'em chociaż nie zawsze da się to osiągnąć. Wygodnie pracuje się gdy każdy ma swój branch na którym pracuje nad swoimi zadaniami bo w ten sposób mamy mniej merge conflict'ów.

## Pull request

Cały sens pull request'a to dokumentacja zmian wprowadzonych z branch'em. Powinno się do niego skopiować najważniejsze punkty z commit'ów, uzasadnić zmiany oraz przybliżyć sposób użycia nowych konstrukcji czytającym.