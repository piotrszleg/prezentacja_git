```bash
# Łączenie repozytorium z repozytorium online:
> git remote add origin <.git link>
> git remote -v # sprawdzenie podpiętych repozytoriów 

# Klonowanie istniejącego repozytorium z internetu:
> git clone <.git link>

# komunikacja z repozytorium online
> git pull
> git push

# wrzucenie obecnych zmian na stos 
# i przejście do stanu z ostatniego commit'a
> git stash
# wrzucenie tych zmian z powrotem
> git stash pop
# git stash jest ogólnie fajny do unikania plików tymczasowych
# które sprawdzają się jedynie gdy pracujecie na małym repo

# Zmiana brancha:
> git checkout <nazwa brancha>
# Zmiana brancha na nowy:
> git checkout -b <nazwa brancha>
# Zmiana nazwy branch
> git branch -m <nowa nazwa brancha>

# powrót do wcześniejszego commit'a
> git checkout <id> .
# powrót na branch
> git stash
> git reset --hard

# cherry pick
git cherry-pick <commit>

# interaktywna redukcja commitów 
> git rebase -i master
```