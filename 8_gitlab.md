# Gitlab 
Tworzymy repozytorium na Gitlabie o nazwie `remotes_practice`, następnie:
```bash
git clone https://github.com/<nazwa na Gitlabie>/remotes_practice.git
git pull
git checkout -b feature
echo "<imie nazwisko>">README.md
git add .
git commit -m "Moja zmiana"
git push
```

Na stronie internetowej Gitlaba modyfikujemy README.md na branch'u `master` na `Dane: <imie nazwisko>`.

```bash
git checkout master
git pull
git checkout feature
git log --graph --oneline --all 
git merge master
# Powinien nastąpić merge conflict
echo "Dane: <imie nazwisko>">README.md
git add .
git commit -m "Naprawiono merge conflict."
git push
```

Wchodzimy na strone remote'a i robimy push request z `feature` na `master`. Powinien przejść.