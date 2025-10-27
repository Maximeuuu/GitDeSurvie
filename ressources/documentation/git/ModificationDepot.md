# Configuration dans un depot

## A - Changement de nom de dépot (nom et url)

Après avoir changé sur le client web du dépot le nom et l'url :

1. Se déplacer dans le depot : `cd <depot>`
2. Vérifier l'URL distante : `git remote -v`
3. La comparer avec celle du dépot (client web)
4. Mettre à jour l'url distante : `git remote set-url origin <depot>.git`
5. Vérifier : `git remote -v` et `git fetch origin`
6. Changer le nom du dossier : `cd ..` et `mv <old> <new>`