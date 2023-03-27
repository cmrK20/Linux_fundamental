# Exercice 1 : Configurer Git

## 1.
git --version

## 2.
git config --global user.name "fraart"
git config --global user.mail "*@gmail.com"

## 3.
git config --list

# Exercice 2 : Workflow de base avec un seul fichier

## 1.
git init test_repo

## 2.
ls -A

## 3.
git status

## 4.
echo "# Test repository" > readme.md
cat readme.md

## 5.
git status

## 6.
git add readme.md

## 7.
git status

## 8.
git commit -m "Add readme file"

## 9.
git status

## 10.
git log --oneline

## 11.
Quels fichiers ont été validés, quand et avec quel message

# Exercice 3 : Workflow de base avec plusieurs fichiers traités séparément

## 1.
> main.py
> functions.py

## 2.
git status

## 3.
git add main.py

## 4.
git status

## 5.
git commit -m "Add main file"

## 6.
git status
git log --pretty

## 7.
git add functions.py
git commit -m "Add functions file"

## 8.
git status

## 9.
git log --oneline

# Exercice 4 : Workflow de base avec plusieurs fichiers traités en une seule fois

## 1.
> requirement.txt
> .gitignore
> .private

## 2.
git status

## 3.
git add .

## 4.
git status

## 5.
git commit -m "Add standard repo files"

## 6.
git status

## 7.
git log --oneline

# Exercice 5 : Fichiers privés

## 1.
> temp.ipynb

## 2.
git status

## 3.
echo "temp.ipynb" >> .gitignore

## 4.
git status

## 5.
> temp.aux
> temp.log

## 6.
git status

## 7.
vim .gitignore
insert : temp*

## 8.
git status

## 9.
echo ".private*" >> exclude
cat exclude
git status

# Exercice 6 : Différence entre les versions

## 1.
vim readme.md
....
cat readme.md

## 2.
git add readme.md

## 3.
git diff --staged

## 4.
git commit -m "Add description"

## 5.
git diff

## 6.
cd
git diff

## 7.
vim readme.md
-> ....

## 8.
git diff

# Exercice 7 : Annuler

## 1.
rm .*

## 2.
git restore .

## 3.
mkdir backup
cp -rf .git /backup

## 4.
rm -rf Test-repo/

## 5.
mkdir c2
mv .bk_git/.git/ c2

## 7.
git log --oneline

