# Gitlab

Tworzymy repozytorium na Gitlabie o nazwie `remotes_practice` i inicjujemy je z README.md
```bash
# Na serwerze Gitlaba wykona się
git init
echo "">README.md
git add .
git commit -m "initial commit"
```

następnie wchodzimy w `bash` i piszemy:
```bash
git clone https://gitlab.com/<username>/remotes_practice.git
cd remotes_practice
git checkout -b feature
echo "Hello world">README.md
git add .
git commit -m "Moja zmiana"
git push --set-upstream origin feature
```

Na stronie internetowej Gitlaba modyfikujemy README.md na branch'u `master` na `Hello universe`.

```bash
# Na serwerze Gitlaba wykona się
git checkout master
echo "Hello universe">README.md
git add .
git commit -m "Update README.md"
```

Pobieramy zmiany i rozwiązujemy merge conflict (można to robić cyklicznie w czasie pracy nad podprojektem):

```bash
git fetch origin
git checkout master
git pull
git checkout feature
git merge master # Powinien nastąpić merge conflict

echo "Hello universe">README.md
git add .
git commit -m "Naprawiono merge conflict."
git push
git log --graph --oneline --all 
```

Wchodzimy na strone remote'a i robimy merge request z `feature` na `master`. Powinien przejść.

```bash
# Na serwerze Gitlaba wykona się
git checkout master
git merge feature
```