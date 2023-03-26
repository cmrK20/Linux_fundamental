# Exercice 1 - Franck : Grep et awk sur des données tabulaires

## 1.
ls -l

## 2.
ls -l | grep bin

## 3.
ls -l / | grep bin | awk '{print $5}'

## 4.
ls -l / | grep bin | awk '{print $6}'

## 5.
(à remplir avec la commande adaptée)

# Exercice 2 - Franck : Grep avec Regex, et sed sur des données non structurées

## 1.
curl https ://en.wikipedia.org/wiki/List_of_cyberattacks > cyberattacks.txt

## 2.
grep "meta" cyberattacks.txt

## 3.
grep -E "meta \w+" cyberattacks.txt

## 4.
(à remplir avec la commande adaptée)

## 5.
cat cyberattacks.txt | grep -P 'A cyberattack is'
cat cyberattacks.txt | grep -P 'A <a href="/wiki/Cyberattack" title="Cyberattack">cyberattack</a> is any type'
cat cyberattacks.txt | grep -A1 'mw-content-text' | grep -v 'mw-content-text'

## 6.
### Extraire le titre de l'onglet
(à remplir avec la commande adaptée)

### Faire une liste des cyberattaques basée sur les titres de sections
(à remplir avec la commande adaptée)
