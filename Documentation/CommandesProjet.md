Commandes utiles
===

## A - Mettre à jour distant vers local
1. `git pull`


## B - Mettre à jour local vers distant (sans conflits)
1. `git push`


## C - Fusionner projet local et projet distant (avec conflits potentiels)
1. `git add .`
2. `git commit -m "..."`
3. `git pull`
4. Resoudre les conflits potentiels
5. `git add .`
6. `git commit -m "résolution des conflits"`
7. `git push`


## D - Ajouter/Supprimer un fichier
1. liste des fichiers à inclure dans le dépot : `git status`
2. supprimer : `git rm <fichier>`
   ajouter   : `git add <fichier>`
3. informer  : `git commit -m "<fichier> update"`
4. envoyer   : `git push`


***
TODO
***


## Random
- voir les modifications récentes : `git log`
- git add .
- ajouter un dépot distant        : `git remote`
- mettre à jour le dépot distant  : `git push`
- mettre à jour le dépot local    : `git pull`

## A regarder

- git switch + git restore
- git checkout
- git restore --source 11cb5b6 -- hello.txt
- git restore --source 11cb5b6 -SW -- hello.txt

- forcer un reset local :
```
git fetch origin
git reset --hard origin/nom_de_ta_branche
```

- changer le branche par défaut : ``git config --global init.defaultBranch main``


## Branches
Permet de créer des nouvelles fonctionnalités

- branche principale : main / master
- Lorsqu'une branche est créée, tous les fichiers sont copiés dans celle-ci.
- Les modifications apportées sur la branches n'influent pas sur la branche d'origine.

### Commandes affichage
- obtenir la branche    : `git branch`
- arborescence du dépot : `git log --graph --oneline --all --decorate --topo-order`

## Créer une branche
1. créer             : `git checkout -b <nom-branche>`
2. afficher branches : `git branch`
- "*" signifie qu'il s'agit de la branche de travail actuele
- basculer entre les branches : `git checkout <nom-branche>`

## Fusionner une branche dans la principale
1. se déplacer dans la branche 'main' : `git checkout main`
2. fusionner : `git merge <nom-branche>`
