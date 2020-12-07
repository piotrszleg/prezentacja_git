# .gitignore

Plik `.gitignore` to plik tekstowy mówiący o tym jakie pliki git ma omijać.

Każda nowa linia to nowy filter. Możemy ignorować pliki lub foldery.

- `/folder/` - ignoruj folder
- `/plik` - ignoruj plik
- `# komentarz`
- `*` - wildcard czyli dowolny tekst
    - `*.pyc` - ignoruje wszytkie pliki .pyc

Samotne `/` oznacza root repozytorium.

`/folder/` -> `D:/Projekty/repozytorium/folder`

`folder/` - wszytkie foldery w repozytorium o nazwie *folder*

Gotowe pliki do np. projektów Unity3D, NodeJS czy Python'a można znaleźć w internecie.