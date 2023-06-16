**Nom :** Maxime Lemoine / Matéo Sa

**Groupe :** B

**Année :** 2023

**IUT Le Havre - Cours GIT**

---

# Compte-rendu TP3 - GitHub en équipe
[tp3](https://abderzah.github.io/Introduction-GIT/tp3/)

Dans ce TP on apprend à travailler en équipe sur un depôt github distant

## Partager un dépot
[github.io](https://github.com/) > `<dépot>` > `Settings` > `Manage access` > `invite a collaborator` > `<user>`

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

## Supprimer un fichier
1. supprimer : `git rm <fichier>`
2. informer  : `git commit -m "<fichier> supprimé"`



