# Initialiser un dépot

## A - Créer un dépot à partir de git

1. `git init`
2. verifier si le repertoire existe déjà     : `git remote -v`
3. lier le dépot local et répertoire distant : `git remote add origin <utilisateur>/<dossier>.git`
4. nom de la branche (main/master)           : `git branch`
5. créer un lien permanant et maj dépot      : `git push -u origin master`

## B - Créer un dépot à partir de GitHub

1. Créer le dépot : [github.com](https://github.com/) > `new repository` > `create repository`
2. Copier le lien : `code` > `ssh` > `git@github.com:USER/PROJET.github.io.git`
3. Cloner le projet en local : `git clone git@github.com:USER/PROJET.github.io.git`
4. Partager le dépot : [github.io](https://github.com/) > `<dépot>` > `Settings` > `Manage access` > `invite a collaborator` > `<user>`

## C - Créer un dépot local ou sur un serveur personnel

Exemple d'utilisation :

- Lorsqu'il y a des problèmes de confidentialité.
- Possibilité d'initialiser sur un NAS.

1. Créer le dépot depuis le serveur : `git init --bare <PROJET>.git`
  *`--bare` : créé un référentiel qui n’a pas de répertoire de travail (rend impossible la modification des fichiers et la validation des modifications dans ce référentiel)*

2. Copier le lien : `ls` / `dir`
3. Cloner le projet en local : `git clone <CHEMIN>/<PROJET>.git`
