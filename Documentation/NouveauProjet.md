Initaliser un nouveau projet sur GitHub
===

## A - Créer un dépot à partir de git
1. `cd <repertoire>`
2. `git init`
3. verifier si le repertoire existe déjà     : `git remote -v`
4. lier le dépot local et répertoire distant : `git remote add origin <utilisateur>/<dossier>.git`
5. nom de la branche (main/master)           : `git branch`
6. créer un lien permanant et maj dépot      : `git push -u origin master`


## B - Créer un dépot à partir de GitHub
1. `github.io` > `new repository` > `create repository`
2. code > ssh > git@github.com:USER/PROJET.github.io.git
3. git clone git@github.com:USER/PROJET.github.io.git


## C - Partager un dépot
[github.io](https://github.com/) > `<dépot>` > `Settings` > `Manage access` > `invite a collaborator` > `<user>`
