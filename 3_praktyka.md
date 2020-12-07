```bash
# Tworzenie repozytorium:
> git init

# Łączenie repozytorium z repozytorium online:
> git remote add origin <.git link>
> git remote -v # sprawdzenie

# Klonowanie istniejącego repozytorium z internetu:
> git clone <.git link>

# commit
> git add .
> git commit -m "Krotki naglowek
reszta opisu zmian
wprowadzonych z commitem"

# komunikacja z repozytorium online
> git pull
> git push

# wrzucenie obecnych zmian na stos 
# i przejście do stanu z ostatniego commit'a
> git stash
# reszta komend stash do doczytania

# powrót do wcześniejszego commit'a
> git checkout <id> .
> git stash
> git reset --hard

# Przejście do nowego brancha:
> git branch <nazwa brancha>

# Zmiana brancha:
> git checkout -b <nazwa brancha>

# merge
> git merge <nazwa innego brancha>

# Przykład:
# https://git-scm.com/docs/git-merge
> git checkout -b master
> git merge topic

	  A---B---C topic
	 /
   D---E---F---G master

      A---B---C topic
	 /         \
   D---E---F---G---H master

```

## Konflikt opercji merge
Anulowanie operacji:
```bash
> git merge --abort
```
Jeżeli decydujemy się na rozwiązanie to dostajemy pliki z sekcjami mówiącymi z którego brancha pochodzą jakie zmiany. Ręcznie usuwamy zmiany które nam nie pasują oraz nagłówki gita. Bardzo łatwo robi się to w edytorach z wtyczkami, np. *VS Code*.

Po zakończeniu robimy:
```bash
> git add .
> commit -m "merge conflict resolved"
```