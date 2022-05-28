To jest plik README.md o nauce gita.

Tutaj beda wpisywane komendy dotyczace podstaw gita:

# utworzenie nowego folderu
mkdir -p workspace/nauka_gita

# konfiguracja nauka_gita
git config -l
git config --global user.name "kaememerel"
# nie lubimy spamerów
# (email jest dołączony do zapisów w git/githubie)
git config --global user.email "kaememerel@users.noreply.github.com"

# zauważ, że cała globalna konfiguracja jest w następującym pliku
cat ~/.gitconfig

# sprawdź, czy jesteś we właściwej ścieżce
pwd

# powinienies zobaczyc
# sciezke konczaco sie nauka_gita

# utworz repozytorium
git init

# zawuaz
# ze repozytorium jest w .git/
ls .git/

# zauwaz ze repozytorium ma swoj
# plik konfiguracyjny
cat .git/config

# tworzenie pliku .md
touch README.md

# otwórz edytor atom w katalogu glownym
# repozytorium
atom .

# komendy git
git status
git add README.md
git status
git commit -m "My N commit" # N=1,2,3
git status
git log

# nastepne komendy zeby kolejno dodac plik
git remote add origin https://github.com/kaememerel/nauka_gita.git
git branch -M main
git push -u origin main
